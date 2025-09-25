# myrepo

Practice commands  Powershell:-

PS C:\Users\Prerana> ssh -i .\Desktop\awskey\110-pem ec2-user@13.201.87.194
The authenticity of host '13.201.87.194 (13.201.87.194)' can't be established.
ED25519 key fingerprint is SHA256:VOCFudk7DoBWl+TKeeUD/rZ7GZojA8bF+WFrTDo5toM.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '13.201.87.194' (ED25519) to the list of known hosts.
   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
[ec2-user@ip-172-31-41-33 ~]$ sudo yum update -y
Amazon Linux 2023 Kernel Livepatch repository                                                                               174 kB/s |  23 kB     00:00
Dependencies resolved.
Nothing to do.
Complete!
[ec2-user@ip-172-31-41-33 ~]$ sudo yum install git -y
Last metadata expiration check: 0:00:12 ago on Thu Sep 25 17:46:01 2025.
Dependencies resolved.
============================================================================================================================================================
 Package                                Architecture                 Version                                        Repository                         Size
============================================================================================================================================================
Installing:
 git                                    x86_64                       2.50.1-1.amzn2023.0.1                          amazonlinux                        53 k
Installing dependencies:
 git-core                               x86_64                       2.50.1-1.amzn2023.0.1                          amazonlinux                       4.9 M
 git-core-doc                           noarch                       2.50.1-1.amzn2023.0.1                          amazonlinux                       2.8 M
 perl-Error                             noarch                       1:0.17029-5.amzn2023.0.2                       amazonlinux                        41 k
 perl-File-Find                         noarch                       1.37-477.amzn2023.0.7                          amazonlinux                        25 k
 perl-Git                               noarch                       2.50.1-1.amzn2023.0.1                          amazonlinux                        41 k
 perl-TermReadKey                       x86_64                       2.38-9.amzn2023.0.2                            amazonlinux                        36 k
 perl-lib                               x86_64                       0.65-477.amzn2023.0.7                          amazonlinux                        15 k

Transaction Summary
============================================================================================================================================================
Install  8 Packages

Total download size: 7.9 M
Installed size: 41 M
Downloading Packages:
(1/8): git-2.50.1-1.amzn2023.0.1.x86_64.rpm                                                                                 1.5 MB/s |  53 kB     00:00
(2/8): perl-Error-0.17029-5.amzn2023.0.2.noarch.rpm                                                                         1.9 MB/s |  41 kB     00:00
(3/8): git-core-doc-2.50.1-1.amzn2023.0.1.noarch.rpm                                                                         38 MB/s | 2.8 MB     00:00
(4/8): perl-File-Find-1.37-477.amzn2023.0.7.noarch.rpm                                                                      1.2 MB/s |  25 kB     00:00
(5/8): git-core-2.50.1-1.amzn2023.0.1.x86_64.rpm                                                                             47 MB/s | 4.9 MB     00:00
(6/8): perl-Git-2.50.1-1.amzn2023.0.1.noarch.rpm                                                                            1.3 MB/s |  41 kB     00:00
(7/8): perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64.rpm                                                                      1.2 MB/s |  36 kB     00:00
(8/8): perl-lib-0.65-477.amzn2023.0.7.x86_64.rpm                                                                            727 kB/s |  15 kB     00:00
------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                        52 MB/s | 7.9 MB     00:00
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                    1/1
  Installing       : git-core-2.50.1-1.amzn2023.0.1.x86_64                                                                                              1/8
  Installing       : git-core-doc-2.50.1-1.amzn2023.0.1.noarch                                                                                          2/8
  Installing       : perl-lib-0.65-477.amzn2023.0.7.x86_64                                                                                              3/8
  Installing       : perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64                                                                                        4/8
  Installing       : perl-File-Find-1.37-477.amzn2023.0.7.noarch                                                                                        5/8
  Installing       : perl-Error-1:0.17029-5.amzn2023.0.2.noarch                                                                                         6/8
  Installing       : perl-Git-2.50.1-1.amzn2023.0.1.noarch                                                                                              7/8
  Installing       : git-2.50.1-1.amzn2023.0.1.x86_64                                                                                                   8/8
  Running scriptlet: git-2.50.1-1.amzn2023.0.1.x86_64                                                                                                   8/8
  Verifying        : git-2.50.1-1.amzn2023.0.1.x86_64                                                                                                   1/8
  Verifying        : git-core-2.50.1-1.amzn2023.0.1.x86_64                                                                                              2/8
  Verifying        : git-core-doc-2.50.1-1.amzn2023.0.1.noarch                                                                                          3/8
  Verifying        : perl-Error-1:0.17029-5.amzn2023.0.2.noarch                                                                                         4/8
  Verifying        : perl-File-Find-1.37-477.amzn2023.0.7.noarch                                                                                        5/8
  Verifying        : perl-Git-2.50.1-1.amzn2023.0.1.noarch                                                                                              6/8
  Verifying        : perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64                                                                                        7/8
  Verifying        : perl-lib-0.65-477.amzn2023.0.7.x86_64                                                                                              8/8

