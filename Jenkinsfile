pipeline {
    agent any 
    
    environment {
           
            PATH="/home/ec2-user/opt/apache-maven-3.6.1/bin:$PATH"
            
   }    
    stages {
        stage('Git Clone') { 
            steps {
                git credentialsId: '9623d212-3904-452e-8b8a-673356f55a90', url: 'https://github.com/sachin193959/simple-java-maven-app.git'
                
                 }
            }
            
            stage('Maven Build') { 
            steps {
                  sh "mvn clean package"
              }
           }
           
       }
       
  }   
