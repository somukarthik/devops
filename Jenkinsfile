properties([parameters([string(name: 'Country', defaultValue: 'India', description: 'Enter the Country Name'), 
            string(name: 'State', defaultValue: 'Karnataka', description: 'enter state name')])])

pipeline {
    agent any

    stages {
	
		stage('GitCheckout'){
			steps{
			  echo "This stage is for GitCheckout"
			}
		}
        stage('Build'){
			steps{
			  echo "This is build stage"
			}
		}
		stage('Sonar'){
			steps{
			  echo "This is static code analysis stage"
			}
		}

		stage('Nexus'){
			steps{
			  echo "This is for uploading artifacts into Nexus stage"
			}
		}
		
		stage('Deployment'){
			steps{
			  echo "This is Deployment stage"
			}
		}       
    }

}
