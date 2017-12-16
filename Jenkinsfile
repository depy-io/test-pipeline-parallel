pipeline {
  agent any
  stages {
    stage('parallel') {
      parallel {
        stage('windows') {
          agent {
            node {
              label 'windows'
            }
          }
          steps {
            echo 'windows slave'
          }
        }
        stage('linux') {
          agent {
            node {
              label 'linux'
            }
          }
          steps {
            echo 'linux slave'
          }
        }
      }
    }
  }
}