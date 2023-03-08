pipeline {
 agent any
  
  parameters {
     booleanParam(name: 'MyBoolean', defaultValue: true, description: 'Enable service ? ')
  }  
  stages {
    stage ("Demo"){
     steps{
      script {
       if(params.MyBoolean == false){
        currentBuild.result = "SUCCESS"
        return
       }
       else {
        echo "MyBoolean is : ${params.MyBoolean}"
       }
      }
      
     }
    }
  }  
}
