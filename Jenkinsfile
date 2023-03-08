pipeline {
 agent any
  
  parameters {
     booleanParam(name: 'MyBoolean', defaultValue: true, description: 'Enable service ? ')
  }  
  stages {
    stage ("Demo"){
      echo "MyBoolean is : ${params.MyBoolean}"
    }
  }  
}
