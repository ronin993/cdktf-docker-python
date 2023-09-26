# cdktf-docker-python
A simple helloworld with Terraform CDKTF and Typescript

This tutorial is taken from https://developer.hashicorp.com/terraform/tutorials/cdktf/cdktf-install

## Prerequisites
In order to use CDKTF, you need:

- The Terraform CLI (1.2+).
- Node.js and npm v16+.

To follow the quickstart, you also need:
- Docker.
- Python v3.7 and pipenv v2021.5.29.
<br />

## Commands:
### Compile:

```pipenv run ./main.py``` Compile and run the python code.

### Synthesize:

```cdktf synth [stack]``` Synthesize Terraform resources to cdktf.out/

### Diff:

```cdktf diff [stack]``` Perform a diff (terraform plan) for the given stack

### Deploy:

```cdktf deploy [stack]```  Deploy the given stack

### Destroy:

```cdktf destroy [stack]``` Destroy the given stack

- Learn more about using modules and providers https://cdk.tf/modules-and-providers

### Use Providers:

  You can add prebuilt providers (if available) or locally generated ones using the add command:
  
  ```cdktf provider add "aws@~>3.0" null kreuzwerker/docker```

- You can find all prebuilt providers on PyPI: https://pypi.org/user/cdktf-team/
- You can also install these providers directly through pipenv:

  ```pipenv install cdktf-cdktf-provider-aws```
  
  ```pipenv install cdktf-cdktf-provider-google```
  
  ```pipenv install cdktf-cdktf-provider-azurerm```
  
  ```pipenv install cdktf-cdktf-provider-docker```
  
  ```pipenv install cdktf-cdktf-provider-github```
  
  ```pipenv install cdktf-cdktf-provider-null```

- You can also build any module or provider locally. Learn more: https://cdk.tf/modules-and-providers
