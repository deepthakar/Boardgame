pipeline {
    agent any
    
    tools{
        maven 'maven3'
        jdk 'java 17'
    }

    stages {        
        stage('Compile') {
            steps {
               sh "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
