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
        javac Hello.java
        '''
      }
    }
    stage('Execute') {
      steps {
        bat '''
        set PATH=%PATH%
        java Hello
        '''
      }
    }
  }
}
