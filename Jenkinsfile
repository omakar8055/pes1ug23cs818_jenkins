pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o pes1ug23cs818-1 main.cpp' // Compiling the C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './pes1ug23cs818-1' // Running the compiled file
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment steps if required
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
