pipeline {
  agent any 
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
