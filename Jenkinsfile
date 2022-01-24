pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                docker build . 
                  }
            }
        stage('two') {
            steps {
                echo "success"
            }
        }
    }
}
