pipeline {
    agent any

    tools {
        maven 'maven-3.8.6'
        jdk 'jdk-8'
    }
    stages {
        stage('Example') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
