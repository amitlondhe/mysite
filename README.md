Install Python3 - 3.8.2
Download and save https://bootstrap.pypa.io/get-pip.py
Install PIP - `python3 get-pip.py`
Install Elastic Beanstalk command line - `pip3 install awsebcli` 

Set your path so you can execute commands from terminal - 
`PATH=$PATH:/Users/<<username>>/Library/Python/3.8/bin`

Create initial project - Be in the folder where you want to create this project
`python3 -m django startproject mysite`


Followed most of - https://realpython.com/deploying-a-django-app-to-aws-elastic-beanstalk


Important Elastic Beanstalk commands used - 
- eb init
- eb create
- eb deploy
- eb config - if you have to change any config item.

Note: During `eb create`, 
 - you need to provide AWS access key that you will generate from AWS console.
 - Also for below question select Y else follow the directions given at the web url. This is due to AWS implementation changes as of October 1st 2024.
Would you like to enable Spot Fleet requests for this environment? (y/N): y
OR
https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/environments-cfg-ec2-imds.html

