# imapsync-docker
Dockerfile for the imapsync utility

## Usage

1. Build the image first

  ```shell
  git clone https://github.com/yurkeen/imapsync-docker.git
  cd imapsync-docker
  docker build -t imapsync .
  ```
2. Run it
  
  ```
  docker run --rm imapsync --ssl1 --ssl2 --nosyncacls --syncinternaldates \
                           --host1 imap.fromserver.net \
                           --user1 fromuser@fromdomain.net \
                           --password1 supersecret1 \
                           --host2 imap.toserver.com \
                           --user2 touser@todomain.com \
                           --password2 supersecret2
  ```


