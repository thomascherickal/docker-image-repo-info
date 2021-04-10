## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:704f95293d14eb2a8c9f1efd26346c3872e100383c6af181957fdba1d757fc89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:0d714d837a4fa3d5b2b5c9058dd0ed5b208aeb208674d2557bd2addba8b2d4d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300344396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e65f9403f9e0df359d54b22a64323c81e782f1ee25c5a4735f66de4a0f76055f`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8754ad7a773d3c69dfb490faa9067785f613bde6f4ce36da2b8ea0a320da9650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244313750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4110c15a33acf5d795af50b2257aa6810e6f4ce18d0fc3d97508b5106edd3fbb`
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
