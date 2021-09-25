pipeline{
  agent any 
    stages {
        stage('Build') { 
            steps {
                   git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic.git'
                   
            }
       }

 stage('read') {
           steps {
               script {
                   def data = readFile(file: 'spring-petclinic')
                   println(data)
               }
           }
       }
 stage('cd') { 
            steps {
                   sh "cd spring-petclinic"
                   
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
