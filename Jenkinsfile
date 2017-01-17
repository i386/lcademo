pipeline {
  agent { docker 'openjdk' }
  stages {
    stage('build') {
      steps {
        sh 'mvn clean compile'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
  post {
    always {
      junit '**/target/*.xml'
    }
  }
}
