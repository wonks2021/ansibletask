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
        ansiblePlaybook credentialsId: 'private-key', installation: 'AAA', inventory: 'dev.inv', playbook: 'createuser.yml'
      }
    }
  }
}
