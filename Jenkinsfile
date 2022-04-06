pipeline{
 agent any
  stages{
    stage('build'){
      steps{
       echo "starting automation build"
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
