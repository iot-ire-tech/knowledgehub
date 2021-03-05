dockerNode('benhall/dind-jenkins-agent:v2') {
  echo "hi"  
}

node {
    checkout scm
   
    docker.withRegistry('', 'credentials-id-tonyennis') {

      docker.image('gustavoapolinario/jenkins-docker').inside {
            
        }
    }
}

