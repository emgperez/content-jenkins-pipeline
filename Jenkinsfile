pipeline {
  
  agent any

  stages {

    stage('build') {
      
      steps {
        sh 'javac -c .src/*.java'
        sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'

      }
    }
  }
}
