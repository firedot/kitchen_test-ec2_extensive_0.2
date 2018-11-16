# kitchen_test-ec2_extensive_0.2
Example of extensive kitchen test for AWS EC2 instance


# What is this reposiotry about
This repository is based on the following tutorial: 

[Detailed Review of the features of Kitchen-Terraform](https://newcontext-oss.github.io/kitchen-terraform/tutorials/extensive_kitchen_terraform.html)

# Prerequisites
- AWS Account
- AWS CLI installed 
- Terraform installed
- rbenv installed
- Ruby installed
- bundle installed

**NOTE:** **The following steps are for MacOS users** **:NOTE**

 * Install and fine tune rbenv by running the following commands
   
```
which rbenv || brew install rbenv

grep ".rbenv" ~/.bash_profile || {
  echo 'export PATH="$HOME/.rbenv/bin:$PATH"' | tee -a ~/.bash_profile
}

source ~/.bash_profile

rbenv init
```
 * Install ruby version 2.3.1 with rbenv by running the following commands

```
rbenv versions | grep 2.3.1 || rbenv install 2.3.1

rbenv local 2.3.1

```

 * Install bundler
 
 ```
 gem install bundler
 ```

## TO-DO

## DONE

- Configure AWS
- Create InSpec Profile
- Generate SSH Key
- Create Test Fixture Terraform Configuration
- Create Test Kitchen Configuration script


### How to use this repository

- Clone the repository to your local machine

```
git clone https://github.com/firedot/kitchen_test-ec2_extensive_0.2.git
```
- Go into the cloned repo directory 

```
kitchen_test-ec2_extensive_0.2
```
- Configure your AWS Credentials according to these instructions: 

[Configuring the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html#cli-quick-configuration)

- Run the following command to test the terraform module

```
./run-test.sh
```

