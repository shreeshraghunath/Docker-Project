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
                sh 'docker build -t 'shreeshraghunath/spring-petclinic-987 . '
                sh 'docker images'
            }
        }
    }
}
