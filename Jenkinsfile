pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                git 'https://github.com/Hemadri92642/jenkins-to-tomcat.git'
            }
        }
        stage('maven build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