Installed:
  git-2.50.1-1.amzn2023.0.1.x86_64                    git-core-2.50.1-1.amzn2023.0.1.x86_64               git-core-doc-2.50.1-1.amzn2023.0.1.noarch
  perl-Error-1:0.17029-5.amzn2023.0.2.noarch          perl-File-Find-1.37-477.amzn2023.0.7.noarch         perl-Git-2.50.1-1.amzn2023.0.1.noarch
  perl-TermReadKey-2.38-9.amzn2023.0.2.x86_64         perl-lib-0.65-477.amzn2023.0.7.x86_64

Complete!
[ec2-user@ip-172-31-41-33 ~]$ git --version
git version 2.50.1
[ec2-user@ip-172-31-41-33 ~]$ sudo yum install python -y
Last metadata expiration check: 0:00:31 ago on Thu Sep 25 17:46:01 2025.
Dependencies resolved.
============================================================================================================================================================
 Package                                        Architecture               Version                                    Repository                       Size
============================================================================================================================================================
Installing:
 python-unversioned-command                     noarch                     3.9.23-1.amzn2023.0.3                      amazonlinux                      11 k

Transaction Summary
============================================================================================================================================================
Install  1 Package

Total download size: 11 k
Installed size: 23
Downloading Packages:
python-unversioned-command-3.9.23-1.amzn2023.0.3.noarch.rpm                                                                 340 kB/s |  11 kB     00:00
------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                       188 kB/s |  11 kB     00:00
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                    1/1
  Installing       : python-unversioned-command-3.9.23-1.amzn2023.0.3.noarch                                                                            1/1
  Running scriptlet: python-unversioned-command-3.9.23-1.amzn2023.0.3.noarch                                                                            1/1
  Verifying        : python-unversioned-command-3.9.23-1.amzn2023.0.3.noarch                                                                            1/1

Installed:
  python-unversioned-command-3.9.23-1.amzn2023.0.3.noarch

Complete!
[ec2-user@ip-172-31-41-33 ~]$ python --version
Python 3.9.23
[ec2-user@ip-172-31-41-33 ~]$
[ec2-user@ip-172-31-41-33 ~]$
[ec2-user@ip-172-31-41-33 ~]$ git config --global user.name "Prerana Karande"
[ec2-user@ip-172-31-41-33 ~]$ git config --global user.email "karandeprerna@gmail.com"
[ec2-user@ip-172-31-41-33 ~]$ git config --list
user.name=Prerana Karande
user.email=karandeprerna@gmail.com
[ec2-user@ip-172-31-41-33 ~]$ git clone https://github.com/prernask/myrepo.git
Cloning into 'myrepo'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (4/4), done.
[ec2-user@ip-172-31-41-33 ~]$ ls
myrepo
[ec2-user@ip-172-31-41-33 ~]$ cd myrepo
[ec2-user@ip-172-31-41-33 myrepo]$ ls
LICENSE  README.md


[ec2-user@ip-172-31-41-33 myrepo]$ python3 helloworld.py
Hello, World from EC2!!!
[ec2-user@ip-172-31-41-33 myrepo]$
[ec2-user@ip-172-31-41-33 myrepo]$
[ec2-user@ip-172-31-41-33 myrepo]$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        helloworld.py

nothing added to commit but untracked files present (use "git add" to track)
[ec2-user@ip-172-31-41-33 myrepo]$ git add helloworld.py
[ec2-user@ip-172-31-41-33 myrepo]$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   helloworld.py

[ec2-user@ip-172-31-41-33 myrepo]$ git commit -m "added hello world"
[main f05ec30] added hello world
 1 file changed, 1 insertion(+)
 create mode 100644 helloworld.py
[ec2-user@ip-172-31-41-33 myrepo]$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

[ec2-user@ip-172-31-41-33 myrepo]$ git push origin main
Username for 'https://github.com': Prerana Karande
Password for 'https://Prerana%20Karande@github.com':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 354 bytes | 354.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/prernask/myrepo.git
   e319de4..f05ec30  main -> main
[ec2-user@ip-172-31-41-33 myrepo]$ git pull
Already up to date.
[ec2-user@ip-172-31-41-33 myrepo]$


<img width="1915" height="910" alt="image" src="https://github.com/user-attachments/assets/20df552e-d4cf-4be6-9f09-f2e919116665" />
