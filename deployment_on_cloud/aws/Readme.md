# Setting up EKS vLLM stack with one command

This script automatically configures a EKS LLM inference cluster.
Make sure your AWS cli is set up, logged in, and region set up. You have eksctl, kubectl, helm installed.

Modify fields production_stack_specification.yaml and execute as:

```bash
bash entry_point.sh YOUR_AWSREGION YAML_FILE_PATH
```

Clean up the service (not the VPC) with:

```bash
bash clean_up.sh production-stack YOUR_AWSREGION
```
