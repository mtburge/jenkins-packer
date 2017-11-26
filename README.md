# Jenkins packer templates
This repository contains templates for building machines on AWS running [Jenkins](https://jenkins.io/). The images only install Jenkins, they do not configure the [recommended security controls](https://jenkins.io/doc/book/system-administration/security/).

## Usage
You must have [Packer](https://www.packer.io/downloads.html) installed on your machine. Packer will use the AWS credentials from your current AWS profile environment variables. If you haven't done so already, you **must** run ```aws configure``` prior to running Packer. To build the AMI, select the operating system you want to use and run:
```
packer build amazonlinux.json
```

## Contributing
Please feel free to create a pull request to contribute templates for running Jenkins on other operating systems.

## Further reading
I have created a Medium article detailing step-by-step instructions on how to configure Jenkins on Amazon Linux. You can find that article on Medium: [https://medium.com/@itsmattburgess/installing-jenkins-on-amazon-linux-16aaa02c369c](https://medium.com/@itsmattburgess/installing-jenkins-on-amazon-linux-16aaa02c369c)
