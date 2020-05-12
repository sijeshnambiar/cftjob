pipeline
{
agent any
stages
{
	stage ('cloudformation creation')
{
		steps
{
			withAWS(region: 'us-east-1a') 
{
    sh 'aws cloudformation create-stack --stack-name cloudformation --template-body file://instance.json'
}
}
}	
}
}
