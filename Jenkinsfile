pipeline {
  agent {
    kubernetes {
      yamlFile 'podtemp.yaml'
    }
  }
  stages {
    stage('Build') {
      steps {
        script {
          echo "TESTING AGENT"
          // Add your build steps here
        }
      }
    }
  }
}
