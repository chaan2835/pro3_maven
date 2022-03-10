pipeline {
  agent any
  stages {
    stage('clean package'){
           steps{
        // echo "cleaning the package"
        sh 'mvn clean package'
      }
    }
    stage('install'){
            steps{
        // echo "install the package"
        sh 'mvn install'
      }
    }
  }
}
