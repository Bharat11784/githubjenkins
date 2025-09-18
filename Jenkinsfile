pipeline{

agent any
tools{
maven 'maven'
jdk 'java-11'

}

stages{
stage('git-checkout'){
steps{
 git branch: 'version1', url: 'https://github.com/Bharat11784/githubjenkins.git'
}
}
stage('compile'){
steps{
sh "mvn compile"
}
}
stage('build'){
steps{
sh "mvn package"
}
}
}
}
