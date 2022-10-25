Jenkinsfile (Declarative Pipeline)
/* Requires the Docker Pipeline plugin */
pipeline {
    
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build stage, step 1'
            }
        }

         stage('Test') {
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
