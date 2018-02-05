pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'Start building'
      }
    }
    stage('Archive') {
      steps {
        archiveArtifacts 'Archive'
      }
    }
  }
}