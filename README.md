# aws_beanstalk_codecommit_codebuild

## aws beanstalk and codecommit, codebuild

* to use aws codecommit with beanstalk you should follow the below steps:

1. initilize a local git repo 
```
git init 
```
2. add your project files
```
git add .
git commit -am "add files"
```

3. deploy your app
```
eb deploy
```
4. if like to change the branch that the env use to deploy files from use below command:
```
eb use test-env --source codecommit/repo-name/test
```
5. be sure to use version 3.18.1 if you faced an issue of using different branch to be used by your env
```
pip install awsebcli==3.18.1
```
