## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:979669c08083f4b7e51e4b409b7c7e1362b120283fd2dd8bce343dd6db04ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:4507e4cbd47c43f67d4ebec7d59a7063d87aea338fc321f52420f57899f14547
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300283308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7d236abc604510366086130dc0c4c3db851368c6b8725bc2b4825ef6292296`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 14:28:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:28:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:28:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 14:28:18 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 14:28:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 14:28:18 GMT
ENV ROS_DISTRO=noetic
# Fri, 12 Mar 2021 14:29:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:29:43 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 14:29:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 14:29:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d439fcdce331cfbd24af9ec200a116545aa115d3565f78478dd27de2d0a7d1`  
		Last Modified: Fri, 12 Mar 2021 15:13:45 GMT  
		Size: 10.9 MB (10891929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51650f8a4757bf3345715d36180068660585c7ab7e9208cd8a1f05048c43659f`  
		Last Modified: Fri, 12 Mar 2021 15:13:43 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b343b7fc39597680e98dc41408965331c3e3ed3b9269d84be7f1cd031a2c36`  
		Last Modified: Fri, 12 Mar 2021 15:13:43 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e02de3945b88419c084f0e7ac6b834dbc8e0c104363de63c31fba1cc1fce99`  
		Last Modified: Fri, 12 Mar 2021 15:14:45 GMT  
		Size: 239.0 MB (238989185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef22b4194f4d468c5275483aeb7ce49bf3f0330060303106ff1ceed1ea7eaa6a`  
		Last Modified: Fri, 12 Mar 2021 15:13:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5f5c6b476657afdd39510daaaf2c883afa112cfb9c0d5ae4463c35a919d5837f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244274391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a6a55c4a5866415316ee2c1ef64a1ff3e3ab744eacbd08faa1265eade8806a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 19:15:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:15:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 19:15:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 19:15:37 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 19:15:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 19:15:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 12 Mar 2021 19:18:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:18:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 12 Mar 2021 19:18:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 19:18:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53046cb4ddd2c71f6f48556c69dfedd0d40a5668fdf7211c76a63e835e1a59cd`  
		Last Modified: Fri, 12 Mar 2021 19:31:25 GMT  
		Size: 10.9 MB (10883427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2db1c1ae82e6ec7deadf959bed6cb2a1ccc28d82d1f8b89e362a6d1c78ae22`  
		Last Modified: Fri, 12 Mar 2021 19:31:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b39bdde59f93cfc9c33e55d7844872af0b8276c969375dbe7f649f34627d95`  
		Last Modified: Fri, 12 Mar 2021 19:31:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a340b06b0b9f0b148ee2e0454acb4824581992881f71449f89c117579987f202`  
		Last Modified: Fri, 12 Mar 2021 19:32:16 GMT  
		Size: 184.2 MB (184193364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d010bf577e72811d88469dd00585be2b75a7b827944f190e4752bf3263ad6ddb`  
		Last Modified: Fri, 12 Mar 2021 19:31:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
