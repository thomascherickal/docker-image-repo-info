## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:c89e65d950775ced6555254d601f74987af0da690d16370e0b5a1881ad7ecdc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:be3bd0e9ad9b1bfa201092046aa111ed15e429892cada8ede01eea7097c65306
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300497941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2552ba432ab152d2c72b30990be71d54482da668cc845aa226d1cf84abfc12`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:38:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:38:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 29 Mar 2022 18:38:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 29 Mar 2022 18:38:10 GMT
ENV ROS_DISTRO=noetic
# Tue, 29 Mar 2022 18:39:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 29 Mar 2022 18:39:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 29 Mar 2022 18:39:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd41fb40810985980555ad4f3e5c98a2d1fb6aba5406dfb13c3a5751591bb3e4`  
		Last Modified: Tue, 29 Mar 2022 18:43:53 GMT  
		Size: 10.9 MB (10892020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd07b963a0a4666adbf672efe29068ca41a393dbe4e8857520f10bbf6567fbe`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15a903c4ecdd8129ebf93bbb6558cae4631b7c8cbdb52f7b8aabed4da3ec9d8`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0aa132a5f18476525f41162559ac29a36d8d7fae933dc20478fd1e1cdce0e`  
		Last Modified: Tue, 29 Mar 2022 18:44:24 GMT  
		Size: 239.2 MB (239165595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04437849c9723fd4c815474f1c9148d9917c601f413fd74c7f39a9de06b02e7b`  
		Last Modified: Tue, 29 Mar 2022 18:43:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:99c39bef50cdd00d850c3c9ab1e91f8a2505ec2f1f89fe200f5c5f0796b39d0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244290803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbd8471853ee4964dcb30625bb7ca89e30a3d288be782a0962b7764bcbceb30`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:34:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:34:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Mar 2022 04:34:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Mar 2022 04:34:25 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:34:26 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Mar 2022 04:34:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Mar 2022 04:35:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:35:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Mar 2022 04:35:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Mar 2022 04:35:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0436424bca719f680c1fa31bd209153e27bae4df6f8ab0c88f6f556fd86307`  
		Last Modified: Wed, 30 Mar 2022 04:44:00 GMT  
		Size: 10.7 MB (10688200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d686950d8b86d430859218f26abce26283e732385e6e4628c7429eba7832a100`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bd18027e243a00e84b9735b7938cde61199963e2bbc17ae05e85f67f80407`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86b5d2ea1e4b4e0797a8e0a2938389a64eb82319bb6529d624a6ec2a3fa569a`  
		Last Modified: Wed, 30 Mar 2022 04:44:29 GMT  
		Size: 184.4 MB (184374338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a27d959bf736646019bdf8cf51e4942ddecd224101884479f6ccca6070ee452`  
		Last Modified: Wed, 30 Mar 2022 04:43:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
