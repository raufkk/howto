node {
  stage ('checkout') {
    echo 'git checkout'
    checkout([$class: 'GitSCM', branches: [[name: '**']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github_raufkk', url: 'https://github.com/raufkk/howto.git']]])
  }
  stage ('build') {
    echo 'build done. proceeding'
  }

  stage ('test') {

    echo 'branch is : env.BRANCH_NAME'
    echo 'git commit is : env.CHANGE_ID'
  }
}
