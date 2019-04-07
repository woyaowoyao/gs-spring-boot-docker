pipeline {
  agent any
  stages {
	stage('Build') {
            steps {
                cmd 'install dockerfile:build'
            }
        }
    stage('Deploy') {
      steps {
        cmd 'docker-compose up -d'
      }
    }
  }
}