pipeline {
    agent any
    stages {
        stage('Cloning our Git') {
           steps {
              git 'https://github.com/YourGithubAccount/YourGithubRepository.git'
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
