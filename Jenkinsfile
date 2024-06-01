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
        
        
        stage('Install') {
            steps {
              sh 'mvn clean install'    
                }
        }
        
    }
}
