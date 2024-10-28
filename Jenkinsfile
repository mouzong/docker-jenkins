pipeline {
  agent { dockerfile true }
  stages{
    stage('Checkout'){
      steps{
        git branch: 'main', 
        url: 'https://github.com/mouzong/docker-jenkins.git'
      }
    }
    stage('Test'){
      steps{
        sh '''
          node --version
          git --version
          curl --version
        '''
      }
    }
  }
}
