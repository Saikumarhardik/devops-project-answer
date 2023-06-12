pipeline{
  agent {
    label "qwertyy"
  }
    stages{
      stage("buiding the image"){
        steps{
          sh "docker build -t new:1 ."
        }
      }
      stage("running the container"){
        steps{
          sh "docker container run -dt --name c1  -p 8080:8080 new:1"
      }
      }
      
  }
}



