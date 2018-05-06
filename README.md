The Docker Image contains the aws-cli and kubectl. It is used to update the AWS ECR credentials periodically in a kubernetes cluster.

# Setup

You need to set your credentials in the aws-secrets.yml. Also you need to set your AWS_ACCOUNT and AWS_REGION in ecr-cron.yml.
Afterwords run:

	aws.sh

Afterwords you should be able to see the cron job with:

	kubectl get cronjobs -n infrastructure

# Thanks

This is based on the work of @xynova.

