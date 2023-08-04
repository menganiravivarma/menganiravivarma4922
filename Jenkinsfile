pipeline {
     agent any
     stages {
          stage ("build") {
              steps {
                  echo 'building the application'
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
