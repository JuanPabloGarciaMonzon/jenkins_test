pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                git 'https://github.com/JuanPabloGarciaMonzon/jenkins_test.git'            
                
            }
        }
// PUSH nuevo     
//ANSIBLE BACKEND NUEVO NUEVO NUEVITO
        stage('Ansible Backend') {
            steps {
                ansiblePlaybook credentialsId: 'an1', disableHostKeyChecking: true, installation: 'ansible', inventory: 'hosts.inv', playbook: 'backend.yml'            
                
            }
        }

        
        
    }
}
