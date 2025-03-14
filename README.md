# aws
AWS Certified Solutions Architect - Associate

# List the start up tasks. Learn more: https://www.gitpod.io/docs/configure/workspaces/tasks
tasks:
  - name: aws-cli
    before:
      cd /workspace
      curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
      unzip awscliv2.zip
      sudo ./aws/install
      cd $THEIA_WORKSPACE_ROOT

      export AWS_ACCESS_KEY_ID=
      export AWS_SECRET_ACCESS_KEY=
      export AWS_DEFAULT_REGION=us-east-1

      gp env AWS_ACCESS_KEY_ID=
      gp env AWS_SECRET_ACCESS_KEY=
      gp env AWS_DEFAULT_REGION=us-east-1
