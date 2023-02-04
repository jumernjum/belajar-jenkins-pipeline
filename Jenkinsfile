pipeline {
   agent any

   stages {
       stage("Build") {
         steps {
           echo("Hello Build")
         }
       }
   
       stage("Test") {
         steps {
           echo("Hello Test")
         }
       }   
      
       stage("Deploy") {
         steps {
           echo("Hello Word")
         }
       }
    }
   
   post {
      always {
         echo "I will always say Hello again!"
      }
      success {
         echo "Yay, success"
      }
      failure {
         echo "Oh no, failure"
      }
      cleanup {
         echo "Don't care sussess or error"
      }
  }
  
}
