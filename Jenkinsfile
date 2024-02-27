pipeline {
    agent any
  
    triggers{
        githubPush()
            }

    
    stages {
        stage('Hello') {
            steps {
            
                echo 'Branch one'
            }
        }
    }
}
