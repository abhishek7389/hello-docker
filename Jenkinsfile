pipeline {
  agent {
    kubernetes {
      	cloud 'kubernetes'
      	defaultContainer 'jnlp'
      }
    }
  stages {
    stage('Deploy App') {
      steps {
        script {
          kubernetesDeploy(configs: "hellodocker.yml", kubeconfigId: "mykubeconfig")
        }
      }
    }
  }
}
