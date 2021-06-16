pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                git 'https://github.com/valdezpjose/sa'            
                
            }
        }
        
//ANSIBLE BACKEND
        stage('Ansible Backend') {
            steps {
                ansiblePlaybook credentialsId: 'an1', disableHostKeyChecking: true, installation: 'ansible', inventory: 'hosts.inv', playbook: 'backend.yml'            
                
            }
        }

        
        
    }
}