pipeline {
    agent any

    stages {

        stage ('Build Docker Image') { 
            steps {
                script {
                    dockerapp = docker.build("brunohcl/kube-news:v1${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }