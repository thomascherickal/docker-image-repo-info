## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:bb6f19ef59ff33c37a77d53128567048c6026526e2cde9a7d03998324a429e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6c3d1c582c2b6d28c0873ef8830fa7009d7c133deff33110e608b8a3d4fc1d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.3 MB (212302189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e86a2e87f5ee62ba3387862b4bf453b2c08bf22ea33af6e127be70e416ba88`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:28bb604051b10c25f4a37d070854a85a6cc436b0d7dde3a10fc46ae64bec79c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187940377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9daae24dfaedd2dfe709a4a184f6a9f6fad1d16fb324ede62db313c1a5c03c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b1d00726fd3fa46d77524a8053bd609365b5abae3a17a67f3683bf297ee8bd0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.6 MB (209551852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ef109a0615f2e6a12306ea2f79634e967bff0243f3dedb39dd1725cacedabe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:21:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:21:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:37:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 09 Dec 2023 02:37:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV LC_ALL=C.UTF-8
# Sat, 09 Dec 2023 02:37:28 GMT
ENV ROS_DISTRO=noetic
# Sat, 09 Dec 2023 02:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 09 Dec 2023 02:40:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 09 Dec 2023 02:40:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 09 Dec 2023 02:40:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2aa78ed8ad18394d7ae521e83b2810fec9fbb7d95aa074d794bb43e6e2bbfb`  
		Last Modified: Sat, 02 Dec 2023 06:56:12 GMT  
		Size: 1.2 MB (1198781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f106a95fef578814e019c4ac69f1cf32b15d5f85da2729a7ab2487c5d3505d`  
		Last Modified: Sat, 02 Dec 2023 06:56:11 GMT  
		Size: 5.5 MB (5532202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde5587588684db83e0c22fb5d4979df124ea1cb18322ace2e4c3ea5c96b6367`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c5b1b69c1b0400c6d51e9b08a29868443a22bc46ce96467a1b6fd75f9aa2c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c0f3f95aca8df1ff165733b239844d0700cbd97842b1699375b9137cd0075e`  
		Last Modified: Sat, 09 Dec 2023 03:56:30 GMT  
		Size: 175.6 MB (175614595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648bea585de95bdc098b0f496d2c461fc072dda803fe1be92b970893fd65443c`  
		Last Modified: Sat, 09 Dec 2023 03:55:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
