pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hi') {
            steps {
                echo 'Hi There!'
            }
        }
        stage('Run nodejs file') {
            steps {
               bat 'node index.js'
            }
        }
    }

    post {
        success {
            echo 'It succeeded!'
        }
        failure {
            echo 'It failed!'
        }
    }
}