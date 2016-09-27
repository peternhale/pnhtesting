properties([parameters([string(defaultValue: 'hi', description: '', name: 'helloworld')]), pipelineTriggers([])])
node {
checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github_pat', url: 'https://github.com/peternhale/pnhtesting.git']]])
    stage('1') {
    'sh env'
    echo "${env.helloworld}"
    }
}