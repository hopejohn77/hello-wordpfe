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
       sh  '/var/lib/jenkins/workspace/hello-wordpfe/ java -cp target/jltsecurity-1.0-SNAPSHOT.jar com.mycompany.app.App'
        }
       }
    }
   }
