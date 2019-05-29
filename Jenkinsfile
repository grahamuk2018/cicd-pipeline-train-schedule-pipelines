pipeline {
  agent any
  stages {
    stage ("Build") {
      steps {
        echo "Running Build Automation"
        sh "./gradle build --no-daemon"
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    }
  }
}
