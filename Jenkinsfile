pipeline {
  agent any {
    stage ('Build') {
      steps {
        echo "Running build automation"
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainShedule.zip'
      }
    }
  }
}
