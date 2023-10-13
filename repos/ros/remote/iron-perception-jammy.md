## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:cb535badfa79a35bbc5539ccb4fc571bf37dfcb5139c8cdc1bf89ad70f607e8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:4400f1351028d53b91050c218dfdcc2f7789e3a81f455d29a8b9b3b0217c8524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.8 MB (959779689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194961637a94c49e7e4e866077db62535a28131f8eee30f289a32b51974dc899`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 09:10:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 09:11:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 09:11:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 13 Oct 2023 09:11:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 13 Oct 2023 09:11:05 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 09:11:05 GMT
ENV LC_ALL=C.UTF-8
# Fri, 13 Oct 2023 09:23:57 GMT
ENV ROS_DISTRO=iron
# Fri, 13 Oct 2023 09:24:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 09:24:45 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 13 Oct 2023 09:24:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 13 Oct 2023 09:24:45 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 09:25:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 09:25:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 13 Oct 2023 09:25:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 13 Oct 2023 09:25:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 09:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88f4f42a82353a9c0283985de717a459b19bfb2efc359c4829a806484d20e81`  
		Last Modified: Fri, 13 Oct 2023 09:33:58 GMT  
		Size: 1.2 MB (1212966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c891fc2128fdc51ff82124d6dd8772e6f15b9d49b492bcffcb32904fad3d37`  
		Last Modified: Fri, 13 Oct 2023 09:33:57 GMT  
		Size: 3.8 MB (3828820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348881bc17ed1b5cc9deae183d10e21fd2c2b23014d9af63f6a686117b20f7ab`  
		Last Modified: Fri, 13 Oct 2023 09:33:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d3a94e39139da8a88b5221c31a1e2766e0377f2fe424397759e44d36322beb`  
		Last Modified: Fri, 13 Oct 2023 09:33:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a71a51fc13dccb3db719be64cb41c5683eb7cdab53ad5014f61544f34cf22da`  
		Last Modified: Fri, 13 Oct 2023 09:36:46 GMT  
		Size: 124.2 MB (124214606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05a5bca23e9a5b29bfe875724698516920afe1583e3125c80ef6fb24db5d46f`  
		Last Modified: Fri, 13 Oct 2023 09:36:26 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbad940e75fa6feaf214f9a87ae68972ed6d925abc7d050104515ef09b81d8a3`  
		Last Modified: Fri, 13 Oct 2023 09:37:06 GMT  
		Size: 85.2 MB (85168726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7c81e35efc137953f14cd34c5b337b4ab44b9290fee23a1fcf6015afaf9fa5`  
		Last Modified: Fri, 13 Oct 2023 09:36:55 GMT  
		Size: 305.0 KB (305021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494818067063196a175679cb215ff90cbe18e2f41e19bace8aaf29db92c93353`  
		Last Modified: Fri, 13 Oct 2023 09:36:55 GMT  
		Size: 2.5 KB (2483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c89d53e365576e1d67c2113b5bb3b9d1c1bb88f7fb5627e0526ac306220306`  
		Last Modified: Fri, 13 Oct 2023 09:36:59 GMT  
		Size: 23.7 MB (23730379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da784f83593e88981fb05168f76fd65b105dbebfe27e882c330ccf01f49a15a`  
		Last Modified: Fri, 13 Oct 2023 09:38:46 GMT  
		Size: 690.9 MB (690875161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b834e3b6e098d103e392d8d18279ce16e41f80bd3d24fee8262623948cbd5ccc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (920007927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca995c3df947fa505348a84f5e41a19b515da2924363f12278987903b8c5d4b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 04:37:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:38:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:38:05 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 13 Oct 2023 04:38:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 13 Oct 2023 04:38:06 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 04:38:06 GMT
ENV LC_ALL=C.UTF-8
# Fri, 13 Oct 2023 04:50:42 GMT
ENV ROS_DISTRO=iron
# Fri, 13 Oct 2023 04:51:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:51:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 13 Oct 2023 04:51:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 13 Oct 2023 04:51:31 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 04:51:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:51:57 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 13 Oct 2023 04:52:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 13 Oct 2023 04:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:54:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18d61171fb1a17fb0edecb7a0600d4d0be1c103726f9d60cfb59071d3eccf9`  
		Last Modified: Fri, 13 Oct 2023 05:00:30 GMT  
		Size: 1.2 MB (1214464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa41e452048780b8d89bde1b448e5c130e073ab26d8a3c3e2ec3d4a4170f55f`  
		Last Modified: Fri, 13 Oct 2023 05:00:27 GMT  
		Size: 3.8 MB (3801906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c55f0e8967a89d129c1106434dacd41bd9239f7fe793b4dc37245f7a26762f`  
		Last Modified: Fri, 13 Oct 2023 05:00:27 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023f71811e459a590f4b10edecae765c4b654f7139277e4c704f11126c720c5f`  
		Last Modified: Fri, 13 Oct 2023 05:00:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7e5397da56a4ded96341848bbe099efaf06181bb8a09f3720aeb98cd49c69`  
		Last Modified: Fri, 13 Oct 2023 05:03:18 GMT  
		Size: 121.7 MB (121671888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b628474c464bf47e0464b172ff209e5e12441f2570b8a83504c6ef68bc1f77`  
		Last Modified: Fri, 13 Oct 2023 05:02:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82511f0dabbf715d554877bab0fec36b1418a40aa932175ad0816f595105f435`  
		Last Modified: Fri, 13 Oct 2023 05:03:35 GMT  
		Size: 82.8 MB (82845322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a7517588a907a56e240f9131473fa8f9e8f3453f23e00a962242a46ea01bc9`  
		Last Modified: Fri, 13 Oct 2023 05:03:27 GMT  
		Size: 304.9 KB (304924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7110d57994728ed7d08117f21b0158ae78a4cb11c5efb4b68db0626e995e099`  
		Last Modified: Fri, 13 Oct 2023 05:03:27 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e9dc421947da7f84fb4df824e59128c51449f0220cbfa2ee41ee150798241d`  
		Last Modified: Fri, 13 Oct 2023 05:03:31 GMT  
		Size: 23.1 MB (23117319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1faa38f97a7c630c926e01526405373d132b0e63c87daf4f874d27dea1eaa825`  
		Last Modified: Fri, 13 Oct 2023 05:05:11 GMT  
		Size: 658.7 MB (658655305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
