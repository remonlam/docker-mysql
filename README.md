# Running MySQL in a Docker container.
![Docker & MySQL banner](/images/docker-mysql-cloudplus-banner.png)

### Docker automated builds
The Docker automated builds can be found over here: https://hub.docker.com/r/remonlam/docker-mysql/

### Pull Docker image
docker pull remonlam/docker-mysql

### Start a container based on this image
docker run --detach \ <br>
  --name mysql \ <br>
  --env MYSQL_ROOT_PASSWORD=$ROOT_PASSWORD \ <br>
  --env MYSQL_USER=wordpress \ <br>
  --env MYSQL_PASSWORD=$WORDPRESS_PASSWORD \ <br>
  --env MYSQL_DATABASE=wordpress \ <br>
  --volume /Users/$USER/docker/mounts/mysql:/var/lib/mysql \ <br>
  remonlam/docker-mysql <br>
