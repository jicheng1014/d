pipeline {
  agent any
  stages {
    stage('flow1') {
      steps {
        parallel(
          "flow1": {
            sh 'echo "hello"'
            sleep 10
            
          },
          "flow2": {
            sh 'echo "1"'
            sh 'echo "2"'
            
          }
        )
      }
    }
  }
}