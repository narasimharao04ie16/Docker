node{
  stage("image creation and pushing"){
    checkout scm
    docker.withRegistry('https://registry.hub.docker.com','dockerhub'){
      def image = docker.build("narasimharao04ie16/test_repo")
      image.push()
    }
  }
}
