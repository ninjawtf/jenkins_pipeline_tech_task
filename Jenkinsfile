pipeline {
    agent any

    tools {
        maven 'maven-3.8.6'
        jdk 'jdk-8'
    }
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git url:'https://github.com/jglick/simple-maven-project-with-tests.git',
                    branch: '*'

                // Run Maven on a Unix agent.
                // sh "mvn -Dmaven.test.failure.ignore=true clean package"
                sh "env"
                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
    }
}
