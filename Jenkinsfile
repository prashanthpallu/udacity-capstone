pipeline{
  agent any
  stages{
    stage("Lint HTML"){
      steps{
        sh 'tidy -q -e *.html'
      }
    }
    stage("Build docker image"){
      steps {
        sh 'echo "Upoading to AWS Bucket"'
        }
    }
    stage("Push image"){
	steps {
	  sh 'echo "Push image to registry"'
	}
    }
    stage("Set current kubectl context"){                                                                                                                                           steps {                                                                                                                                                                       sh 'echo "Set current kubectl context"'                                                                                                                                   }
    }
    stage("Deploy container"){                                                                                                                                                        steps {                                                                                                                                                                       sh 'echo "Deploy Conatiner"'                                                                                                                                            }
    }
 }
}
