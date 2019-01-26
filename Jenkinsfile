pipeline{
    agent any
    stages{
       stage (Integration){
          steps {
            echo "getting the code from github" 
          }       
       }       
       stage (Building){
           steps {
              echo "Building the code"
           } 
       }
       stage (testing) {
          steps {
             echo "Testing the code"
          }
       }
       stage (QA) {
          steps {
              echo "Code quality with Sonarcube"
          }
       }
       stage (Deploying){
       input (UAT) {
       message "press OK to continue"
       }

          steps {
          
            echo "Deploying into Tomcat"
       }
       
          }             
    }

}
