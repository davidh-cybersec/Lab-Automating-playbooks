# CIS-460

## Working with this code repository

1. Set up [SSH authentication to GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Clone your fork to your local environment
3. In your local clone, set the upstream repo: 
`git remote add upstream git@github.com:highlinecollege/CIS-460.git`

## Automating deployment
The Cloudformation template in this repo will deploy an EC2 instance and the
resources it needs for networking. The deployment script is in 
[.github/workflows/deploy.yaml](.github/workflows/deploy.yaml). Running this
script requires [adding secrets to GitHub Actions](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions)

Lab: Automating Playbooks
The Goal: Configure the GitHub repository secrets (AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY) required for the automated deployment workflow.
The Roadblock: The lab guide instructs us to set AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY using values from the Vocareum AWS environment. 

Steps Taken:
Created my GitHub repository and uploaded the assignment files.
I went through and had to research on how to update/modify the bastion.yaml.
Found out how to get the AWS started and where to find the credential.
Created a stack using the template bastion.yaml file and saw the stack already in the assignment
Completed all the steps in the assignment on canvas.
I even played around a bit with the stack and reviewed my playbook steps to verify they would work.
Reviewed the RFI log to see if I missed anything and saw multiple issues I never saw in the assignment.
Reviewed the README.md file and found more actual lab instructions.
Restarted the AWS lab and now understood why there was a ppk
Updated all of the keys in github to connect right. 
I was working on this - Finishing my setting up SSH authentication on GitHub.
Reallized I was all done and that I got the files via the zip and didn't need to download since we were not using the Highline github account. 

