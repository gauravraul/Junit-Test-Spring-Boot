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
                sh 'uname'
                sh 'hostname'
                sh 'sudo apt install maven'
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
