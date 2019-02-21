pipeline {
  agent any
  stages {
    stage('ini|') {
      steps {
        git(url: 'https://github.com/sukantamaikap/TestRepo', branch: 'master', credentialsId: 'user-git')
      }
    }
    stage('build') {
      steps {
        sh './gradlew build'
      }
    }
  }
}