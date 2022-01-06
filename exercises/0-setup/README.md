# Getting Set up for Exercises and Experiments

In this first exercise we'll make sure that we're all set up with our AWS credentials and access to AWS, and then we'll
create a Cloud9 server/environment where we'll run further exercises.

## Log into the AWS Console and Create an Access Key for yourself

1. Log in to AWS using the link, username, and password provided to you
1. In the top bar, near the right, you'll see your username/alias @ introterraform. Clicking on that will display a dropdown
1. In the dropdown, click on "My Security Credentials"
1. This will take you to your security credentials screen/tab. Feel free to change your password if you like, you'll be using this account for the next 2 days.
1. Click "Create access key"
1. An access key and secret will be created for you, **copy the Access key ID and Secret access key (or download a CSV file), we'll use them in setting your environment up below**
1. Close out of the modal/pop-up

## Install Terraform

Run these commands in your cloud9 IDE terminal window to install Terraform

```bash
curl -O https://releases.hashicorp.com/terraform/0.12.29/terraform_0.12.29_linux_amd64.zip
sudo unzip terraform_0.12.29_linux_amd64.zip -d /usr/bin/
```

Then test to ensure it was installed properly.

```bash
terraform -v
```

If you get an error, inform your instructor.

## Pull the exercises repository

The next thing we need to do is pull this repository down so we can use it in future modules. Run the following to 
do this:

```bash
mkdir -p workshop
cd workshop
git clone https://github.com/ferninphilly/intro-to-terraform .
```

Having done that, we should be ready to move on!
