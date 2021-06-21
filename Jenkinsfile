pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'https://gitee.com/hgerhardt/auto-test-online-env.git', branch: 'master')
      }
    }

    stage('test') {
      steps {
        bat 'mvn clean test'
      }
    }

  }
}