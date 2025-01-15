pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                script {
                    properties([pipelineTriggers([pollSCM('* * * * *')])])
                }
                git 'https://github.com/preach2time1/python_project3.git'
            }
        }
        stage('run python') {
            steps {
                script {
                    sh 'python3 1.py'
                }
            }
        }
    }
}
