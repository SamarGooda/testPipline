pipeline {
    agent any
    stages {
        stage('Cloning our Git') {
           steps {
              git 'https://github.com/SamarGooda/testPipline.git'
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
