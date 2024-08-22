pipeline {
	agent any
	
	stages {
		stage('Checkout') {
		   steps {			
			 checkout scm
		    }	
		}
		stage('Build') {
		    when { branch 'dev' }
      		    steps {
            		echo "this is dev"
      		    }  		
		}
		stage('Deploy') {
		   when { branch 'prod' }
        	   steps {
         		echo "this is prd ready to deploy"
      		   }    
		}
	}
}
