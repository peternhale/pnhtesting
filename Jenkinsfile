#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}
	java.util.regex.Matcher myMatcher = env.JOB_NAME.toLowerCase() =~ /.*testpnh.*/
	if (env.JOB_NAME.toLowerCase().matches(/.*testpnh.*/)) {
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
