## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:ebe3629a857c25505f17cbd1285994d748cd41d8843c236eca4bb1865b6ff81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:4a76deae2883ad607454aacf5d6cf1cf978cf9b8fd1f10b5deeb19c1e04e66cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.4 MB (484376349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc6023da50bafa7cbb83bded85c244a0ca652c7dffe0cf69da9647820b089fb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:28:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:28:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 10 Apr 2021 17:28:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 10 Apr 2021 17:28:55 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 17:28:55 GMT
ENV LC_ALL=C.UTF-8
# Sat, 10 Apr 2021 17:28:56 GMT
ENV ROS_DISTRO=noetic
# Sat, 10 Apr 2021 17:29:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:29:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 10 Apr 2021 17:29:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 10 Apr 2021 17:29:57 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:30:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:30:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 10 Apr 2021 17:30:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:31:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fd28af89a0ec9fa7157e75ed0261639c0702b8898b0a3b81554dc41b1ce18`  
		Last Modified: Sat, 10 Apr 2021 17:39:07 GMT  
		Size: 10.9 MB (10891856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20806ddcc138c4e5019982aea0dbf501e123c81985010951ce27cb94a8adff25`  
		Last Modified: Sat, 10 Apr 2021 17:39:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5178e646abf53ad34c7703b18289d4cd11b2c157ac1db512d75cd60930f05`  
		Last Modified: Sat, 10 Apr 2021 17:39:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adfcdeaa5de540b72df582982773b9c0821a7569d4ea0e25941cf47690610f6`  
		Last Modified: Sat, 10 Apr 2021 17:39:43 GMT  
		Size: 239.0 MB (239017733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b70b18fc6d7282af35cad3bac815061d46d925b61cf03003a6d72ad3c0b7e2`  
		Last Modified: Sat, 10 Apr 2021 17:39:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0491425016129d8d01213f6600d2e0de25fb249b8dec1b787377ed1fb0189b`  
		Last Modified: Sat, 10 Apr 2021 17:40:07 GMT  
		Size: 86.6 MB (86565682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bb5a193c722e39b341fa35767a7c99c431423ce22dbc7e474e119ccdbc6bfb`  
		Last Modified: Sat, 10 Apr 2021 17:39:52 GMT  
		Size: 276.4 KB (276394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2045d3560751fbf29e11c60a692646a1c74e807e85481209ae6bf6b83fb134`  
		Last Modified: Sat, 10 Apr 2021 17:40:05 GMT  
		Size: 76.0 MB (75974966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29146bf62b5b3732b087d20d9ac4059fb7c556ad171dd34df17df37652b11d1c`  
		Last Modified: Sat, 10 Apr 2021 17:40:18 GMT  
		Size: 21.2 MB (21214911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:aa51bb6360e7bac0da5813c7e375b6b285b410f751f7ac387a99275a39a1d56c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423903217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3346eb67997304b948f0b8ece9a4611ea3f122d9e2effe10c89b4af3624e807b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:59 GMT
ADD file:320ad0e2a3d6c676ddb8ce5646b5a94d18d82a8868955da3a9379a261dfe1ffe in / 
# Sat, 10 Apr 2021 00:41:01 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:37:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:37:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 10 Apr 2021 15:37:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 10 Apr 2021 15:37:16 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:37:17 GMT
ENV LC_ALL=C.UTF-8
# Sat, 10 Apr 2021 15:37:18 GMT
ENV ROS_DISTRO=noetic
# Sat, 10 Apr 2021 15:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:40:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 10 Apr 2021 15:40:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 10 Apr 2021 15:40:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:41:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:41:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 10 Apr 2021 15:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:43:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:01cf0f0da10ede0eec0fc1c5fbfdeb63a447dfcc0a3c4419c0a4c3f0a2826636`  
		Last Modified: Sat, 10 Apr 2021 00:47:28 GMT  
		Size: 49.2 MB (49225782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a3b7dee476a7c21f147f8ba83dfd7c574332ae1351bab531f996d1f40d252`  
		Last Modified: Sat, 10 Apr 2021 15:56:28 GMT  
		Size: 10.9 MB (10883505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d476645129f490eb4af61264fcab0cb2bd9eb9af56e8c2a84a027e733bbb7a`  
		Last Modified: Sat, 10 Apr 2021 15:56:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed05dd4c3440f5d1ca1c0b4deec634cee528af76b508e0909d0d75d0f0ac896b`  
		Last Modified: Sat, 10 Apr 2021 15:56:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbd4e4275f95551283e9dade9816ebd70b2885ef7d355b9c6bad63be31d7863`  
		Last Modified: Sat, 10 Apr 2021 15:57:30 GMT  
		Size: 184.2 MB (184202626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147fa70d954f9519fefbf0d8866f60d576cf506dc64a41f60f017b8ef416f838`  
		Last Modified: Sat, 10 Apr 2021 15:56:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a473f227cf740e3c139957b5ddf02997e137c602d3be3a576ce51dd91696eb0`  
		Last Modified: Sat, 10 Apr 2021 15:57:57 GMT  
		Size: 84.4 MB (84355758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37993ff61eb58e3fbe83d66af5f42aa709c1bdec6617606cee9423557fcd8fa`  
		Last Modified: Sat, 10 Apr 2021 15:57:36 GMT  
		Size: 276.4 KB (276397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51720a1eccbe930e8c3ca42e1259593fb1e914af8375becab8e6436e929bdab`  
		Last Modified: Sat, 10 Apr 2021 15:57:56 GMT  
		Size: 74.1 MB (74089062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3dc8e191354812f0a2afb846422ce84fb08e1373ea1036bd45e9fe48756795`  
		Last Modified: Sat, 10 Apr 2021 15:58:10 GMT  
		Size: 20.9 MB (20868250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
