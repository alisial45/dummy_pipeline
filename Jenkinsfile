pipeline {
    agent any

    parameters {
        string(defaultValue: 'one-parameterized', description: 'This is my dynamic branch', name: 'MY_BRANCH')
    }

    stages {
       
    
        stage('Checkout') {
            steps {
                echo "Selected branch: ${params.MY_BRANCH}"
                // Use MY_BRANCH parameter value for dynamic branch checkout
                checkout([$class: 'GitSCM', branches: [[name: "$MY_BRANCH"]], userRemoteConfigs: [[url: 'https://github.com/alisial45/dummy_pipeline']]])
            }
        }
    }
}
