# AWS CloudFormation Helper Scripts
AWS CloudFormation helper scripts can be used to install software and start services on an EC2 instance created as a part of the stack
CloudFormation Helper scripts aren’t executed by default and calls must be included in the template to execute specific helper scripts.
CloudFormation helper scripts are preinstalled on Amazon Linux AMI images.

## cfn-init
cfn-init  can be used to retrieve and interpret resource metadata, install packages, create files, and start services.
cfn-init helper script reads template metadata from the AWS::CloudFormation::Init key and acts accordingly to:
      Fetch and parse metadata from CloudFormation
      Install packages
      Write files to disk
      Enable/disable and start/stop services

## cfn-signal
    cfn-signal can be used to signal with a CreationPolicy or WaitCondition, so you can synchronize other resources in the stack when the prerequisite resource or application is ready.
    cfn-signal script is used in conjunction with a CreationPolicy or an Auto Scaling group with a WaitOnResourceSignals update policy.
    When CloudFormation creates or updates resources with those policies, it suspends work on the stack until the resource receives the requisite number of signals or until the timeout period is exceeded.
    For each valid signal that CloudFormation receives, CloudFormation publishes the signals to the stack events so that you track each signal.

