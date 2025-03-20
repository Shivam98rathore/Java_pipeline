
pipeline{
  agent any
  stages{
    stage("Compile"){
      steps{
        bat 'javac Test.java'
      }

    }
    stage("run java program"){
      steps{
        bat  'java Test'
      }
    }
  }
}

