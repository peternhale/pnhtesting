properties([
	[$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/peternhale/pnhtesting.git/'],
	parameters([
		string(defaultValue: 'thisIsTheValue', description: '', name: 'VAR_NAME')
	]),
	pipelineTriggers([
		[$class: 'GitHubPRTrigger', events: [], spec: '* * * * *', triggerMode: 'CRON']
	])
])
node {
	checkout scm
	stage('1') {
		sh 'env'
		echo "${env.VAR_NAME}"
	}
}
