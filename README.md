# Base

7Targets help site built using Jekyll template. Browse through a [live demo](https://orange-ape.cloudvent.net/).

## Develop

Built with [Jekyll](http://jekyllrb.com/) version 3.4.3, but should support newer versions as well.

Install the dependencies with [Bundler](http://bundler.io/):
Go to the directory where you cloned this repo and run the command below. Install Bundler if you do not have it.

~~~bash
$ bundle install
~~~

Run `jekyll` commands through Bundler to ensure you are using the right versions:

~~~bash
$ bundle exec jekyll serve --config _s3_config.yml
~~~

## Release process

1. After merging your changes to `develop` branch the QA site is available at **http://www.7targets-qa.ai.s3-website-us-east-1.amazonaws.com/help/** for you to verify your changes
2. After merging to `master` branch from the `develop` branch, it is released to prod **https://7targets.ai/help**
3. On merge to `master`, it also triggers the pipeline for the help-bot model release

## Support widget

The shared `_layouts/default.html` layout embeds the 7targets support widget from
`js/7targets-chat-widget.js`. Set `chat_widget_enabled: true` or `false` in
`_config.yml` (and `_s3_config.yml` for S3 builds) to show or hide it on the
website. The production S3 config sets `chat_widget_demo_mode: false`; the QA
workflow adds `_qa_config.yml` to keep QA in demo mode.

The widget requests short-lived tokens from
`https://opsrabbit-chat.netbird.aaic.cc/api/opsrabbit/chat-token`. Set
`chat_widget_api_base` in `_s3_config.yml` to the separate HTTPS base URL of
the already-running OpsRabbit Chat API before enabling production traffic.
The token endpoint is not the Chat API and must not be used as its `apiBase`.

The widget's public runtime defaults are supplied at build time through the
widget project's `.env` or `.env.local` file. The static site must never contain
an OpsRabbit admin token, private signing key, SMTP credential, or long-lived
JWT. Leave the upload URL empty until the widget-scoped upload/bind contract is
available; the current OpsRabbit widget route rejects arbitrary `attachment_ids`.

The full agent prompt and SLA skill are documented in the sibling
`../gaurav-exp/docs/plans/7targets-support-widget-integration.md` plan.
