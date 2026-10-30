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
            mail to: 'lovestrantkemboi@gmail.com', subject: "Jenkins  ${env.JOB_NAME} Pipeline Success", body: 'The Jenkins pipeline has completed successfully.'
        }
        failure {
            echo 'It failed!'
            mail to: 'lovestrantkemboi@gmail.com', subject: "Jenkins ${env.JOB_NAME} Pipeline Failure", body: 'The Jenkins pipeline has failed.'
        }
    }
}