pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/wengh/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn test verify clean'
      }
    }

  }
}