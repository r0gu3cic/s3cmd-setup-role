# S3CMD-SETUP-ROLE

=========

This Ansible role is designed for setting up s3cmd tool on an Ubuntu server. This role prepares the server for production use, enabling server to use s3 buckets.
Config file is example for DigitalOcean space.

## Requirements

------------

This role is designed to work with Ubuntu distributions. It requires the following:

- Ansible 2.10.8 or higher
- `sshpass` for running the playbook with SSH password authentication.

## Role Variables

------------

The following variables can be configured for this role:

- **`s3.access_key`**: Access key.
- **`s3.secret_key`**: Secret key.
- **`s3.endpoint`**: Endpoint.

These variables can be defined in the playbook or in a `vars` file.

## Dependencies

------------

This role has no dependencies on other roles.

## License

------------

MIT Licence

## Testing Guide

------------

To run a local test for this role, use the following command:

```bash
ansible-playbook tests/test.yml -i tests/local_inventory.ini -u root -k --extra-vars "hosts=local_vm"
```

## Author Information

------------

This role was created by Stefan, aka enabler, aka r0gu3cic. For any inquiries or further information, please reach out via [GitHub](https://github.com/r0gu3cic).
