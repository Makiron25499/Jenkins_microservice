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
    agent {docker {image 'maven:3.6.3'}}
    stages{
        stage('Build'){
            steps{
                echo "Build"
                sh "mvn --version"
            }
        }
        stage('Integration Test'){
            steps{
                echo "Integration Test"
            }
        }
		
    }
}