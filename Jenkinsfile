pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn install'
            }
        }
         stage('Build the docker image') {
            steps {
                sh 'docker build -t 'shreeshraghunath/spring-petclinic:v1 . && docker images'
            }
        }
    }
}
