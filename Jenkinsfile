pipeline {
  agent any
  stages {
    stage('Clean All') {
      steps {
        sh '''sh "rm -rf /var/lib/jenkins/.gradle/caches"
sh "./gradlew clean"'''
      }
    }
    stage('build') {
      steps {
        git(url: 'https://github.com/sukantamaikap/TestRepo', branch: 'master', credentialsId: 'user-git')
      }
    }
  }
}