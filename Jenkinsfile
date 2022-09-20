//

// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// }

// 2)SCRIPTED PIPELINE

// node {
// 	echo "Build"
// 	echo "Test"
// 	echo " Dev"
	
// }


// 3) DECLARATIVE PIPELINE

pipeline {
	agent any
	stages {
		stage("Build") {
			steps {
				echo "Build"
			}
		}
		
		stage {
			steps("Test") {
				echo "Test"
			}

		}
	}
	post {
		always {
			echo "I am awesome"
		}
		success {
			echo "I run when successful"
		}
		failure {
			echo "I run when fail"
		}
	}
}


