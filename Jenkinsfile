pipeline {
   agent any

   stages {
       stage("Build") {
         steps {
           echo("Start Build")
            sh("./mvnw clean compile test-compile")
            echo("Finish Build")
         }
       }
   
       stage("Test") {
         steps {
           echo("Start Test")
            sh("./mvnw test")
            echo("Finish Test")
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
