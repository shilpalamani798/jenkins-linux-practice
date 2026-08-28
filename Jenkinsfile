pipeline {
    agent any

    parameters {
        string(
            name: 'USERNAME',
            defaultValue: 'Shilpa',
            description: 'Enter your name'
        )

        choice(
            name: 'BUILD_MODE',
            choices: ['Debug', 'Release'],
            description: 'Choose build mode'
        )

        booleanParam(
            name: 'RUN_TESTS',
            defaultValue: true,
            description: 'Run test stage?'
        )
    }

    stages {

        stage('Print Parameters') {
            steps {
                echo "Hello ${params.USERNAME}"
                echo "Build Mode: ${params.BUILD_MODE}"
                echo "Run Tests: ${params.RUN_TESTS}"
            }
        }

    }
}
