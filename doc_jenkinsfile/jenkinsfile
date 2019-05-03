pipeline { 
    agent none
    
    environment{
        MAGLOIRE = "c'est mon nom"
        PATRICK= "c'est mon prenom"
    }
    
    options{
        timeout(time: 5, unit: 'SECONDS') 
    }
    
        stages {
            
            stage("checkout"){ 
            steps{
                retry(3) {
                echo "coucou c'est mon premier stage"
                echo "$PATRICK"
                
                }
            }
        }
            
            stage ("test"){
            steps{
            
           echo "mon stage 2"
     
                }
     
            }
        
        
        stage ("deploy"){
        steps{
            
            echo "wwaaaazzzzzzzaaaaaaaa  !!!!!!!"
            echo "$MAGLOIRE"
                }
     
            }
        }
        post{
            success{
                echo "aaazzzziiiiii tout roule bro"
            }
                failure{
                echo "ça marche pas oulalou"
            }
        }

}    
