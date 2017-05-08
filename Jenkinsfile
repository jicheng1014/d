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
            
          },
          "flow3": {
            echo 'aaaaa'
            
          },
          "AA": {
            sh '''sleep 10s
echo "1"'''
            
          }
        )
      }
    }
    stage('flow4') {
      steps {
        parallel(
          "flow4": {
            sh 'echo "1"'
            
          },
          "flow5": {
            echo '1111'
            
          }
        )
      }
    }
    stage('flow6') {
      steps {
        parallel(
          "flow6": {
            echo '1'
            
          },
          "flow7": {
            echo '1111'
            
          }
        )
      }
    }
  }
}