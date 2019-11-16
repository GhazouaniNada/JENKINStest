pipeline {
    agent {
        label "master"
    }
   
    
    stages {
        stage("clone code") {
            steps {
                script {
                    // Let's clone the source
                    git 'https://github.com/GhazouaniNada/JENKINStest.git';
                }
            }
        }
        stage("mvn build") {
            steps {
                script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat "mvn package -DskipTests=true"
                }
            }
        }
        stage("mvn clean install 11454yyyyrrrr4477774") {
            steps {
                script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat "mvn clean"
                }
            }
        }
        stage("mvn test ") {
            steps {
                script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat "mvn test"
                }
            }
        }
     
        
        
                stage("mail") {
          steps {
          mail bcc: '', body: 'testtttttttttttttttttttt', cc: '', from: '', replyTo: '', subject: 'HELOOO from JENKINS', 
              to: 'ghazouaninada02@gmail.com' 
            
          }
        
        
        
           
         stage("mvn deploy") {
            steps {
                script {
                    // If you are using Windows then you should use "bat" step
                    // Since unit testing is out of the scope we skip them
                    bat "C:\\Program Files\\apache-maven-3.6.1\\bin\\mvn deploy"
                }
            }
        }

        
        }
        
        
       
}


}
