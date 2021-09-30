pipeline{
  agent {label 'slave' };
    
      stages {
        stage("init") {
            steps {
                script {
                   gv = load "script" 
                }
            }
        }
      }
        stage('Build') { 
            steps {
    script {
                    gv.build()
                }                   
            }
       }
  stage('cd') { 
            steps {
                      script {
                    gv.cd()
                }
            }
            
       }
        stage('mvnw ') { 
            steps {
                     script {
                    gv.mvnw()
                }
            }
       }
       
      
        
    }


}
