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
--template-body file://templates/http.json
```

Deploy the template
```
aws cloudformation create-stack \
--stack-name http \
--template-body file://templates/http.json \
--parameters file://parameters/http.json
```

Delete stack
```
aws cloudformation delete-stack \
--stack-name http
```
