pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Building in progress...'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
