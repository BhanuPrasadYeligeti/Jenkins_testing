pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                checkout([$class: 'GitSCM',
                    branches: [[name: '*/main']],
                    doGenerateSubmoduleConfigurations: false,
                    extensions: [],
                    userRemoteConfigs: [[
                        credentialsId: 'fdae8480-b6fa-4a32-b1fe-00a0747183ac',
                        url: 'https://github.com/BhanuPrasadYeligeti/Jenkins_testing.git'
                    ]]
                ])
            }
        }

        stage('Hello') {
            steps {
                echo 'Hello World Bhanu'
            }
        }
    }
}
