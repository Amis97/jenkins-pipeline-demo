pipeline {
    agent any
    stages {
        stage('say Hello') {
            steps {
                echo 'Hello, jenkins!'
            }
        }
        stage('wait for input') {
            steps {
                input message: 'ادامه بدیم؟'
            }
        }
        stage('continu'){
            steps {
                echo 'مرحله بعدی اجرا شد'
            }
        }
    }
}
