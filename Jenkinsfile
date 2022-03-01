@Library('roboshop') _

log.info 'Starting'
log.warning 'Nothing to do!'

pipeline{
    agent{
        label 'WORKSTATION'
    }
    //Auto trigger
    triggers {
        pollSCM('*/2 * * * *')
    }
    stages{
        stage('compile the code'){
            steps{
                sh 'echo compile the code'
            }
        }
        stage('check the code quality'){
            steps{
                sh 'echo check the code quality'
            }
        }
        stage('Test cases'){
            steps{
                sh 'echo Test cases'
            }
        }

    }
}