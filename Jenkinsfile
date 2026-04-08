pipeline {
    agent any

    stages {

       stage('build') {
          steps {
            sh 'mvn package' 
          }
       }
    }

        stage('Run') {
            steps {
                sh 'mvn exec:java -Dexec.mainClass="hello.HelloWorld"'
            }
        }

    }
}
