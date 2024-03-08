pipeline {
    agent {
        kubernetes {
            withCredentials([azureServicePrincipal('serviceprincipal_secret_text')]) {
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
