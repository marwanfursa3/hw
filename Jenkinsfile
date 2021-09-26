pipeline{
  agent slave
    stages {
        stage('Build') { 
            steps {
                   git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
                   
            }
       }
  stage('cd') { 
            steps {
                   sh "pwd"
              dir('spring-petclinic'){
                 sh "pwd"
              }
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


}
