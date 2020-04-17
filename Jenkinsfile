pipeline {
    agent any

    stages {
        stage('clean') {
            steps {
                sh "mvn clean -f my-app"
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                sh "mvn test -f my-app"
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package -f my-app"
                echo 'Deploying....'
            }
        }
    }
}
