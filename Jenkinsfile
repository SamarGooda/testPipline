pipeline {
    agent any
    stages {
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
