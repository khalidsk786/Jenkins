pipeline {
  agent  {
    node {
    label 'Agent-1'
    }
   }
    environment{
    COURSE = "jenkins"
  }
    stages {
       stage ('build')
       {
         steps {
           script {
              sh """
                  echo "this is building"
                  echo $COURSE
              """
      
           }
         }
      }

       
       stage ('test')
       {
            
         steps {

            echo "this is testing"
         }
        
       }
       
       stage ('deploy')
       { 
         steps{

            echo "this is deploy"
         }
          
        
       }

     }

   post{

      always{

        echo "always run whether it is susccess or filure"
      }

      success{

          echo "i will run if pipeline success"
      }
      
      failure{
         
         echo "i will run if it pipeline failure"

       }
    }

}