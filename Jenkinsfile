pipeline {
   agent any
stages {
stage('executeyaml file') {
      steps {
        sh '''
          ansible --version
          ansible-playbook --version
          ansible-galaxy --version
        '''
      }
    }
  }
}
