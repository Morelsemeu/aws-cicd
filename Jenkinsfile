pipeline {
  agent any

 environment {
    BRANCH_NAME = 'main'
    GIT_URL = 'https://github.com/Morelsemeu/aws-cicd.git'
 }


  stages {
    stage('git checkout'){
        steps{
            git branch: "${BRANCH_NAME}", url: 'https://github.com/Morelsemeu/aws-cicd.git'
        }
    }
  stage('docker build'){
    steps{
        sh 'docker build -t awscicd . '
        sh 'docker images'
    }
  }
  
  }


}