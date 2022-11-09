# Description

- [Terraform docs](https://www.terraform.io/).
- [Ansible docs](https://docs.ansible.com/).

## Build infrastructure

```sh
terraform init
```

```sh
terraform validate
```

```sh
terraform plan
```

```sh
terraform apply
```

## PEM

For Terraform complete provisioning on AWS, we must create an SSH pair key under EC2 - Security and
save as `iac.pem` on this project root folder.

## Opening HTTP server

```sh
nohup busybox httpd -f -p 8080 &
```

## Using Ansible playbook

```sh
ansible-playbook playbook.yml -u ubuntu --private-key iac.pem -i hosts.yml
```
