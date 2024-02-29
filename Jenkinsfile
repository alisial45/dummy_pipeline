pipeline {
    agent any

    parameters {
        string(defaultValue: '', description: 'This is my dynamic branch', name: 'MY_BRANCH')
    }

    stages {
        stage('Set Default Branch') {
            steps {
                script {
                    // Set the default value of MY_BRANCH to the value of GIT_BRANCH environment variable
                    params.MY_BRANCH = env.GIT_BRANCH ?: ''
                }
            }
        }

        stage('Checkout') {
            steps {
                echo "Selected branch: ${params.MY_BRANCH}"
                // Use MY_BRANCH parameter value for dynamic branch checkout
                checkout([$class: 'GitSCM', branches: [[name: "$MY_BRANCH"]], userRemoteConfigs: [[url: 'https://github.com/alisial45/dummy_pipeline.git']]])
            }
        }
    }
}
