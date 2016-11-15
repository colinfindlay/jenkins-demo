node {
  stage 'Build and Test'
  checkout scm
  sh 'echo RunBuild'


 }

stage 'promotion'
def userInput = input(
 id: 'userInput', message: 'Let\'s promote?', parameters: [
 [$class: 'TextParameterDefinition', defaultValue: 'uat', description: 'Environment', name: 'env']
])
echo ("Env: "+userInput)
