pipeline {
  agent {
    label 'slave2'
    docker {
      image 'ubuntu:16.04'
      // Run as root to install software
      args '-u root'
    }
  }
  stages {
    stage('Test1'){
      steps {
        sh 'echo hello world'
      }
    }
    stage('Test2'){
      steps {
        sh 'apt-get update'
        sh 'apt-get install -y unzip wget git'
      }
    }
  }
}
