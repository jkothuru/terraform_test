pipeline {
  agent any
  stages{
    stage ('Check Terraform Version') {
         steps {
            script {
            def tfhome = tool name: 'terraform-12', type: 'org.jenkinsci.plugins.terraform.TerraformInstallation'
            env.PATH = "${tfhome}:${env.PATH}"
          }
          sh 'terraform --version'
         }
      }
}
}
