pipeline{
  agent {label 'slave' };
    
     stages {
      
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic'
			}
        }
		stage('change dir') {
            steps {
				sh "pwd"
				dir('spring-petclinic'){
				sh "pwd"
				}
				
			
			}
        }
    
		stage('mvnw') {
			steps {
				script{
					"./mvnw package"
				}
			}

        }
	
    }

}
