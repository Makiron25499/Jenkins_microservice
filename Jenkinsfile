/*node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
}
*/
pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo "Build"
                //sh "mvn --version"
            }
        }
        stage('Integration Test'){
            steps{
                echo "Integration Test"
            }
        }
		
    }
}