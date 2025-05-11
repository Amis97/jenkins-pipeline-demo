pipeline {
    agent any
    triggers {
        cron('H H * * *')
    }

    //parameters {
     //   string(name: 'USERNAME', defaultValue:'USER',description: 'enter your name')
      //  booleanParam(name: 'RUN_EXTRA_STEP', defaultValue: false, description: 'RUN the extra step?')
    //}

    stages {
        stage('check day') {
            steps {
                script {
                    def today = new Date().format('EEEE', TimeZone.getTimeZone('Asia/Tehran'))
                    echo "today is: ${today}"
                    if (today == 'Friday') {
                        sh './friday.sh'
                    }
                    else {
                        echo 'Not Friday, skipping special task.'
                    }                  }
            }
        }
    }
}
