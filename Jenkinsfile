pipeline{
agent any
tools{
maven 'Maven'
}
stages{
stage('Checkout')
{
steps{
git branch:'master', url:'https://github.com/Shweta311204/MavenWeb2.git'
}}
stage('Build')
{
steps{
sh 'mvn clean package'
}}
stage('Test')
{
steps
{
sh 'mvn test'
}}
stage('Run Application')
{steps{
sh 'cp target/MavenWeb2.war /opt/tomcat/webapps'}
}}}
