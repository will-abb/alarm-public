# Alarm Control App - README

## Overview
The **Alarm Control App** is a serverless application designed to manage alarm notifications using AWS Lambda, AWS CodePipeline, and Slack integration. This project is not complete and was made for for practicing with aws ci/cd services.

## Key Features
- **Lambda Function**: Processes incoming alarm events and integrates with AWS SES and Slack.
- **CI/CD Pipeline**: Automates deployment using AWS CodePipeline and CodeBuild.
- **Slack Integration**: Custom Slack app for notifications and interactions.
- **CloudFormation Templates**: Infrastructure as code for all resources.

## Usage
1. **Build and Deploy**: Configure and run the CI/CD pipeline (`pipeline.yaml`).
2. **Slack Configuration**: Set up the Slack app using `slack-app-manifest.yaml`.
3. **Lambda Function**: Customize the logic in `index.py` to suit your alarm handling requirements.

## Deployment
- Validate templates using the commands in `buildspec.yml`.
- Use `AWS CloudFormation` to deploy resources defined in `template.yaml`.

## Permissions
IAM roles (`code-build-role.json` and `code-pipeline-role.json`) grant necessary permissions for pipeline execution, logging, and resource management.
