pipeline {
    agent any

    parameters {
        string(name: 'USERNAME' defaultValue: 'kashefi')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello ${params.USERNAME}!"
            }
        }
    }
}
