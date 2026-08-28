pipeline {
    agent any

    environment {
        PROJECT = "Linux Backporting"
        AUTHOR = "Shilpa"
    }

    stages {

        stage('Environment Variables') {
            steps {
                echo "Project Name: ${PROJECT}"
                echo "Author Name: ${AUTHOR}"

                sh 'echo "Workspace Path: $WORKSPACE"'
                sh 'echo "Build Number: $BUILD_NUMBER"'
                sh 'echo "Job Name: $JOB_NAME"'
            }
        }

    }
}
