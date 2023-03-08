pipeline {
 agent any
  
  parameters {
     booleanParam(name: 'MyBoolean', defaultValue: true, description: 'Enable service ? ')
  }  
  stages {
    stage ("Demo"){
     steps{
      echo "MyBoolean is : ${params.MyBoolean}"
     }
    }
  }  
}
