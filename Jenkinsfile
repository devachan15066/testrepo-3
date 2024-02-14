pipeline {
  agent {
    kubernetes3 {
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
