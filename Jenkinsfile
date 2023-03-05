pipeline{
agent any
stages {
stage("run frontend"){
steps{
echo "executing yarn"
nodejs('Node-1.5.1')
{
sh 'yarn install'
}
}
}

stage("run backend"){
steps{
echo "executing gradle"
sh './gradlew -v'
}
}

}
}
