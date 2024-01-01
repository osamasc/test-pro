@Library('utils') _

import de.check24.energy.Slack

pipeline {
    agent any
    stages {

        stage('Checkout') {
            steps {
                script {
                    slack.checkk()
                    slack.sendReleaseMessage("r20230915-105717")
                }
            }
        }

        stage('Hello') {
            steps {
                script {
                    slack.changeReleaseToDiff("r20230915-105717")
                }

            }
        }
    }
}

