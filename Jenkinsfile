pipeline {
  agent any
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            git(url: 'https://github.com/yesdeepakmittal/test-git-actions.git', branch: 'main')
          }
        }

        stage('parallel step') {
          steps {
            echo 'parallel step executing'
          }
        }

      }
    }

  }
}