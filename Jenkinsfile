pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'java -version'
      }
    }
    stage('README') {
      when {
        branch "test*"
     }
      steps {
        sh '''
	  cat README.md
	'''  

      }
    }
  }
}
