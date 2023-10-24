pipeline {
    agent any
    environment {
        CONECTION_STRING = credentials('ReportingService')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script {
                    def test = 2 +2 > 3? 'cool':'not cool'
                    echo test
                }
                echo "Connection string: ${CONECTION_STRING}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}