/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:18.18.2-alpine3.18' } }
    stages {
        stage('build') {
            steps {
                sh 'npm i'
                sh 'node index.js'
            }
        }
    }
}

/*
pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'echo "Fail!"; exit 1'
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}
*/

