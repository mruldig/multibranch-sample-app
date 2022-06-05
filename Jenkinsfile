pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Hello World"
      }
    }
    stage('cat README') {
      when {
        branch "*-warnings-*"
      }
      steps {
        sh '''
          cat README.md
        '''
      }
    }
  }
}
