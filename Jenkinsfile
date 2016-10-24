#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}
	def m = "foobar" =~ /quux/
	if (m.getCount()) {
    // example won't get here as "quux" doesn't exist in "foobar", the count is 0
        echo m[0]
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
