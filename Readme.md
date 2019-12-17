## Git commands

### to create develop branch
```git commands
git checkout -b origin/develop
```
### to commit to develop branch
```git commands
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/vsprakash2003/awslambda_playground.git
git push -u origin origin/develop
```

## to setup the lambda function
### first time
`claudia create --region us-east-2 --handler index.handler`

### setup trigger for the lambda function from a S3 folder
`claudia add-s3-event-source --bucket my-cute-pizzeria --prefix images/`
here "my-cute-pizzeria" is the S3 bucket name

## to update the lambda function
`claudia update`
