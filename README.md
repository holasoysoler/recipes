# Recipes
Recipe book for infrastructures


## Create secret keys and file with key in it : 
* aws ec2 create-key-pair --key-name MyKeyPair --query 'KeyMaterial' --output text > MyKeyPair.pem

## Run the following command to retrieve the access credentials for your cluster and automatically configure kubectl.
* aws eks --region $(terraform output -raw region) update-kubeconfig --name $(terraform output -raw cluster_name)
