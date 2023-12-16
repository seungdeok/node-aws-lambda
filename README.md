# node-aws-lambda-api

Build api using node & aws(IAM, Lambda, API gateway) & circle ci

<br>

## Get Started

#### Prerequisites

1. Use the package manager [node](https://nodejs.org/ko/) to install node package.

2. Use the to deploy

- Create Lambda(under development)

- Update Lambda(on Running)
  - [ ] Create Lambda
  - [ ] Add Lambda Trigger API Gateway on AWS
    - [x] Set cicd.yml "parameters: aws-lambda-function-name" in CircleCI
  - [ ] Add Repo in CircleCI
  - [ ] Setup Environment variables in CircleCI
    - [x] AWS_ACCESS_KEY_ID
    - [x] AWS_REGION
    - [x] AWS_SECRET_ACCESS_KEY

<br>

#### Installation

```bash
npm install
node handler.js
```

<br>

#### CI / CD

```bash
# main branch에서 CI/CD 실행하므로 branch 변경.
git checkout main

# 모든 파일 업로드, '.' 대신 파일이름도 가능.
git add .

# commit message 작성
git commit -m 'commit message'

# on Push branch only main -> Run CircleCI
npm push origin main
```

<br>

## Bug Report

If you find a bug, please report it to me using the [issues](https://github.com/seungdeok/node-aws-lambda-api/issues) page on Github.

<br>

## Contribute

You're free to contribute to this project by submitting [issues](https://github.com/seungdeok/node-aws-lambda-api/issues) and/or [PRs](https://github.com/seungdeok/node-aws-lambda-api/pulls).

<br>

## Reference

https://docs.aws.amazon.com/ko_kr/lambda/latest/dg/nodejs-package.html
https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-awscli.html
