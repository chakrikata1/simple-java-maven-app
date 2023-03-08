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
   stage ("Functions"){
    steps {
      myFunc("Hello from the functions stage!")
    }
   }
  }  
}

def myFunc(String myText){
 echo "myText is set to: ${myText}"
}
