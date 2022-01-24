pipeline {
    agent any
    stages {
        stage('test') {
           steps {
               script {
                  withCredentials([usernamePassword(credentialsId: 'my-pass', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
  // available as an env variable, but will be masked if you try to print it out any which way
  // note: single quotes prevent Groovy interpolation; expansion is by Bourne Shell, which is what you want
  sh 'echo $PASSWORD'
  // also available as a Groovy variable
  echo USERNAME
  // or inside double quotes for string interpolation
  echo "username is $USERNAME"
                  }}
                }
            
                 }
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
