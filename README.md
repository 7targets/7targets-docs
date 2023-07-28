# Base

7Targets help site built using Jekyll template. Browse through a [live demo](https://orange-ape.cloudvent.net/).

## Develop

Built with [Jekyll](http://jekyllrb.com/) version 3.4.3, but should support newer versions as well.

Install the dependencies with [Bundler](http://bundler.io/):
Go to the directory where you clone this repo and run below command. Install Bundler if you do not have it.

~~~bash
$ bundle install
~~~

Run `jekyll` commands through Bundler to ensure you're using the right versions:

~~~bash
$ bundle exec jekyll serve  --config _s3_config.yml
~~~

## Release process
1. After merging your changes to `develop` branch the QA site is available at **http://www.7targets-qa.ai.s3-website-us-east-1.amazonaws.com/help/** for you to verify your changes
2. After merging to `master` branch from the `develop` branch, it is released to prod **https://7targets.ai/help**
3. On merge to master, it also triggers the pipeline for tbe help-bot model release
