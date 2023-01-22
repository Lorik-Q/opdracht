pipeline {
    agent any
    environment {
        MYSQL_USER=credentials('MYSQL_USER')
        MYSQL_ROOT_PASSWORD=credentials('MYSQL_ROOT_PASSWORD')
        MYSQL_PASSWORD=credentials('MYSQL_PASSWORD')
        MYSQL_DATABASE=credentials('MYSQL_DATABASE')

    }
    stages {
        stage ('Build') {
           steps {
              sh 'docker compose build'
           }
        }
        stage ('Deploy') {
           steps  {
               sh 'docker compose up -d'
           }
        }
    }
}
