pipeline {
      agent any
      stages {
      stage ('compile stage') {
       
      steps {    
          withMaven(maven : '/usr/share/maven') {
             sh 'clean compile'
              }
           }
       }
     stage ('Testing stage') {
       
       steps {
          withMaven(maven : '/usr/share/maven') {
           sh 'mvn test'
            }
         }
    }
      
  }
}
