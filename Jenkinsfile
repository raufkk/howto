node {
  stage ('checkout') {
    echo 'git checkout'
    checkout([$class: 'GitSCM', branches: [[name: '**']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github_raufkk', url: 'https://github.com/raufkk/howto.git']]])
  }
  stage ('build') {
    echo 'build done. proceeding'
  }

  stage ('test') {

    if (env.BRANCH_NAME == 'master') {
    echo 'this is master branch'
    }
    else {
    echo 'this is not master branch'
    }
  }
}
