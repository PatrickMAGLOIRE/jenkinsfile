pipeline {
agent any
stages {
    stage("mon stage non sequentiel") {
        
        steps {
            git branch: 'sequentiel', credentialsId: '02342744-7118-42a1-84ab-a79c42bea0f5', url: 'https://github.com/PatrickMAGLOIRE/jenkinsfile.git'
            echo "stage non sequentiel"
        }
    }
    stage("mon stage sequentiel") {
             
        stages {
           stage("stage sequentienl 1") {
               steps {
                   echo "mon premier stage séquentiel"
               }
           }
           stage("stage séquentiel 2") {
               steps {
                   echo "mon deuxieme stage sequetiel"
               }
            }
                
           stage("stage séquentiel 3") {
               steps {
                   echo "mon troisieme stage sequetiel"
               }   
           }
        }
    }
}


