pipeline {
    agent none
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('build') {
          steps {
            sh 'pip install -r requirements.txt'
          }
        }
        stage('test') {
          steps {
            sh 'python test.py'
          }   
        }
  }
}
