pipeline {
    agent { docker { image 'golang:1.17.5-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
                sh 'XDG_CACHE_HOME=/tmp/.cache go run main.go'
            }
        }
    }
}
