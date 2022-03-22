pipeline {
  agent any
  stages {
    stage('Clone the repo') {
      steps {
        echo 'Clone the repo'
      }
    }
  }
  post {
    failure {
      emailext body: 'Summary', subject: 'Pipeline Status', to: 'lphan@haeger-consulting.de'
    }
  }
}
