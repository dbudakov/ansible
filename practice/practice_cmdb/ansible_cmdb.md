# ansible-cmdb

- [ansible-cmdb](https://github.com/fboender/ansible-cmdb)

Установка демонстация ansible-cmdb, веб интерфейс

```bash
# DONT USE ansible-playbook

ansible all  -m setup --tree out  -i ./inventories/

sudo rm -f /var/www/html/*
ansible-cmdb /vagrant/share/out | sudo tee /var/www/html/index.html >>/dev/null

curl -s http://192.168.0.121
```