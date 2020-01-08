node{
          stage('dhruv checkout')
          {
          git 'https://github.com/Dhruvsahu9/Jenkins-maven-git-integration'
          }
          stage('compile package')
          {
                    def mav=tool name: 'maven3', type: 'maven'
                    sh "${mav}/bin/mvn package"
          }
     
}
