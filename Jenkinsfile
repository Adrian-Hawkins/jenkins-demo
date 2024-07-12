pipeline {
    agent any
    stages {
        stage("build") {
            steps {
                echo 'building...'
                nodejs('Node-22.4.1') {
                    sh 'npm ci'
                    sh 'npm run build'
                }
                echo 'built'
            }
        }
    }
}