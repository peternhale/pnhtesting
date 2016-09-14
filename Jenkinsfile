#!groovy
node {

	stage('checkout source') {
		// when running in multi-branch job, one must issue this command
		checkout scm
	}

	stage('env') {
		sh 'env'
	}

	stage('look around') {
		sh 'find .'
	}
}
