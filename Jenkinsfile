pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Hello World build'
            }
        }
        stage('test') {
            steps {
                echo 'Hello World test'
            }
        }
        stage('deploy') {
            steps {
                echo 'Hello World deploy'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'I will say hello if I succeed!'
        }
        failure { 
            echo 'I will say hello if things do not go well'
        }
    }
}
