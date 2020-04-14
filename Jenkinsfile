pipeline {
    agent {
        docker {
            image 'centos'
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
    }
}