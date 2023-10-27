pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}

/* Requires the Docker Pipeline plugin */
//pipeline {
//    agent { docker { image 'node:18.18.2-alpine3.18' } }
//    stages {
//        stage('build') {
//            steps {
//                sh 'node --version'
//            }
//        }
//    }
//}

