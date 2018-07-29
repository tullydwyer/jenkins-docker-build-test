pipeline {
  agent {
    label 'slave2'
  }
  stages {
    stage('Test1'){
      steps {
        sh 'echo hello world'
      }
    }
    stage('Test2'){
      steps {
        sh 'aws --version'
      }
    }
  }
}
