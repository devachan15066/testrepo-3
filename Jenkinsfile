pipeline {
  agent {
    kubernetes {
      withCredentials([azureServicePrincipal('credentialsId')]) {
        sh 'az login --service-principal -u 6f0a2a84-d215-44f3-ab8b-ec78c64a2bc9 -p 28672742-4976-4c20-80f8-27222df65075 -t 28672742-4976-4c20-80f8-27222df65075'
        yamlFile 'podtemplate.yaml'
      }
    }
  }
  stages {
    stage('Build') {
      steps {
        script {
          echo "TESTING AGENT"
        }
      }
    }
  }
}

