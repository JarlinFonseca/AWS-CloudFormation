empty:
	@echo ""


delete-staging:
	aws cloudformation delete-stack --stack-name staging-user-data 
deploy-staging:
	aws cloudformation deploy --stack-name staging-user-data --template-file stack-user-data.yaml --parameter-overrides KeyPairParameter=keypair-pruebas-cf2 VpcIdParameter=vpc-0d566183548ec1274 AmiIdParameter=ami-053b0d53c279acc90 Environment=staging



delete-prod:
	aws cloudformation delete-stack --stack-name prod-user-data 
deploy-prod:
	aws cloudformation deploy --stack-name prod-user-data --template-file stack-user-data.yaml --parameter-overrides KeyPairParameter=keypair-pruebas-cf2 VpcIdParameter=vpc-0d566183548ec1274 AmiIdParameter=ami-053b0d53c279acc90 Environment=prod