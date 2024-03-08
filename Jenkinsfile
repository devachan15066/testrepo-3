pipeline {
  agent {
    kubernetes {
      withCredentials([azureServicePrincipal('Azure_service_principal')]) {
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

