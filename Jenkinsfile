pipeline {
   agent any
stages {
stage('executeyaml file') {
      steps {
            ansiblePlaybook installation: 'Ansiblerun', inventory: 'dev.inv', playbook: ' createuser.yml '
       }
    }
}
}
