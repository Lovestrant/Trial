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
                node index.js
            }
        }
    }
}