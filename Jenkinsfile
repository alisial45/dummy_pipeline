pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: "${env.GIT_BRANCH}"]], userRemoteConfigs: [[url: 'https://github.com/alisial45/dummy_pipeline.git']]])
            }
        }
    }
}

