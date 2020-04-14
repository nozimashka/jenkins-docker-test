pipeline {
    agent {
        dockerfile true
        label 'generic'
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