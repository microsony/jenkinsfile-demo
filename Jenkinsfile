pipeline {

    agent { label 'Slave1' }
    environment {
    SERVER_CREDS = credentials('hello-world')
    }
   stages {
    
      stage ("build") {
          
          steps {
              echo "Building the application..."
          }
          }
          
      stage ("test") {
          
          steps {
              echo "testing the application..."
          }
      }
     
      stage ("deploy") {
          
          steps {
              echo "deplolying the application..."
              echo "Deploying with ${SERVER_CREDS}"
          }
      }
    }
 }
