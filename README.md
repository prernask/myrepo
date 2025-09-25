# myrepo

🚀 EC2 + GitHub Setup & Hello World Project (Refined Guide)
1. Launch & Connect to EC2

In AWS console → EC2 → Launch Instance

AMI: Amazon Linux 2023 
GitHub
+1

Instance type: t3.micro (fits Free Tier)

Key pair: create/download a .pem file for SSH

Security Group: allow SSH (port 22) from your IP (or 0.0.0.0/0 for testing, but not recommended for production)

After launch, note the Public DNS or Public IPv4

Connect via SSH from your machine:

chmod 400 key.pem
ssh -i "key.pem" ec2-user@<ec2-public-dns>

2. Update & Install Required Packages
sudo yum update -y
# (Optionally, sudo yum upgrade -y)

# Install Git
sudo yum install git -y
git --version

# Install Python3 (since Amazon Linux 2023 likely has Python 3)
sudo yum install python3 -y
python3 --version


Note: Use python3 explicitly (not python) because many systems don’t symlink python to python3.

3. Configure Git

Inside the EC2 instance, set your global Git identity:

git config --global user.name "Atul Kamble"
git config --global user.email "atul_kamble@hotmail.com"
git config --list

4. Create GitHub Repository

Go to GitHub → New repository

Name it e.g. myrepo

(Optional) initialize with README, add license (MIT is good)

Copy the repository HTTPS URL (or SSH, if you prefer)

5. Clone Repository on EC2

Back in your EC2 terminal:

cd ~
git clone https://github.com/atulkamble/myrepo.git
cd myrepo

6. Create & Test Python “Hello World”
touch helloworld.py
nano helloworld.py


Inside helloworld.py, write:

print("Hello, World from EC2!")


Save & exit (Ctrl+O, Enter, Ctrl+X in nano).
Then run:

python3 helloworld.py


You should see output:

Hello, World from EC2!

7. Push Code to GitHub
git status
git add helloworld.py
git status
git commit -m "Added hello world python file"

GitHub Authentication (PAT / Token)

GitHub no longer accepts account passwords for command-line Git operations; instead:

Go to GitHub → Settings → Developer settings → Personal access tokens (classic)

Generate a token with repo scope

When Git prompts for your password, use this token instead

Then:

git push origin main


If you change the file again, you can:

git pull   # to fetch changes
git add . && git commit -m "Update" && git push

✅ What You Achieve

Instance up & running on EC2

Git & Python installed

Git configured (your name/email)

GitHub repo created

Python “Hello World” file made and run

Changes committed and pushed to GitHub
