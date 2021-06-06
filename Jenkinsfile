pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install aws-project petclinic  --set image.repository=registry.hub.docker.com/felixgokmen/aws-project-maven --set image.tag=0.1'
              			
            }           
        }
    }
}
