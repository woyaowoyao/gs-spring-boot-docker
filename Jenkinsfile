pipeline {
  agent any
  stages {
	stage('Build') {
            steps {
                bat 'mvn install dockerfile:build'
            }
        }
    stage('Deploy') {
      steps {
        bat 'docker-compose up -d'
      }
    }
  }
}