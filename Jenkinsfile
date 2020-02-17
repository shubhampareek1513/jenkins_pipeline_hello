pipeline
{
agent any
stages
{

stage('scm checkout')
{
steps{

git branch: 'master', url: 'https://github.com/shubhampareek1513/jenkins_pipeline_hello.git'

}
}
stage ('validate code')
{
steps
{
withMaven(jdk: 'localjdk', maven: 'local-mvn'){
sh 'mvn validate'
}
}
}
}
