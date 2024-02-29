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
                    params.MY_BRANCH = env.GIT_BRANCH
                }
            }
        }
        
        stage('checkout') {
            steps {
                echo env.GIT_BRANCH
                
            }
        }
    }
}
