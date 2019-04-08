pipeline {
  agent any
  stages {
    stage('Stop') {
      steps {
        sh 'docker-compose down'
      }
    }
	stage('Build') {
            steps {
                sh 'mvn install dockerfile:build'
            }
        }
    stage('Deploy') {
      steps {
        sh 'docker-compose up -d'
      }
    }
  }
}