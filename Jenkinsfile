pipeline {
  agent any
  //environment {
    //PATH = "${PATH}:${getTerraformPath()}"
  //}
  stages{
    stage ('Check Terraform Version') {
         steps {
            script {
            def tfhome = tool name: 'Terraform-12', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation'
            env.PATH = "${tfhome}:${env.PATH}"
          }
          sh 'terraform --version'
         }
      }

//def getTerraformPath(){
  //def tfHome = tool name: 'terraform-12', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation'
  //return tfhome
}
}
