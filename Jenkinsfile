pipeline {
    agent any

    tools {
        maven "Maven"
        jdk "JDK"
    }

    stages {
        stage('Build') {
            steps {
                withEnv(['JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.18']) {
                    sh 'mvn clean compile'
                }
            }
        }
    }
}
