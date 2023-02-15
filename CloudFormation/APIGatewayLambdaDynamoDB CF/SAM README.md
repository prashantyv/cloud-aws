# Build and Deploy Application using SAM 

#Step 1 - Only needed first time
sam init

#Step 2 - Build your application
cd <inside-folder-with-template.yaml>
sam build

#Step 3 - Deploy your application
sam deploy --guided
