# CircleCI SE Challenge
Simple Node.js project to demonstrate CircleCI capabilities.

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)

![GitHub language count](https://img.shields.io/github/languages/count/ashleymichaelwilliams/aws-sandbox) ![GitHub top language](https://img.shields.io/github/languages/top/ashleymichaelwilliams/aws-sandbox)<br>
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white) ![AquaSec](https://img.shields.io/badge/aqua-%231904DA.svg?style=for-the-badge&logo=aqua&logoColor=#0018A8) !
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white) ![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)
<br>

## Prerequisites
- [Yarn](https://yarnpkg.com/) and [Node.js](https://nodejs.org/en/).
- Free [Sumo Logic](https://www.sumologic.com/) account w/ CircleCI dashboards & endpoints setup. See [Sumo Logic Orb](https://circleci.com/orbs/registry/orb/circleci/sumologic) and [Sumo Logic Setup Docs](https://circleci.com/docs/2.0/insights/#the-sumo-logic-orb) for details. You should create a few ENV variables at the project-level for this.
- [DockerHub](https://hub.docker.com/) repository for an image.
- [AWS Account, Access, and Secret Keys](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys)
- [AWS ECR](https://aws.amazon.com/ecr/) repository for an image.
- A [context](https://circleci.com/docs/2.0/contexts/) named `demo-prod` with the following ENV variables defined:

Variable Name         | Description 
----------------------|----------------------------------------------------
AWS_ACCESS_KEY_ID     | AWS Access Key ID
AWS_SECRET_ACCESS_KEY | The AWS Secret Key generated with the Access Key ID
AWS_S3_BUCKET_NAME    | URI of bucket name in the form of "s3://bucket-name"
AWS_DEFAULT_REGION    | The default AWS region, set to `us-east-1` or other
AWS_REGION            | Same value as AWS_DEFAULT_REGION
AWS_ECR_ACCOUNT_URL   | URL to the account's ECR, without the repo name (ends in ".com")
AWS_ECR_REPO_NAME     | Name of the repository (e.g "my-image-repo"). `AWS_ECR_ACCOUNT_URL` combines with `AWS_ECR_REPO_NAME` to form the full AWS ECR tag.
DOCKER_LOGIN          | Username for DockerHub login
DOCKER_PWD            | Password to the DockerHub login
DOCKER_TAG            | Full tag for the DockerHub repository (e.g. `username/repo`)

## Setup & Run
1. Clone the repository and run `yarn` to install dependencies.
2. Run `yarn start` to start a simple web server serving the static assets.

## Test
The test uses [TestCafe](https://devexpress.github.io/testcafe/) to run UI tests. It also assumes Chrome and Firefox browsers available on the system.

1. Run `yarn test` to start tests.

## Deploy
[CircleCI](https://circleci.com/) is used to automatically run the tests and, upon manual approval, build Docker images, push them to DockerHub & ECR, and then deploy the website files to S3.

You can visit those jobs by clicking on the status badge above or clicking [here](https://circleci.com/gh/nholuongut/AWS-Tools-for-Cybersecurity/circleci-demo).

I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](bitfield.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.



