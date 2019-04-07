pipeline {
  agent any
  stages {
	stage('Build') {
            steps {
                bat 'install dockerfile:build'
            }
        }
    stage('Deploy') {
      steps {
        bat 'docker-compose up -d'
      }
    }
  }
}