# AWS Selenium Lambda Layer + AWS Lambda Function Full Template

This is an example of set up Selenium testing with AWS lambda layers Python3.6

### File Structure

- seleniumLayer -  https://github.com/kevsersrca/lambda-selenium-layer
- lambda

```bash
── /seleniumLayer/
  ├── /selenium
  │  └──/python/
  │   └── /lib/
  │     └── /python3.6/*
  ├── /chromedriver/
  │ ├── /chromedriver
  │ └── /headless-chromium
  └── /serverless.yaml
── /lambda/
  ├── /handler.py
  └── /serverless.yaml
```


### Deploy Lambda Layers
Go to root directory of project
```bash
$ cd seleniumLayer
$ sls deploy
```

### Deploy Lambda Function
Go to root directory of project
```bash
$ cd lambda
$ sls deploy
```

### Start Testing
Go to root directory of project
```bash
$ cd lambda
$ sls invoke --function hello
```
