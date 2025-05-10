pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue:'kashefi', description: 'Enter your name')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello ${params.USERNAME}!"
            }
        }
    }
}
