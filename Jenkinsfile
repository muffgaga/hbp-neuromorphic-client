pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        git(url: 'https://github.com/cpehle/hbp-neuromorphic-client', branch: 'master')
        sh '''#!/bin/bash
env
pip install -r requirements.txt
nosetests
'''
      }
    }
  }
}
