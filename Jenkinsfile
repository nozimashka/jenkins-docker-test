pipeline {
    agent {
        dockerfile true

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
                pyton requestgoogle.py
                """
            }
        }
    }
}