# github_intgration_ios-mac_app

Git Integration in iOS/Android:

We may be interested to access info of private repos(list of repos exists in our org account, contributors list to particular repos..etc) from iOS app, for e.g. Project Management app.

It is very easy to get all of this details.
Today we will go with this step by step

STEP 1 =>
First of all you should have to obtain GIT_API_TOKEN, its very easy, just follow the following process.

To obtain API Token
i) Click on following link, 
https://github.com/settings/tokens
then
ii) Click on “Generate new token” button, then 
iii) Enter token description, and select the options which you want to access.
iv) Click on “Generate Token” button

STEP 2 =>
Now by using obtained token you can access different details of private repo as follows:

Note =>
wherever I user OWNER, you should replace it with your org name on github and
wherever I user TOKEN, you should replace it with token obtained in 

STEP 3 :

A)
To get list of private repos 
https://api.github.com/orgs/OWNER/repos?access_token=GIT_API_TOKEN

B)
To get list of contributors to particular repo

https://api.github.com/repos/OWNER/REPO_NAME/contributors?access_token=TOKEN

where OWNER => your organizations name on GitHub

C)
To get commit list on repos:

https://api.github.com/repos/OWNER/REPO_NAME/commits?access_token=TOKEN

Thanks,
If you have any query, you can comment. I will try to help you out whatever possible!!!

Reference :
For more details, you can go through following link.
https://developer.github.com/v3/

Thanks,


