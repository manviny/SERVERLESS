

  npm install -g serverless
  serverless config credentials  --provider aws --key *********** --secret *********** --profile serverless-admin

Cretea new Lambda function
==========================
  sls create --template aws-python --path hello-world-python
  sls create --template aws-java-maven --path hello-java

Deploy
======
  sls deploy -v

Invoke
======
  sls invoke -f hello -l

Deploy just the function
========================
  sls deploy function -f hello

Show logs dinamically
=====================
  sls logs -f hello -t

Remove lambda function
======================
  sls remove

