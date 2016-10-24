#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}

	if (env.JOB_NAME.toLowerCase().matches('unit')) {
	stage('unit tests') {
		echo 'unit tests'
	}
	} else (env.JOB_NAME.toLowerCase().matches('integration')) {
	stage('integration tests') {
		echo 'integration tests'
	}
	}
}
