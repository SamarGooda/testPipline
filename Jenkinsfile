pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sudo docker build . 
            }
        }
        stage('two') {
            steps {
                echo "success"
            }
        }
    }
}
