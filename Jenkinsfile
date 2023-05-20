pipeline {
    agent any

    stages {
        stage('git clone') {
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
         stage('deploy tomcat') {
            steps {
                sh 'sudo cp -r annaApps.war /home/ubuntu/apache-tomcat-10.1.9/webapps/'
            }
        }
    }
}


