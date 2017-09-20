# Matt's work laptop customizations

ansible-playbook --ask-sudo-pass playbook.yml

Note: Must create a secrets.yml in root of project directory that looks like follows:

```yaml

# Red Hat Kerberos Principal and Local ID should be the same for the SSSD role to work
secret_local_user: mattsmith

# Created in the RHSM portal
secret_rhsm_activation_key: my_activation_key

# My RHSM org ID, most easily obtained by running "subscription-manager identity" on an existing RHEL system connected to your account on RHSM
secret_rhsm_org_id: 111111111111

# These two URLs can be obtained from internal helpdesk documents (see Matt's Mojo)
secret_redhat_itca_rpm: https://foo
secret_redhat_ovpn_rpm: https://bar

```
