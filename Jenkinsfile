pipeline{
agent any
  parameters {
    choice(name: 'VERSION', choices: ['1.1.0','1.2.0','1.3.0'],description:'')
    booleanParam(name: 'executeTests', defaultValue:true, description:'')
  }
  environment {
    NEW_VERSION = '1.3.0'
  }
stages {
stage("build"){
steps{
echo "building the app"
  echo "build done"
}
}

stage("test"){
  when {
    expression {
      params.executeTests
    }
  }
steps{
echo "testing the app"
  echo "new version ${NEW_VERSION}"
}
}

stage("deploy"){
steps{
echo "deploying the app"
}
}
}
}
