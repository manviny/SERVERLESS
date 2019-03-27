
```bash
  npm install -g serverless
  serverless config credentials  --provider aws --key *********** --secret *********** --profile serverless-admin
  


VideoTutorial

1 - Create IAM Role, allow full access to Lambda
2 - Create Java function to upload
3 - Create Lambda Function in AWS
4 - Create .jar in eclipse
5 - upload jar
6 - handler is the package name followed by class name, ej com.amazonaws.lambda.demo.LambdaFunctionHandler
7 - Test function
  
  
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

