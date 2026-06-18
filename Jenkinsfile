pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/roopalimule/MyMavenApp07.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
