pipeline{
  agent any
  stages{
    stage('build') {
      steps{
        sh 'docker pull nginx'
      }
    }
    stage('test') {
      steps{
        sh 'echo "docker image pulled successfully"'
      }
    }
    stage('deploy') {
      steps{
        sh 'docker run nginx'
      }
    }
    stage('checking'){
      sh 'echo "docker image run successfully"'
    }
  }
}
