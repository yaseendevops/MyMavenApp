pipeline {
    agent any
    tools {
        maven 'M3'
    }
    stages {
        stage('git') {
            steps{
                git 'https://github.com/yaseendevops/MyMavenApp.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
