pipeline{
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Aman'
			
                }
        }
	    stage('Two'){
		    
		steps {
			echo "Let's build the pipeline"
        }
	    }
        stage('Three') {
            parallel{
                stage("Unit Test")
                {
                    steps{
                        echo "Running the unit test"
                    }
                }
                stage("Integration test")
                steps {
			     echo "Running the integration test"
                        }
        }
        }
       stage('Four'){
        steps{
            echo "Thanks!"
        }
       } 
      
}
}