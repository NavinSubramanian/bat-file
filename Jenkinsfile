pipeline {
  agent any
  environment {
    PATH = "C:\\WINDOWS\\SYSTEM32"
  }
  stages {
    stage('Build') {
      steps {
        bat '''
        set PATH=%PATH%
        echo Starting hello World pipeline
        '''
      }
    }
    stage('Check') {
      steps {
        bat '''
        set PATH=%PATH%
        hello.bat
        '''
      }
    }
  }
}
