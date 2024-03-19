pipeline {
  agent {
    kubernetes {
      yamlFile 'podtemplate.yaml'
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
