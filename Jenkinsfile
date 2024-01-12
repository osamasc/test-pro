@Library('utils') _

pipeline {
    agent any
    stages {

        stage('Checkout') {
            steps {
                script {
                    echo env.GIT_COMMIT
                    slack.checkk()
                }
            }
        }

        stage('Hello') {
            steps {
                script {
                    slack('pro', 'tg', 'environment')
                }

            }
        }
    }
}

