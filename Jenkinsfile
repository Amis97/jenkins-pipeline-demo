pipeline {
    agent any

    parameters {
        string(name: 'sima', defaultValue: 'kashefi', description: 'golpar')
    }

    stages {
        stage('Greet') {
            steps {
                echo "Hello ${params.USERNAME}!"
            }
        }
    }
}
