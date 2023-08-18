empty:
	@echo ""


delete-staging:
	aws cloudformation delete-stack --stack-name staging-conditionals 
deploy-staging:
	aws cloudformation deploy --stack-name staging-conditionals --template-file stack-conditionals.yaml --parameter-overrides KeyPairParameter=keypair-pruebas-cf2 VpcIdParameter=vpc-0d566183548ec1274 AmiIdParameter=ami-08a52ddb321b32a8c Environment=staging



delete-prod:
	aws cloudformation delete-stack --stack-name prod-conditionals 
deploy-prod:
	aws cloudformation deploy --stack-name prod-conditionals --template-file stack-conditionals.yaml --parameter-overrides KeyPairParameter=keypair-pruebas-cf2 VpcIdParameter=vpc-0d566183548ec1274 AmiIdParameter=ami-08a52ddb321b32a8c Environment=prod