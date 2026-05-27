# CIS-460

## Working with this code repository

1. Set up [SSH authentication to GitHub] (https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Clone your fork to your local environment
3. In your local clone, set the upstream repo: 
`git remote add upstream git@github.com:highlinecollege/CIS-460.git`

## Automating deployment
The Cloudformation template in this repo will deploy an EC2 instance and the
resources it needs for networking. The deployment script is in 
[.github/workflows/deploy.yaml](.github/workflows/deploy.yaml). Running this
script requires [adding secrets to GitHub Actions](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions)

## Lab: Automating Playbooks
As computing infrastructure becomes 'hyperconvergedLinks to an external site.', incident response playbooks can be written for the CSIRT and for the computers they work with. In other words, a playbook can be interpreted by responders as well as server environments. Playbooks can be part of infrastructure as code.
1.	Log into GitHub and access this GitHub ClassroomLinks to an external site..
•	GitHub will ask you to map your GitHub account to your identity in Canvas and will automatically fork the assignment repo. Clone this fork to your development environment.
•	In your fork of the repo you will find a CloudFormation template, bastion.yaml, that defines a virtual machine and the network it runs in.
•	This repo includes an automated deployment script, .github/workflows/deploy.yaml, that can log into AWS and generate the infrastructure defined in the CloudFormation template. Set two secrets on the repo, AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY using values from your Vocareum labs AWS environment. Every time you push to your fork's main branch, the automation will run.
2.	Cut a new branch in your local clone. In that branch, modify bastion.yaml to do the following:
A.	Add a security group that would isolate the bastion host from any communication within the VPC or with the public Internet.
B.	Add comments to the CloudFormation template with incident response playbook steps that can be used to contain the bastion for a scenario that requires isolation and investigation. Consider a scenario like anomalous network activity detected through automated monitoring on the network. Make sure one of the containment steps shows how to update the security groups assigned to the bastion for isolation.
C.	Add a comment above the line that assigns security groups to the bastion that would allow shell access from inside the network.
3.	Push your branch to your fork on GitHub and open a pull request to class upstream repo. Post the URL of your pull request to this Canvas assignment.

## Steps Taken:
•	Created my GitHub repository and uploaded the assignment files. 
•	I went through and had to research on how to update/modify the bastion.yaml. 
•	Found out how to get the AWS started and where to find the credential. 
•	Created a stack using the template bastion.yaml file and saw the stack already in the assignment. 
•	Completed all the steps in the assignment on canvas. 
•	I even played around a bit with the stack and reviewed my playbook steps to verify they would work. 
•	Reviewed the RFI log to see if I missed anything and saw multiple issues I never saw in the assignment. 
•	Reviewed the README.md file and found more actual lab instructions. 
•	Restarted the AWS lab and now understood why there was a ppk. 
•	Updated all of the keys in GitHub to connect right. 
•	I did find the AWS: ssh://ec2-3-83-161-207.compute-1.amazonaws.com
•	I was working on this - Finishing my setting up SSH authentication on GitHub. 
•	Realized I was all done and that I got the files via the zip and didn't need to download since we were not using the Highline GitHub account.
