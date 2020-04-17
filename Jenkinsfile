pipeline {
    agent any

    stages {
        stage('clean') {
            steps {
                sh "mvn clean"
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                sh "mvn test"
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package"
                echo 'Deploying....'
            }
        }
    }
}
