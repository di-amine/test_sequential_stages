pipeline {
    agent any 
    options {
        parallelsAlwaysFailFast()
    }
    stages {
        stage('Parallel') {
            parallel {
                stage('Parallel1') {
                    when {
                        branch 'master'
                    }
                    failFast true
                    steps {
                        echo "Parallel 1"
                    }
                }
                stage('Parallel2') {
                    when {
                        branch 'dev'
                    }
                    steps {
                        echo "Parallel 2"
                    }
                }
            }
        }
    }
}
