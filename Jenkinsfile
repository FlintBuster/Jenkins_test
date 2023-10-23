pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                scipts {
                    def test = 2 +2 > 3? 'cool':'not cool'
                    exho test
                }
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