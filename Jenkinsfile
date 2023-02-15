pipeline{
  agent any
  stages{
    stage('Cloning'){
      steps{
        git branch: 'main', url: 'https://github.com/Prajot8/Jenkins_docker.git'
        sh 'pwd'
      }
    }
    stage('Build'){
      steps{
        sh'''docker build -t html-img-1 .
        docker images'''
      }
    }
    stage('Run image'){
      steps{
        sh'''docker-compose up -d
        docker ps -a'''
      }
    }
    }

}
