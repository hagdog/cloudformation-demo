pipeline {
  agent any
  stages {
    stage('Submit Stack') {
      steps {
        sh "aws cloudformation create-stack --stack-name cloudformation-demo-stack --template-body file://s3deployment.json --region 'us-east-1'"
      }
    }
  }
}