
## Step after you clone the repo

1. Create a feature branch call feature/first_setup
2. Rename JenkinsTemplate to Jenkinsfile and remove the first line
3. Update the pyproject.toml
4. Update README.md
5. Make sure src folder is source root and tests in test root in Pycharm
6. Rename the project_template under src folder
7. Update ChangeLOG
8. Commit and create PR to review.

## Get the Python Package from local nexus

pip3 install --no-cache-dir \
    --extra-index-url https://<username>:<password>@saturn:30088/cicd/nexus/repository/saturn-python-hosted/simple \
    --trusted-host saturn \
    -r requirements.txt
