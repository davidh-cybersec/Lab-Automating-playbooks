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
Reviewed the README and lab instructions.
Fished setting up SSH authentication on GitHub
Attempted to access the AWS Lab Environment through Canvas.
Received an error indicating the course has ended and is no longer available.
Searched through the course materials but could not find an alternative location for the AWS credentials.


Quick setup — if you’ve done this kind of thing before
or	
git@github.com:davidh-cybersec/AutomatingPlaybooks.git
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line
echo "# AutomatingPlaybooks" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:davidh-cybersec/AutomatingPlaybooks.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin git@github.com:davidh-cybersec/AutomatingPlaybooks.git
git branch -M main
git push -u origin main