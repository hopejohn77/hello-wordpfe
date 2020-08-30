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
       sh  '/home/maven/bin/mvn deploy'
        }
       }
    }
   }
