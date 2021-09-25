pipeline{
  agent any 
    stages {
        stage('Build') { 
            steps {
                   git 'https://github.com/spring-projects/spring-petclinic
'
 
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
        stage('Deploy') { 
            steps {
                // 
            }
        }
    }


}
