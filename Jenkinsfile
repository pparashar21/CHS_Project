node{

    stage('Build')
    {
        git credentialsId: 'chs-project-id', url: 'https://github.com/pparashar21/CHS_Project.git'
    }
    
    stage('Run')
    {
        sh 'sudo docker-compose build'
        sh 'sudo docker-compose up -d'
    }
  stage('PUSH image to Docker Hub')
             
             sh 'sudo docker login -u "pparashar21" -p "123soon21" docker.io'
             //sh 'sudo docker push upasanatestdocker/mysql'
             //sh 'sudo docker push upasanatestdocker/job1_web1.0'
             sh 'sudo docker push chs_project'
            // sh 'docker push upasanatestdocker/mysql'
          
    }
}
