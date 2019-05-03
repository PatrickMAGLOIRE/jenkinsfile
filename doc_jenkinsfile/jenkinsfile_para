pipeline {
    agent any
    stages {
        stage('Run Tests') {
            parallel {
                stage("stage parallel 1") {
                    
                    
                    steps {
                        echo "etape parallel 1"
                    }
                    
                }
                stage("stage parallel 2") {
                    
                    
                    steps {
                        echo "etape parallel 2"
                    }
                   
                }
            }
        }
    }
}
