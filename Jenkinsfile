pipeline{
  agent{label "!built-in"}
  tools{nodejs "Nodejs"}
  stages{
    stage("clone"){
      steps{
        git url: "https://github.com/bvsaikr/Blog-Portal-Frontend.git", branch: "main"
      }
    }
    stage("unittest"){
      steps{
        sh 'echo "unitested"'
      }
    }
    stage("build"){
      steps{
        sh 'docker build -t frontendapp .'
      }
    }
  }
}
