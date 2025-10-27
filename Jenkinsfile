pipeline{
    agent{
        any agent
         

         stages{
            stage("checkout"){

                git"https://github.com/amrAdel-1/three-tier-project/tree/nodejs-app"
            }
            stage("build dockerfile"){
                                
              sh 'docker build -t nodejs-app'
                            
         }

        stage("run container"){
            sh 'docker run -d -p 3000:3000 --name nodejs nodejs-app'
        }
    }
    }
    }
    
        