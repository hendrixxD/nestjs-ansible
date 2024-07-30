# Automated Deployment and Configuration with Ansible for Boilerplates

## Screenshots
1.

_start of deployment_
![start_deploy.png](./imgs/start_deploy.png)

_half way through_
![start_deploy.png](./imgs/end_deploy.png)

_end of deployment_
![end of deployment](./imgs/end_of_deployment.png)

### Deployment Server
2.

   ```ssh
   sudo -u hng npm run start:dev
   ```
![runing server](./imgs/runing_server.png)

3.

Response on `http://127.0.0.1:3000/api/v1`
   ```ssh
   ansible hng -i inventory.cfg -b -m command -a "curl http://127.0.0.1:3000/api/v1"
   ```
   ![message on /api/v1](./imgs/message.png)

4.

runing nginx service
   ```ssh
   ansible hng -i inventory.cfg -b -m command -a "systemctl status nginx"
   ```
![nginx](./imgs/nginx.png)

5.

runing redis service
   ```ssh
   ansible hng -i inventory.cfg -b -m command -a "ystemctl status redis-server"
   ```
![nginx](./imgs/redis.png)
