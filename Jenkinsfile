node {
	checkout scm
	properties([[$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/peternhale/pnhtesting.git/'], [$class: 'EnvInjectJobProperty', info: [loadFilesFromMaster: false, propertiesContent: 'A="B"', propertiesFilePath: 'jenkins/a.properties'], keepBuildVariables: true, keepJenkinsSystemVariables: true, on: true], pipelineTriggers([])])
	stage('1') {
		sh 'env'
		echo "${env.VAR_NAME}"
	}
}
