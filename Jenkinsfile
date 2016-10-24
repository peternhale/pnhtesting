#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}
	def unit = ~/testPNH/
	if (unit.matches(env.JOB_NAME.toLowerCase()) {
		echo 'hit'
	} else {
		echo 'no hit'
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
