pipeline{
    agent any
    stages{
        stage('SCM Checkout'){
            steps{
                git 'https://github.com/aqsa286/Ansible.git'
            }
        }
        stage('Execute Ansible'){
            steps{
                ansiblePlaybook disableHostKeyChecking: true, installation: 'ansible2', inventory: 'hosts', playbook: 'playbook/pkg.yml'
                }
          }
      }
}
