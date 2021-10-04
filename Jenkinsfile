pipeline {
   agent any
stages {
stage('executeyaml file') {
      steps {
            ansiblePlaybook inventory: 'dev.inv', playbook: ' createuser.yml '
       }
    }
}
}
