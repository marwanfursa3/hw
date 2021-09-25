pipeline{
  agent any
    stages {
        stage('Build') { 
            steps {
                   git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
                   
            }
       }
  stage('cd') { 
            steps {
                   sh "pwd"
                        // sh "cat ${spring-petclinic}"
     
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
