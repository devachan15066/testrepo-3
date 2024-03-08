pipeline {
  agent {
    kubernetes {
      withCredentials([azureServicePrincipal(credentialsId: 'serviceprincipal_secret_text', variable: 'AZURE_CREDENTIALS')])
      yamlFile 'podtemplate.yaml'
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
