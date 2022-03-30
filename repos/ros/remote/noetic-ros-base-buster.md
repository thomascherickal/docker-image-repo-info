## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:68292f6442d9a335f0c095dd3a79684a37f4bfb5571fac950473af2b4b355c16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:e96e34d4dbcd475ca6cf853d057fb8570bf32fc53bcd4435d06411b728d0c121
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463345704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ae4dfb48508ccf4b9cc436b97de0230175db74153eb3b6a7c0b94e10f1afe1`
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
# Tue, 29 Mar 2022 18:39:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:39:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 29 Mar 2022 18:40:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4312d90907c6e468e1d0d5dca383651b811b150e9b6e169af56a5650d492fe38`  
		Last Modified: Tue, 29 Mar 2022 18:44:45 GMT  
		Size: 86.6 MB (86566668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b306a49cda07cd17bf29d90b1b872d94dfefcec3a9a19e13770ae6b052165d7`  
		Last Modified: Tue, 29 Mar 2022 18:44:32 GMT  
		Size: 305.0 KB (304968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e60e6f9eb483ac56169058a0ad6cd0a9f4d5438c948eeb61f5d931c47b346fd`  
		Last Modified: Tue, 29 Mar 2022 18:44:43 GMT  
		Size: 76.0 MB (75976127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5cc576a7d1f81464d643eebcb8fc69b455081e737eb974d9c3fc8968850bc3fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402811997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfd5679fb23e1214d8b101e73d52266aaf7f053a7122cfaf9f23214a97fa5cd`
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
# Wed, 30 Mar 2022 04:36:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:36:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Mar 2022 04:37:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c5db582a1aecd5ca67e5b89c286be79777101278f9914867e9e19070a0c52db4`  
		Last Modified: Wed, 30 Mar 2022 04:44:48 GMT  
		Size: 84.4 MB (84351038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa363f4fd3acddae5e480d68c74edd2ad900349f498c9d74774e1fbd98ce84`  
		Last Modified: Wed, 30 Mar 2022 04:44:38 GMT  
		Size: 304.9 KB (304925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e3c3857cda4e11d22479d728cf8b9caad08735e08d037d5512627830dcc03f`  
		Last Modified: Wed, 30 Mar 2022 04:44:47 GMT  
		Size: 73.9 MB (73865231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
