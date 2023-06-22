pipeline {
  agent any
  
  environment {
    MYSQL_ROOT_PASSWORD = credentials('DB_PASSWORD')
  }
  
  stages {

    stage('build') {
      steps {
      	sh 'docker-compose build'
      	}
    }

    stage('run') {
      steps {
      	sh 'docker-compose up -d'
    	}
     }
  }
}
