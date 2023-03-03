pipeline {
    agent any

    tools {
        maven "Maven"
        jdk "JDK-11"
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
