pipeline {
    agent any
    stages {
        stage('Build') {
            steps {

                retry(3) {
                    sh 'echo "Hello World"'
                    sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    '''
                    }
                 timeout(time: 3, unit: 'MINUTES') {
                    sh 'free -h'
                }
                
            }
        }
    }
}