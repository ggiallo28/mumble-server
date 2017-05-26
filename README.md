# Mumble Server

## Requirements

Ensure you have your AWS access keys. You can get them [here](https://console.aws.amazon.com/iam/home?#security_credential)

## Prepare 

```sh
pip install -r requirements.txt
```

```sh
pre-commit install
```

## Running

```sh
ansible-playbook --inventory-file inventory playbooks/server.yml
```
