node{
          
          stage('compile package')
          {
                    def mav=tool name: 'maven3', type: 'maven'
                    sh "${mav}/bin/mvn package"
          }
          stage('Email notification')
          {
                    mail bcc: '', body: '''Hi welcome to jenkins email alerts
             thanks
hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'awsconsole.cloudcomputing@gmail.com'
          }
          
          stage('slack notification')
          {
             slackSend baseUrl: 'https://hooks.slack.com/services/', channel: '#jenkins-pipeline-demo', color: 'good', tokenCredentialId: 'slack-demo', username: 'awscloudhq'      
          }
}
