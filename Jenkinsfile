#!groovy
@Library('GlobaLPipeline@master') _
node {
properties([buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '2', numToKeepStr: '2'))])
pipeline {
GIT_URL 		                 = 'https://github.com/pramodvishwa/Tutorial-Pipe.git'
BRANCH                       = 'dev'
GIT_CREDENTIALS 	           = 'Git-Credentials'
MAVEN_HOME                   = '/app/maven-3.5.4'
MAVEN_GOAL 		               = 'clean install'
//SONAR_PROPERTY		         = 'sonar-project.properties'
MAVEN_GOAL                   = 'versions:set -DgroupId=org.apache.maven.* -DartifactId=* -DoldVersion=2.0.* -DnewVersion=2.0.1'
  }
}
