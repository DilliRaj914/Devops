pipeline{
    tools{
       
        maven 'mymaven'
    }
	agent any
      stages{
           stage('Checkout'){
	    
               steps{
		 echo 'cloning'
                 git 'https://github.com/DilliRaj914/Devops-Practice.git'
              }
          }
          stage('Compile'){
             
              steps{
                  echo 'complie the code..'
                  sh 'mvn compile'
	      }
          }
          stage('CodeReview'){
		  
              steps{
		    
		  echo 'codeReview'
                  sh 'mvn src:App.js'
              }
          }
          
        
          stage('Package'){
		  
              steps{
		  
                  sh 'mvn package'
              }
          }
	     
          
      }
}