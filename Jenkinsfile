// 1) #################################################################################################

// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// }

// 2) SCRIPTED PIPELINE ################################################################################

// node {
// 	echo "Build"
// 	echo "Test"
// 	echo " Dev"
	
// }


// 3) DECLARATIVE PIPELINE   #############################################################################

// pipeline {
// 	agent any
// 	stages {
// 		stage("Build") {
// 			steps {
// 				echo "Build"
// 			}
// 		}
		
// 		stage("Test") {
// 			steps {
// 				echo "Test"
// 			}

// 		}
// 	}
// 	post {
// 		always {
// 			echo "I am awesome"
// 		}
// 		success {
// 			echo "I run when successful"
// 		}
// 		failure {
// 			echo "I run when fail"
// 		}
// 	}
// }

// 4) Build Run on Container (Docker Image) ############################################################

//  pipeline {
// 	//agent any
// 	agent { docker { image 'maven:3.8.6'} }
// 	stages {
// 		stage("Build") {
// 			steps {
// 				echo "Build"
// 				sh 'mvn --version'
// 			}
// 		}
		
// 		stage("Test") {
// 			steps {
// 				echo "Test"
// 			}

// 		}
// 	}
//  }

// 5) Pipeline Variable  #####################################################################################################################

pipeline {
	agent any
	stages {
		stage("Build") {
			steps {
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"

			}
		}
		
		stage("Test") {
			steps {
				echo "Test"
			}

		}
	}
}



// 6)   #####################################################################################################################
