pipeline {
    
    agent any
    environment {
        NEW_VERSION = '1.3.0'
    }
    stages {
        stage('build') {
            steps {
                echo 'build stage, Building...'
                echo 'version is ${{NEW_VERSION}'
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
                echo 'version is ${{NEW_VERSION}'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deploy stage, Deploying....'
            }
        }
    }
}
