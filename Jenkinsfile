pipeline {
    agent {
        dockerfile {
            label 'generic'
        }

    }      
    stages {
        stage("Run Hello World!") {
            steps {
                sh """
                    python helloworld.py
                    """
            } //steps
        }
        stage("Test requests") {
            steps {
                sh """
                python requestgoogle.py
                """
            }
        }
    }
}