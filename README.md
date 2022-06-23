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
--template-body file://templates/http.yaml
```

Deploy the template
```
aws cloudformation create-stack \
--stack-name http \
--template-body file://templates/http.yaml \
--parameters file://parameters/http.yaml
```

Delete stack
```
aws cloudformation delete-stack \
--stack-name http
```
