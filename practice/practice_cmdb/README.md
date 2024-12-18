# ansible-cmdb

Демонстрация работы ansible-cmdb

```bash
vagrant up 
vagrant ssh control
cd /vagrant/share

ansible all  -m setup --tree out  -i ./inventories/
sudo rm -f /var/www/html/*
ansible-cmdb /vagrant/share/out | sudo tee /var/www/html/index.html >>/dev/null

# результат работы
curl -s http://192.168.0.121
```