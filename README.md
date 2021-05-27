# Recipes
Recipe book for infrastructures


# Create secret keys and file with key in it : 
aws ec2 create-key-pair --key-name MyKeyPair --query 'KeyMaterial' --output text > MyKeyPair.pem
