# Mumble Server

[![CircleCI](https://circleci.com/gh/willsoto/mumble-server.svg?style=svg&circle-token=959882b884046e51f676c2a6e1d4f51a6bdd2645)](https://circleci.com/gh/willsoto/mumble-server)

These Ansible playbooks will create a [Mumble](https://wiki.mumble.info) server on a [t2.micro EC2 instance](https://aws.amazon.com/ec2/instance-types/).

Credit to [Streisand](https://github.com/jlund/streisand) for the EC2 roles.

## Requirements

### AWS Access

Ensure you have your AWS access keys. You can get them [here](https://console.aws.amazon.com/iam/home?#security_credential).

### Ansible

Create a virtual environment and run:

```sh
pip install -r requirements.txt
```

## Running

```sh
ansible-playbook --inventory-file inventory playbooks/server.yml
```

### Developing

```sh
pre-commit install
```

### Testing

```sh
vagrant up --provision
```

This will run the mumble role only.
