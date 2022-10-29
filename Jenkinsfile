pipeline {
    
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build stage, Building...'
            }
        }

         stage('Test') {
             when {
                 expression {
                    BAANCH_NAME == 'main'
                 }
             }
            steps {
                echo 'test stage, Testing..'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deploy stage, Deploying....'
            }
        }
    }
}
