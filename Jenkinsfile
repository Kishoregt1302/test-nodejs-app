pipeline { 
  
   agent none

   stages {
   
     stage('Install Dependencies') { 
       agent {label 'TomcatJfrog'}
        steps { 
           sh 'npm install' 
        }
     }
     
     stage('Test') {
       agent {label 'TomcatJfrog'}
        steps { 
           sh 'echo "testing application..."'
        }
      }

         stage("Deploy application") { 
           agent {label 'TomcatJfrog'}
         steps { 
           sh 'echo "deploying application..."'
         }

     }
  
   	}

   }
