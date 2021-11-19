pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy in parallel') {
            parallel{
                stage('Prod'){
                    steps{
                        echo 'Prod Deploy'
                        }
                }
                stage('dev'){
                    steps{
                        echo 'Devolopment'
                        }
                }
             }
        
        }
    }
}
