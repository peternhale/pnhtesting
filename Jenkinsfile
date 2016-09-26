#!groovy
node {

	stage('checkout source') {
		// when running in multi-branch job, one must issue this command
		checkout scm
		echo env.BRANCH_NAME
	}

withCredentials([[$class: 'FileBinding', credentialsId: 'jwt_key', variable: 'JWT_KEY']]) {
	'sh env'
	echo "${env.JWT_KEY}"
	if (env.BRANCH_NAME == 'master') {
		stage('m1') {}
		stage('m2') {}
	} else {
		stage('o1') {}
		stage('o2') {}
		stage('o3') {}
	}
}
}
