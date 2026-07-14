Copy and paste the following code:
pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac HelloWorl.java'
            }
        }

        stage('Test') {
            steps {
                bat 'java HelloWorl'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.class', fingerprint: true
            }
        }
    }
}
