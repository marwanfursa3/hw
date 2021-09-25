pipeline{
  agent any 
    stages {
        stage('Build') { 
            steps {
                   git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
                   
            }
       }
        stage('mvnw ') { 
            steps {
                  script{
                            "./mvnw package"
                   
            }
       }
       
      
        
    }


}
