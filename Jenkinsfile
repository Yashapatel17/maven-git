pipeline {
    agent any

    tools {
        maven "Maven"
        jdk "JDK"
    }

    stages {
        stage('Build') {
            steps {
                withEnv(['JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.18.0.10-1amzn2.0.1.x86_64/bin/java']) {
                    sh 'mvn clean compile'
                }
            }
        }
    }
}
