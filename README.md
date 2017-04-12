# Apache Guacamole AWS Cloudformation Template

## Creation

`aws cloudformation create-stack --profile siq --template-body file://template.yml --stack-name guacamole-stack`

## Deletion

`aws cloudformation delete-stack --stack-name test-guacamole-large --profile siq`

## SSH

`ssh -i [key] ubuntu@[DNS Name]`
