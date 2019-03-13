
```bash
  npm install -g serverless
  serverless config credentials  --provider aws --key *********** --secret *********** --profile serverless-admin
```
Create new Lambda function
--------------------------
```bash
  sls create --template aws-python --path hello-world-python
  sls create --template aws-java-maven --path hello-java
```

Deploy
------
```bash
  sls deploy -v
```  

Invoke
------
```bash
  sls invoke -f hello -l
```  

Deploy just the function
------------------------
```bash
  sls deploy function -f hello
```  

Show logs dinamically
---------------------
```bash
  sls logs -f hello -t
```

Remove lambda function
----------------------
```bash
  sls remove
```

[Run locally](https://serverless.com/framework/docs/providers/aws/cli-reference/invoke-local/)
-----------
```bash
serverless invoke local --function list
serverless invoke local --function functionName --data '{"a":"bar"}'
```

