pipeline {
    agent any
    parameters {
    booleanParam(name 'runTests', defaultValue: true, description: " do you want to run tests?")
    choice(name: 'OPTION', choices: ['option 1 (default)', 'option 2', 'option 3'], description: "testing choices")
    }  
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
