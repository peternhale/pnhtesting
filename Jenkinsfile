#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}
	Matcher myMatcher = "env.JOB_NAME.toLowerCase()" =~ /testPNH/
	if (myMatcher.matches()) {
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
