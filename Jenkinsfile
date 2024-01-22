pipeline {
  agent any
  stages {
    stage('Pull Request') {
      steps {
        git(url: 'https://github.com/praveenpadashetty/JenkinTest.git', branch: 'master')
      }
    }

    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('archiving') {
      steps {
        echo 'archiving'
      }
    }

  }
}