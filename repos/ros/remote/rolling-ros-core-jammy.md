## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:7f2a3b8535a6ceea8415ff92355c7d8ffe1900d7ace1409f63f10d3089c89490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:88d8e636517283d5770a6934daa23f3085df98f2a7399f947111b5f48ef741f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154922349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07897d4d91378e7373d7bffa34dab18c8033a18f0d9288f05eaf42654eef357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:46:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:46:38 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:46:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:46:39 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:59:30 GMT
ENV ROS_DISTRO=rolling
# Tue, 31 Jan 2023 20:00:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:00:24 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 20:00:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 20:00:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841d9fe8d0ff117e288a003adeabeb14357e33e4aaeb9257fa966be44f049e8e`  
		Last Modified: Tue, 31 Jan 2023 20:12:32 GMT  
		Size: 1.2 MB (1169563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c427b1bb1855b88b68681612cfd3c47ddc0f7bf0af96dfbe3f1180a6f2413a92`  
		Last Modified: Tue, 31 Jan 2023 20:12:31 GMT  
		Size: 3.8 MB (3828410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78c7c7c697e8abb3149aa5d42619ca359de2bb03e4c2804b4136cc438866512`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740dbc132b076b321e969fa6e07fa61d94522609befffcd4716b01ba43c7c191`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0639606d4c30abe710b02e4245b4fde0a8ee07b0486abb6ac2f74126a215dc`  
		Last Modified: Tue, 31 Jan 2023 20:15:32 GMT  
		Size: 119.5 MB (119492954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f96ec662a48c684ba70d75e56b6831b6097f50bb4c0a99dcae6d3cfbe82e36`  
		Last Modified: Tue, 31 Jan 2023 20:15:12 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e394f41765f530ad2770ed87db90f1f573193f39bc49a07bfc7fa77c74126be6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150523404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5936a6233f7abbc6bcd6e5513f9083391b6511f6468b87d529828d8243968d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:46:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:46:40 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:46:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:46:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:46:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 04:00:41 GMT
ENV ROS_DISTRO=rolling
# Thu, 02 Mar 2023 04:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:17 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 04:01:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 04:01:17 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e362755fe88c9ce24cdfd898e23336ea1e231c0355f5d49a8a090f30dcc91641`  
		Last Modified: Thu, 02 Mar 2023 04:09:59 GMT  
		Size: 1.2 MB (1170222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980df12f072c7f0de28be975f627d604d5b9a0654e18d2621a5e2d310e3e137`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 3.8 MB (3800684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7b471ed8254de6e76b4dcdf32eb0960e56b82110798e4a53a070bf256d7fb`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d901dc6555255c6c878b02f88c977443c642128031c9d915198af1c15ea5bee4`  
		Last Modified: Thu, 02 Mar 2023 04:09:56 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1512e661fd644a0a4900ade6cc3896f1af3864cb271b92c768460df153fe80`  
		Last Modified: Thu, 02 Mar 2023 04:12:30 GMT  
		Size: 117.2 MB (117162162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0c490f5c253510c383ddd657e6887f0bb539a113c0a0435d523ba56efd749`  
		Last Modified: Thu, 02 Mar 2023 04:12:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
