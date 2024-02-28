pipeline {
    agent any

    parameters {
        string(name: 'GIT_BRANCH', defaultValue: 'master', description: 'Name of the branch to build')
    }
    
    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = params.GIT_BRANCH
                    echo "Building branch: ${branchName}"
                    // Add steps to build the specified branch
                    checkout([$class: 'GitSCM', 
                              branches: [[name: "${branchName}"]], 
                              userRemoteConfigs: [[url: 'https://github.com/alisial45/dummy_pipeline.git']], 
                              extensions: [[$class: 'CloneOption', depth: 1]], 
                              doGenerateSubmoduleConfigurations: false, 
                              submoduleCfg: [], 
                              browser: [$class: 'GitHubWeb', repoUrl: 'https://github.com/alisial45/dummy_pipeline.git', version: ''],
                              extensions: [[$class: 'RefSpecs', values: [[value: "refs/heads/${branchName}"]]]]])
                }
            }
        }
    }
}
