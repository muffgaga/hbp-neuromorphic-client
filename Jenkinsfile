@library("jenlib") _

pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        git(url: 'https://github.com/cpehle/hbp-neuromorphic-client', branch: 'master')
        inSingularity(app: "visionary-defaults") {
        sish '''#!/bin/bash       
env
pip install -r requirements.txt
nosetests
'''
        }
      }
    }
  }
}
