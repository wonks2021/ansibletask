pipeline {
   agent any
stages {
          stage('Ansible Init') {
            steps {
                script {
                
               def tfHome = tool name: 'AAA'
                env.PATH = "${tfHome}:${env.PATH}"
                 sh 'ansible --version'
                    
            }
            }
        }
        
stage('executeyaml file') {
      steps {
        sh "ansiblePlaybook installation: 'AAA', inventory: 'dev.inv', playbook: 'createuser.yml'"
      }
    }
  }
}
