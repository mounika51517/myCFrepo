pipeline {
    agent any

    stages {
        stage('create_stack') {
            steps {
                sh 'aws cloudformation create-stack --stack-name vpc-stack --template-body file://VPC_stack.yml --region "us-east-1"'
            }
        }
    }
}
