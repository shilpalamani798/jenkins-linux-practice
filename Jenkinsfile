pipeline {
    agent any

    stages {

        stage('Checkout Information') {
            steps {
                echo 'Pipeline started successfully!'
                sh 'pwd'
                sh 'whoami'
            }
        }

        stage('Compile C Program') {
            steps {
                sh 'gcc hello.c -o hello'
            }
        }

        stage('Run C Program') {
            steps {
                sh './hello'
            }
        }

    }
}
