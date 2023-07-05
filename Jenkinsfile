// nodejs

pipeline{
    agent {
        label 'ws'
    }
    stages{                                              //start of the stages
        stage("Lint checks"){
          steps{
            sh "echo Installing JSLint"
            sh "npm i jslint"
            sh "ls -ltr node_modules/jslint/bin/"
            sh "node_modules/jslint/bin/jslint.js server.js || true"
          }  
            
        }
        stage("Code Compile"){
          steps{
            sh "npm install"
            }  
            
        }
    }
   
}