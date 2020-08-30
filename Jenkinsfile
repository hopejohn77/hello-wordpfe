pipeline{
  agent any
    stages{
      stage('build'){
        steps{
        sh '/home/maven/bin/mvn clean install'
        }
       }
      stage('test'){
        steps{
       sh '/home/maven/bin/mvn test'
        }
       }
     stage('delivery'){
        steps{
       sh '/home/maven/bin/mvn validate'
        }
       }
     stage('deploy'){
        steps{
       echo "hello world! about plateforme jlt security"
        }
       }
    }
   }
