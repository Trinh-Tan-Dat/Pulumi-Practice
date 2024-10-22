# Pulumi Practice

## Configure AWS
1. Install AWS CLI
```sh
#Download
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

#Unzip file
unzip awscliv2.zip

#Run the install program
sudo ./aws/install

#Confirm the installation
aws --version
```

2. Set up AWS Credentials
```sh
aws configure

# Configure
AWS Access Key ID [None]: YOUR_ACCESS_KEY
AWS Secret Access Key [None]: YOUR_SECRET_KEY
Default region name [None]: us-east-1
Default output format [None]: json
```

```sh
aws configure set aws_session_token YOUR_SESSION_TOKEN
```

## Configure Pulumi
1. Install Pulumi
```sh
curl -fsSL https://get.pulumi.com | sh
```
2. Login to Pulumi
```sh
pulumi login
```

## Create a new project
1. Create a new project
```sh
pulumi new aws-typescript
```
2. Install dependencies
```sh
npm install @pulumi/aws
```
3. Create a new stack
```sh
pulumi stack init dev
```

## Deploy the app
1. Start the app
```sh
pulumi up
```
2. Destroy the app
```sh
pulumi destroy
```
