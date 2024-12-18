# machine_id

Сбор значений /etc/machine_id на controlnode, тремя способами

```bash
vagrant up
vagrant ssh control

cd /vagrant/share
ansible-playbook -i ./inventory/ 01.playbook.yaml
ansible-playbook -i ./inventory/ 02.playbook.yaml
ansible-playbook -i ./inventory/ 03.playbook.yaml

# результаты сбора фактов
ls -l /vagrant/share/out
```