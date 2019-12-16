node{
          stage('dhruv checkout')
          {
          git 'https://github.com/Dhruvsahu9/Jenkins-maven-git-integration'
          }
          stage('Compile-Package')
          {
          def mvnHome= tool name: 'maven3', type: 'maven'
          sh "${mvnHome}/bin/mvn package"
          }
          stage('Email notification')
          {
                    mail bcc: '', body: '''Hi welcome to jenkins email alerts
thanks
hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'awsconsole.cloudcomputing@gmail.com'
          }
}
