pipeline {
  agent any
  stages {

    stage('install npm'){
      steps{
        bat '''npm install'''
      }
    }
    stage('install cypress') {
      steps {
        bat '''
          npm install cypress
        '''
      }
    }
    stage('test') {
      steps {
        bat '''
          npx cypress run --browser chrome'''
      }
    }
  }
}
