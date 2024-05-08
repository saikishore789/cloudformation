# AWS CloudFormation Helper Scripts
AWS CloudFormation helper scripts can be used to install software and start services on an EC2 instance created as a part of the stack[^1]
CloudFormation Helper scripts aren’t executed by default and calls must be included in the template to execute specific helper scripts.[^2]
CloudFormation helper scripts are preinstalled on Amazon Linux AMI images.[^3]

## cfn-init
cfn-init  can be used to retrieve and interpret resource metadata, install packages, create files, and start services.[^1]
cfn-init helper script reads template metadata from the AWS::CloudFormation::Init key and acts accordingly to:[^2]
[^1]Fetch and parse metadata from CloudFormation
[^2]: Install packages
[^3]: Write files to disk
[^4]: Enable/disable and start/stop services

## cfn-signal

