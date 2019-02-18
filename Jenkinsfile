pipeline {
    agent any
    tools {
        tool name: 'M3', type: 'maven'
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
