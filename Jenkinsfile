pipeline {
  agent any
  environment {
    PATH = "C:\\WINDOWS\\SYSTEM32"
    JAVA_HOME='C:\\Program Files\\Java\\jdk-17'
  }
  stages {
    stage('Build') {
      steps {
        bat '''
        set PATH=%JAVA_HOME%;%PATH%
        echo Starting hello World pipeline
        javac Hello.java
        '''
      }
    }
    stage('Execute') {
      steps {
        bat '''
        set PATH=%JAVA_HOME%;%PATH%
        java Hello
        '''
      }
    }
  }
}
