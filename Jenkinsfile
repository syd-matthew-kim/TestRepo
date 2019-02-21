pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'https://github.com/sukantamaikap/TestRepo', branch: 'master', credentialsId: 'user-git')
      }
    }
  }
}