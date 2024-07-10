pipeline {
    agent any

    tools {
        maven 'maven 3.9.6'
    }
    stages {
        stage('Voting Build') {
            steps {
                echo 'Compiling the voting app...'
                dir('voting') {
                    sh 'mvn compile'
                }
            }
        }
    }

    post {
        always {
            echo 'Completed the pipeline for craftista...'
        }
    }
}
