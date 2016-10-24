#!groovy
node {
	stage('checkout source') {
		checkout scm
		sh 'env'
	}

	configFileProvider([configFile(fileId: '4f4a2a99-5a51-4856-ae63-b8181f49f45d', variable: 'matchers')]) {
		if (matchers.strMatches(env.JOB_NAME, 'unit')) {
			doUnitTests();
		} else (matchers.strMatches(env.JOB_NAME, 'integration')) {
			doIntegrationTests()
		}
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
