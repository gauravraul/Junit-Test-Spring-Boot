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
                sh 'uname -a'
                sh 'cat /etc/*release*'
                sh 'hostname'
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
                sh 'printenv'
                sh 'surefire-report:report'
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
