pipeline {
    agent any

    parameters {
        string(defaultValue: 'one-parameterized', description: 'This is my dynamic branch', name: 'MY_BRANCH')
    }

    stages {
       
    
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: 'origin/one-parameterized']],
                userRemoteConfigs: [
                    [ url: 'https://github.com/alisial45/dummy_pipeline.git' ]
                ])
                
            }
        }
    }
}
