pipeline {
    agent any 
     stages {
        stage('Non-Sequential Stage') {
            steps {
                echo "On Non-Sequential Stage"
            }
        }
        stage('Sequential') {
            stages {
                stage('Hello1') {
                    steps {
                        echo "Hello1"
                    }
                }
                stage('Hello2') {
                    steps {
                        echo "Hello2"
                    }
                }

            }
        }
    }
}
