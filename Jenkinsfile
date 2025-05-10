pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue:'USER',description: 'enter your name')
        booleanParam(name: 'RUN_EXTRA_STEP', defaultValue: false, description: 'RUN the extra step?')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello ${params.USERNAME}!"
            }
        }
        stage('Extra Step') {
            when {
                expression {
                    return params.RUN_EXTRA_STEP }
                }
                steps {
                    echo 'This is the extra step running!'
                }
            }
        }
    }
