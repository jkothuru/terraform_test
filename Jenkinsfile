pipeline {
  agent any
  environment {
    PATH = "${PATH}:${getTerraformPath()}"
  }
  stages{
    stage('terraform '){
      steps{
        sh "terraform -version"
      }
    }
  }
}
def getTerraformPath(){
  def tfHome = tool name: 'terraform-12', type: 'terraform'
  return tfhome
}
