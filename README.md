# AWS Cloudformation scripts

Make creating EC2 instances easier.

## Getting started

List stacks

```
aws cloudformation list-stacks
```

Validate the template
```
aws cloudformation validate-template \
--template-body file://http_server.json
```

Deploy the template
```
aws cloudformation create-stack \
--stack-name http \
--template-body file://http_server.json
```
