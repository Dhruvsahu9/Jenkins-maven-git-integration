node{
          stage('dhruv checkout')
          {
          git 'https://github.com/Dhruvsahu9/Jenkins-maven-git-integration'
          }
          
          stage('Email notification')
          {
                    mail bcc: '', body: '''Hi welcome to jenkins email alerts
thanks
hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'awsconsole.cloudcomputing@gmail.com'
          }
          stage('Slack notification')
          {
                    slackSend baseUrl: 'https://hooks.slack.com/services/', channel: '#jenkins-pipeline-demo', color: 'good', message: 'my-jenkins-pipeline-slack', tokenCredentialId: 'slack-demo', username: 'awscloudhq'
          }
}
