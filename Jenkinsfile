pipeline {
    agent any
    stages {
        stage('Run Tests') {
            parallel {
                stage("stage parallel 1") {
                    
                    
                    steps {

                        git branch: 'develop', credentialsId: '02342744-7118-42a1-84ab-a79c42bea0f5', url: 'https://github.com/PatrickMAGLOIRE/jenkinsfile.git'

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
