pipeline {
    agent any
    tools {
        maven 'apache-maven-3.0.1' 
		java 'jdk8'
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
