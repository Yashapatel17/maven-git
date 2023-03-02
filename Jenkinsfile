pipeline {
    agent any
    
    tools {
        maven "Maven"
        jdk "JDK"
    }

    
    stages {
    stage('Checkout'){
        steps{
            
            git 'https://github.com/Yashapatel17/maven-git'
        }

    }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}
