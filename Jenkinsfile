pipeline {
         agent any
         stages {
              stage('Checkout') {
                  steps {
                          checkout scm
                        }}
                  stage('Build') {
                     steps {
                            sh '/home/shubm/Documents/devops-tool/apache-maven-3.9.1/bin/mvn install'
                            }}
                  stage('Deployment'){
                     steps {
                     
                         sh 'cp target/hike.war /home/shubm/Documents/devops-tool/apache-tomcat-9.0.73/webapps'
                         }
}}}                         

