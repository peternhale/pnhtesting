#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}

	if (env.JOB_NAME.toLowerCase().matches('unit')) {
		doUnitTests();
	} else (env.JOB_NAME.toLowerCase().matches('integration')) {
		doIntegrationTests()
	}
}

def doUnitTests() {
	stage('unit tests') {
		echo 'unit tests'
	}
}

def doIntegrationTests() {
	stage('integration tests') {
		echo 'integration tests'
	}
}
