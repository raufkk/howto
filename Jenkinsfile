node {
  stage ('checkout') {
    echo 'git checkout'
    checkout([$class: 'GitSCM', branches: [[name: '**']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github_raufkk', url: 'https://github.com/raufkk/howto.git']]])
  }
  stage ('build') {
    echo 'build done. proceeding'
  }

  stage ('test') {

    echo 'Testing will be done'
  }
}
