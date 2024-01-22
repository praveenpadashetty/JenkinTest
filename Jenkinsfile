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
        bat 'mvn package'
        sh 'env.Path="C:/workspace/softwares/apache-maven-3.9.6-bin/apache-maven-3.9.6/bin;c:\\\\windows\\\\System32"'
      }
    }

    stage('archiving') {
      steps {
        archiveArtifacts 'target/*.jar'
      }
    }

  }
}