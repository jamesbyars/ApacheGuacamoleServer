# Apache Guacamole AWS Cloudformation Template

From the [Apache Guacamole](https://guacamole.incubator.apache.org/) site:

Apache Guacamole is a clientless remote desktop gateway. It supports standard protocols like VNC, RDP, and SSH.

We call it clientless because no plugins or client software are required.

Thanks to HTML5, once Guacamole is installed on a server, all you need to access your desktops is a web browser.

## Creation

`aws cloudformation create-stack --template-body file://template.yml --stack-name guacamole-stack --profile siq`

Visit the page at [DNS]:8080/guacamole

## Deletion

`aws cloudformation delete-stack --stack-name guacamole-stack --profile siq`

## SSH

`ssh -i [key] ubuntu@[DNS Name]`
