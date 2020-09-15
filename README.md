# SSH Deploy for GitHub Actions
Example script on how to archieve:
* Automatic deployment to stage environment on every push to master
* Manual input deployment to production
* Keys in GitHub Secrets

## Configuration
The following configuration should be placed in secrets. They are hopefully self explainatory. 
The keys should be added as deployment keys to the repo and on initial checkout
secrets.STAGE_SSH_PRIVATE_KEY = Used for both connecting and git pull the repo.
secrets.STAGE_SSH_HOST 
secrets.STAGE_SSH_PORT
secrets.STAGE_SSH_USER
secrets.STAGE_REPO_PATH = Remote path to run git pull
secrets.PROD_SSH_PRIVATE_KEY  = Used for both connecting and git pull the repo.
secrets.PROD_SSH_HOST
secrets.PROD_SSH_PORT
secrets.PROD_SSH_USER
secrets.PROD_REPO_PATH = Remote path to run git pull
