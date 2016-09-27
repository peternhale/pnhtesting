properties([parameters([string(defaultValue: 'hi', description: '', name: 'helloworld')]), pipelineTriggers([])])
node {
checkout scm
    stage('1') {
    'sh env'
    echo "${env.helloworld}"
    }
}
