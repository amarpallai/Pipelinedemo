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
                    step{
                        echo 'Prod Deploy'
                        }
                }
                stage('dev'){
                    step{
                        echo 'Devolopment'
                        }
                }
             }
        
        }
    }
}
