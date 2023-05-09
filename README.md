# AWS Code* Services
This Repository will be used for practise with the following AWS services
- AWS CodeBuild
- AWS CodeDeploy
- AWS CodePipeline

Different deployment scenarioes have been completed using this repository
- Set up AWS EC2 instance
- Installed dotnet, CodeDeploy Agent on EC2
- Add correct IAM policies to EC2 user
- Add correct IAM policoes to Code* services accounts
### Scenario 1
- Used CodeBuild to create and artifact and store it in S3
- Used CodeDeploy to consume the artifact and deploy it to an instance of EC2

### Scenario 2
- Published my application and stored the dlls in /app
- Used CodeDeploy on a specific github Commit to deploy my app into an instance of EC2

## appsettings.yml
Depending where your source file is, the appsettings.yml will need to be modified
- S3:             destination: s3://{bucket-name}/{file-name}
- Github commit:  destination: /path/to//hello-world
