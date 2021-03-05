dockerNode('benhall/dind-jenkins-agent:v2') {
  echo "hi"  
}

node {
    checkout scm
   
    docker.withRegistry('https://hub.docker.io', 'credentials-id-tonyennis') {

      docker.image('gustavoapolinario/jenkins-docker').inside {
            sh 'echo hi'
        }
    }
}

