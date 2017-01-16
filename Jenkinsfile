pipeline {
  agent { docker 'openjdk' }
  stages {
    stage ("build") {
      steps {
        sh 'mvn clean compile'
      }
    }
  }
}
