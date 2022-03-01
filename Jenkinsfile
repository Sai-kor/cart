@Library('roboshop') _

//nodejs.info 'Starting'
//nodejs.warning 'Nothing to do!'

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
                script{
                    nodejs.info 'compile the code'
                }
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