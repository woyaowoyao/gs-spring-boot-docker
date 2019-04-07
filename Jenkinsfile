pipeline {
  agent any
  stages {
    stage('Stop') {
      steps {
        bat 'docker-compose down'
      }
    }
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