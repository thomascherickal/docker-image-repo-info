## `ros:iron-ros-core-jammy`

```console
$ docker pull ros@sha256:1be64b7d89fd25f5a85eee5b92be95a7f3696e89225060d9bde07224ab163504
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:1bef6d4dca57ccf1f40b69ea40870eb19b765516f4ff98f42b300ffbd4482796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161866568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a8412314f5add223ada483750192b264e0d9928002b40d76ac7b42c3d6eba1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:59:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:59:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:59:29 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Jun 2023 01:59:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:59:30 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:59:30 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 02:10:30 GMT
ENV ROS_DISTRO=iron
# Fri, 02 Jun 2023 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:11:19 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Jun 2023 02:11:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 02:11:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe96d1fba3fa9e98471e901128195164795f58738d564b8e5333821c2d36fa`  
		Last Modified: Fri, 02 Jun 2023 02:19:54 GMT  
		Size: 1.2 MB (1212553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd030ad19cbefc93e59086b7b3a1d7d9202b78f7b9b6bee26e8b9143c3f34b4`  
		Last Modified: Fri, 02 Jun 2023 02:19:52 GMT  
		Size: 3.8 MB (3828373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e3c81f7012312e2bc2972b420a5563185979c68499270f73ff0c63597015ee`  
		Last Modified: Fri, 02 Jun 2023 02:19:51 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082bef69dc8cd56d3c591f03babaa60e31e94fcbf1e67695e2c04319f267f9ed`  
		Last Modified: Fri, 02 Jun 2023 02:19:51 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77780c4c126136e8a12bb468d6d6e634a2759bd527c76d837ff30a16dd78256`  
		Last Modified: Fri, 02 Jun 2023 02:22:36 GMT  
		Size: 126.4 MB (126392948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb69b122370996abbb04b98810f22d536235d44dbf22be9fb8f2426ca2fb8a`  
		Last Modified: Fri, 02 Jun 2023 02:22:17 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ec16631ea5fd743af62667e8849d73f8cbc81f0ee4beaec85c1e8a019798317c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155018679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fe6f1c8df8149aaa3bc208f0042e2cbd748743843abddf667803840535fa8a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:22:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:22:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 16 Jun 2023 01:22:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 01:22:21 GMT
ENV LC_ALL=C.UTF-8
# Fri, 16 Jun 2023 01:36:04 GMT
ENV ROS_DISTRO=iron
# Fri, 16 Jun 2023 01:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:36:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 16 Jun 2023 01:36:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 16 Jun 2023 01:36:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254e648ecdfc867db0b42c6dbd4640c3f7f9b6ba3a884f30c88384561d38d6ee`  
		Last Modified: Fri, 16 Jun 2023 01:47:02 GMT  
		Size: 1.2 MB (1213527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f811aafc45c062b5c1d9c3c624d4bff1dedfdc438dd8870309e1dc91901d96`  
		Last Modified: Fri, 16 Jun 2023 01:47:00 GMT  
		Size: 3.8 MB (3801066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ed4d8208fedb864dbcc1837f588b07dc9126ba57c6f8902e82adb80853b7e`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6454f40413af60c629e3a0ba0acaa7a2a321a8bdf245ab80623052b37f0052d8`  
		Last Modified: Fri, 16 Jun 2023 01:46:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e41c2e8b43236d79b82b2ce24c1f568a4a3ea25c30dfdc4895cce00480072`  
		Last Modified: Fri, 16 Jun 2023 01:49:43 GMT  
		Size: 121.6 MB (121612466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14e36042bc13bfe0d1c0fb91a96ad3ed768c36fbac710c2082179a1022f1da`  
		Last Modified: Fri, 16 Jun 2023 01:49:22 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
