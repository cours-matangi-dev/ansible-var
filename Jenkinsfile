pipeline{
    agent any

	stages {

		stage('Ansible') {

			steps {
				ansiblePlaybook(credentialsId: 'ec2terminatekey', inventory: '00_inventory.yml', playbook: 'playbook.yml', extras: '--extra-vars "mot={MAVARJENKINS}"')
			}
		}
    } 
}
