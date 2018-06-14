pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {

                echo 'Deploying....'
            }
        }
    }
}
