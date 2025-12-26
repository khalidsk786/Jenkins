pipeline {
  agent  {
    node {
    label 'Agent-1'
    }
  }
    stages {
       
       stage ('build')
       {
         steps {

            echo "this is building"
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



}