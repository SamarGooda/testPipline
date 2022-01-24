pipeline {
    agent any
    stages {
        stage('install') {
            steps {
                sh "yum install docker"
                  }
            }
        stage('build') {
            steps {
                sh "docker build ."
                  }
            }
        stage('two') {
            steps {
                echo "success"
            }
        }
    }
}
