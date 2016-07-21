node('docker-cloud') {
  stage 'Build and Verify'
  checkout scm
  docker.image("maven:3.3.3-jdk8").inside(){
    sh 'mvn verify'
  }
}
