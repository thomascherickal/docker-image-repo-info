## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:1dff9243d94d47fc980259fc398b6c9e5f6b94911d7c4bf5b304cdb48f0dd794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:105f8658d8405e3398963e7dba92d1f3621e206f1c33e2ed6da8430349c03365
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463095715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba7b56ea2d3c33b3d139eae3132f4689bd93cabce7a2e350b0d8647ec97518b`
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
# Fri, 12 Mar 2021 14:30:18 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:30:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 14:30:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:61941cae869a833b7d2642e3dcada6cf0f5b389aa8374be8fe2a6808975c65f6`  
		Last Modified: Fri, 12 Mar 2021 15:15:20 GMT  
		Size: 86.6 MB (86566494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7404043514149d9500f8523d98bf28e7b6d26a482307648255b6686705e00`  
		Last Modified: Fri, 12 Mar 2021 15:14:56 GMT  
		Size: 271.1 KB (271088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71893e1a186340ab22df78a026c2447e49960b6b3b7145050a7344452b17898e`  
		Last Modified: Fri, 12 Mar 2021 15:15:19 GMT  
		Size: 76.0 MB (75974825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1f272830d86717476a954a930975f43266b2ba494238d6cd9ece2d2838641377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.0 MB (402989563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a28cc087c2728ef1872bb66eec043eee1e767d661718ce3c4284a2952cc5b32e`
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
# Fri, 12 Mar 2021 19:19:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:19:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 19:20:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:5baca0e537f99398b8fc49cb67f036929eb2c0e10903d4c1b950573899aa827e`  
		Last Modified: Fri, 12 Mar 2021 19:32:43 GMT  
		Size: 84.4 MB (84355178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5149f734a8f7339aefd08d7be0f0891d0cb52339a2139d65b1abd5b41e2f85c7`  
		Last Modified: Fri, 12 Mar 2021 19:32:24 GMT  
		Size: 271.1 KB (271096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7bc09c9720385cf565207a02027f1b25b651be83d2284103b33cd9d241a325`  
		Last Modified: Fri, 12 Mar 2021 19:32:42 GMT  
		Size: 74.1 MB (74088898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
