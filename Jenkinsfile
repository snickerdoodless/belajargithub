pipeline {
    agent: any

    stages {
        stage ("Test Triggers") {
            steps {
                echo "Triggers Success"
            }

            post {
                success {
                    echo "Exit 0"
                }

                failure {
                    echo "Exit 1"
                }
            }
        }
    }
}