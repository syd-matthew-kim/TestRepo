pipeline {
  agent any
  stages {
    stage('init') {
      steps {
        git(url: 'https://github.com/sukantamaikap/TestRepo', branch: 'master', credentialsId: 'user-git')
      }
    }
    stage('build') {
      steps {
        sh './gradlew build'
      }
    }
    stage('test') {
      steps {
        sh './gradlew test'
      }
    }
  }
}