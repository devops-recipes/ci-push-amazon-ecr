# Docker Build, Push and Continuous Integration for a Node JS application

[![Run Status](https://api.shippable.com/projects/59006c891fb3ec0700e1d646/badge?branch=master)](https://app.shippable.com/github/himanshu0503/ci-push-amazon-ecr) [![Coverage Badge](https://api.shippable.com/projects/59006c891fb3ec0700e1d646/coverageBadge?branch=master)](https://app.shippable.com/github/himanshu0503/ci-push-amazon-ecr)

![AyeAye](https://github.com/devops-recipes/ci-push-gcr/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI posses and then pushes the image
to Amazon ECR

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](https://app.shippable.com)
* Create a GCR [integration](http://docs.shippable.com/integrations/imageRegistries/ecr/) on shippable to connect your Amazon ECR account
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `ecr-integration`
* Change the IMAGE_REPO and AWS_ACCOUNT_URL to point to your repo and AWS Account url
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/devops-recipes/ci-push-amazon-ecr/blob/master/public/resources/images/integration.png)

### CI Console Output
![CI Console Output](https://github.com/devops-recipes/ci-push-amazon-ecr/blob/master/public/resources/images/console.png)
