pipeline {
   agent any
   }

   stages {
      stage('Build') {
         steps {
            sh 'mvn clean package'
         }
         stage('Development Tests') {
         when {
            beforeAgent true
            branch 'development'
         }
         steps {
            echo "Run the development tests!"
         }
      }

      }

   }
}
