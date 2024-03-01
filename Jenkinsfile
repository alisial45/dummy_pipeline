pipeline {
    agent any

    stages {      
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: 'origin/one-parameterized']],
                userRemoteConfigs: [
                    [ url: 'https://github.com/alisial45/dummy_pipeline' ]
                ])
                     
            }
        }
    }
    
}

