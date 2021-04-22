pipeline {
    agent any
    tools {
        maven 'maven-3.6.3' 
		java 'jdk-8'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                sh 'java -version'
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
