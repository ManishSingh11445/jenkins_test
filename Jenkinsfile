pipeline{
agent any
stages {
stage("run frontend"){
steps{
echo "executing yarn"
nodejs('Node-19.7')
{
sh 'yarn install'
}
}
}


}
}
