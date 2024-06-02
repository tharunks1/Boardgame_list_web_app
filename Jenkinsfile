pipeline {
    agent any
    
    tools {
        maven 'maven3'
        jdk 'jdk17'
    }

    stages {
        stage('Git') { 
            steps {
                git branch: 'main', url: 'https://github.com/jaiswaladi246/Boardgame.git'     
                }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'    
                    }
        }
        
        stage('Build') {
            steps {
              sh 'mvn package'    
                }
        }

         stage('clean') {
            steps {
              sh 'mvn clean'    
                }
        }
        
    }
}
