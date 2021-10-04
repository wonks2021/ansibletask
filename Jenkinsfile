pipeline {
   agent any
stages {
          stage('Ansible Init') {
            steps {
                script {
                
               def tfHome = tool name: 'Ansible'
                env.PATH = "${tfHome}:${env.PATH}"
                 sh 'ansible --version'
                    
            }
            }
        }
        
stage('executeyaml file') {
      steps {
        sh "ansible-playbook createuser.yml"
      }
    }
  }
}
