# Simple Docker SFTP server.

1. Install Docker.
2. You can change **port** 2222 to any in docker-compose.yml file.
3. You can change **user** ('foo') and **password** ('pass') to any in docker-compose.yml file.
3. Run:
```
docker-compose up -d
```
4. Connection example for PHP (on Windows):
```
$sftp = new SFTP('host.docker.internal', 2222);
$sftp->login('foo', 'pass')
```