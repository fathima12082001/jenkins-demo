pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Running build stage'
                sh '''
                  echo "Hello Pathu"
                  echo "Pipeline is working"
                  whoami
                  hostname
                  date
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests (dummy stage)'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully 🎉'
        }
        failure {
            echo 'Pipeline failed ❌'
        }
    }
}

