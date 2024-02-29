pipeline {
    agent any

    parameters {
        string(defaultValue: '', description: 'This is my dynamic branch', name: 'MY_BRANCH')
    }

    stages {
        stage('checkout') {
            steps {
                echo env.GIT_BRANCH
                
            }
        }
    }
}
