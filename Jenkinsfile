pipeline {
  agent any
  stages {
    stage('clean package'){
      agent {label "slave-node-2"}
                 steps{
        // echo "cleaning the package"
        sh 'mvn clean package'
      }
    }
    stage('install'){
      agent {label "slave-node"}
                steps{
        // echo "install the package"
        sh 'mvn install'
      }
    }
  }
}
