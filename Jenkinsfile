pipeline {
  agent any

  stages {
    stage('git checkout'){
        steps{
            git branch: 'main', url: 'https://github.com/Morelsemeu/aws-cicd.git'
        }
    }
  stage('test'){
    steps{
        sh 'echo test'
    }
  }
  stage('prod'){
    steps{
        sh 'echo prod'
    }
  }

  }


}