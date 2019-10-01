To access your instance:
Open an SSH client. (find out how to connect using PuTTY)
Locate your private key file (blockdevs_ec2_proximax_keypair.pem). The wizard automatically detects the key you used to launch the instance.
Your key must not be publicly viewable for SSH to work. Use this command if needed:
chmod 400 blockdevs_ec2_proximax_keypair.pem
Connect to your instance using its Public DNS:
ec2-3-1-80-38.ap-southeast-1.compute.amazonaws.com
Example:
ssh -i "blockdevs_ec2_proximax_keypair.pem" ubuntu@ec2-3-1-80-38.ap-southeast-1.compute.amazonaws.com
Please note that in most cases the username above will be correct, however please ensure that you read your AMI usage instructions to ensure that the AMI owner has not changed the default AMI username.

Setup Proximax:
https://github.com/proximax-storage/vagrant-testnet-sirius-peernode