pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            echo "$GIT_BRANCH"
            powershell(script: 'pwd')
            powershell(script: 'echo $pwd')
         }
      }
   
      stage('Docker Build') {
         steps {
            pwsh(script: 'docker images  ls')
           
         }
      }
   }
}
