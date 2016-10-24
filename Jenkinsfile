#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}

	if (env.JOB_NAME.toLowerCase().matches(/.*unit.*/)) {
		doUnitTests();
	} else if (env.JOB_NAME.toLowerCase().matches(/.*integration.*/)) {
		doIntegrationTests()
	} else {
		doUnitTests();
	}
}

def doUnitTests() {
	stage('unit tests 1') {
		echo 'unit tests'
	}
	stage('unit tests 2') {
		echo 'unit tests'
	}
}

def doIntegrationTests() {
	stage('integration tests 1') {
		echo 'integration tests'
	}
	stage('integration tests 2') {
		echo 'integration tests'
	}
	stage('integration tests 3') {
		echo 'integration tests'
	}
}
