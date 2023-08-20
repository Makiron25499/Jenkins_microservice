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
    /*stages{
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
		
    }*/
    stages{
        stage('Build Docker Image'){
            steps{
                script{
                    docImage=docker.build("makiron/jenkins:${env.BUILD_TAG}")
                    echo "Build Success"
                }
            }
        }
        /*stage('Push Docker Image'){
            steps{
                script{
                    docker.withRegistry('','dockerhub'){
                        docImage.Push('Latest');
                    }
                }
            }
        }*/
    }
}