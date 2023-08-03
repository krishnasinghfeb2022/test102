
pipeline {
    agent {
        ecs {
            inheritFrom 'build-example'
        }
    }
    stages {
      stage('Test') {
          steps {
              script {
                  sh "echo this was executed on non spot instance"
              }
              sh 'ls -lrt'
              sh 'env'
              sh 'whoami'
              sh 'echo sleep is done'
          }
      }
    }
}
