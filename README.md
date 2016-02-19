# cdh-roles

Before adding hosts to CDH cluster:
1) Add IPs to `roles/update-hosts/files/hosts` and run:
`ansible-playbook -i inventory-devcluster setup-before-cdh.yml --user=cloud-user --private-key=cdh.pem`

After:
```
ansible-playbook -i inventory-devcluster setup-after-cdh.yml --user=cloud-user --private-key=cdh.pem
```
