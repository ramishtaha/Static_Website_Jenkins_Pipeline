stages{
      stage('deploy to S3'){
          steps{
              sh 'aws s3 cp public/index.html s3://ramishtaha-jenkins-staticweb'
              sh 'aws s3api put-object-acl --bucket ramishtaha-jenkins-staticweb --key index.html --acl public-read'
              sh 'aws s3 cp public/error.html s3://ramishtaha-jenkins-staticweb'
              sh 'aws s3api put-object-acl --bucket ramishtaha-jenkins-staticweb --key error.html --acl public-read'
          }
      }
  }