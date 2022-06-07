# Docker_and_Ansible
![img](./img.png)  
[記事](https://pro-broccoli.com/2022/06/07/docker_and_ansible/)
- Ansibleコンテナとターゲットコンテナを生成
- Ansibleコンテナからターゲットコンテナに対してplaybookを実行

## 手順
```bash
git clone https://github.com/hgssnk/docker_and_ansible.git
cd dockerfiles
docker-compose up -d --build
docker exec -it ansible /bin/bash
ansible-playbook -i hosts playbook.yml
```

## 参考
[【Ansible】DockerでAnsibleハンズオン](https://qiita.com/knaot0/items/39eeefa5de652b857372)
