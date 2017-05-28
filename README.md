# Mumble Server

[![CircleCI](https://circleci.com/gh/willsoto/mumble-server.svg?style=svg&circle-token=959882b884046e51f676c2a6e1d4f51a6bdd2645)](https://circleci.com/gh/willsoto/mumble-server)

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
