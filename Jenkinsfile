pipeline {
     agent any
     stages {
          stage ("git clone") {
              steps {
                  git branch: 'main', url: 'https://github.com/menganiravivarma/menganiravivarma4922.git'
              }
          }
          stage ("test") {
               steps {
                    echo 'testing the application'
               }
          }
          stage ("deploy") {
               steps {
                   echo 'deploying the application'
               }
          }
      }
      post {
          always {
               mail to: "menganiravivarma4922@gmail.com",
               subject: "check the status",
               body:    "CHECK"
           }
      }
}
