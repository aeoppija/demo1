pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'cat README.md'
      }
    }
    stage('Cleanup') {
      steps {
        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true, cleanWhenSuccess: true, cleanupMatrixParent: true, cleanWhenUnstable: true, deleteDirs: true)
      }
    }
  }
}