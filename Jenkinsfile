pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git(url: 'https://github.com/cpehle/hbp-neuromorphic-client', branch: 'master')
      }
    }
  }
}