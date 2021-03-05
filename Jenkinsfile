dockerNode('benhall/dind-jenkins-agent:v2') {
  echo "hi"  
}

node {
    checkout scm
   
    //docker { image 'node:14-alpine' }
    agent any  

    docker.withRegistry('', 'credentials-id-tonyennis') {

      docker.image('gustavoapolinario/jenkins-docker').inside {
            
        }
    }
}

