pipeline
{
agent any
stages
{
	stage ('cloudformation creation')
{
		steps
{
			withAWS(credentials: 'jenkins', region: 'us-east-1') 
{
    sh 'aws cloudformation create-stack --stack-name cloudformation --template-body file://combine.json'
}
}
}	
}
}
