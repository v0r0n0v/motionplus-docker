# motionplus-docker

This repository was opened as a test,
The task was to quickly deploy a docker container with motionplus.

size images: 1.37GB

Launch

1. Pulling the repo: git clone git@github.com:v0r0n0v/motionplus-docker.git
2. Go to the folder: cd ./motionplus-docker/
3. Download the motion-plus code: git clone https://github.com/Motion-Project/motionplus.git
4. launch the build: docker build -t motion-plus .
5. start container:

docker run -d --name=motion-plus -p 0.0.0.0:8080:8080/tcp -h motioneye -v /etc/localtime:/etc/localtime:ro --restart=always motion-plus

6. Go to the page of the project we raised: http://you_ip:8080
7. congratulations, you've done well

Addition:

Path to configs in the container: /usr/local/etc/motionplus
Binary path to launch: /usr/local/bin/motionplus

The photo shows the software version:

MotionPlus 0.1.1-git-20231020-70da5c1

<a href="https://ibb.co/mNY1Xs8"><img src="https://i.ibb.co/g4XHP1V/0-1-1.png" alt="0-1-1" border="0"></a>
