## `ros:humble`

```console
$ docker pull ros@sha256:3141cb337a6a9557de512baa0d78fe8fba551e41f52a72dd8ef8dc1562b58aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble` - linux; amd64

```console
$ docker pull ros@sha256:68d0f1cb0624c2becba5d4fe6d007c4fd99a992bbc2fa33dc59e4cfdf255db73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263047549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a7f3d015fbf1b8ac174c038036a4954d12efdeb3f47822b1eab0b754083db3`
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
# Tue, 31 Jan 2023 19:46:39 GMT
ENV ROS_DISTRO=humble
# Tue, 31 Jan 2023 19:48:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:48:25 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:48:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:48:25 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:49:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:49:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:49:24 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d7dbb0503db5f19ae74e3c7c940df7c5248d499d30ce0985e6409ac424799731`  
		Last Modified: Tue, 31 Jan 2023 20:12:47 GMT  
		Size: 106.3 MB (106349009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec811a3c99d671ab7f5d5f315d7f9d697eee754e3341d514f9655a6268f4e70`  
		Last Modified: Tue, 31 Jan 2023 20:12:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654827ae50559de75f17e31c8eb7d8114ae3c475c5d522c80fc93b9eb584da4`  
		Last Modified: Tue, 31 Jan 2023 20:13:10 GMT  
		Size: 97.9 MB (97886072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2abe6d5f00f78dbc81de4e1df815ec3a80701d8ff0d320e02c0431276b94b`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 309.5 KB (309524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733d6dcbe3a07073e084f07786756fd36746e07596df9e1e7be429415224ecd`  
		Last Modified: Tue, 31 Jan 2023 20:12:56 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a5d015357f84bdfc3267cb55ce2208054dbf6bd70bfde9a028d1da8e2980b4`  
		Last Modified: Tue, 31 Jan 2023 20:12:59 GMT  
		Size: 23.1 MB (23071097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c2d497729f6aee71e99bcdd9e454ad5eb1dd3468ae4d4effbf6d4f0ba96c689f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.7 MB (255709503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af910ab58e75966664e169632c6f9accf125c72c2c695d2fa000e4570f4eb25c`
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
# Thu, 02 Mar 2023 03:46:42 GMT
ENV ROS_DISTRO=humble
# Thu, 02 Mar 2023 03:48:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:48:35 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:48:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:48:35 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:49:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:49:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:49:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d13cc6d4ba7a8ad400f19bd92e8cb2286caeca1d46ce132719b2b1987256c21f`  
		Last Modified: Thu, 02 Mar 2023 04:10:13 GMT  
		Size: 104.1 MB (104057998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396dec5942a2fa6aff8e013fe4ebdcfabe51979982de742c3c3a1f04b10a63d5`  
		Last Modified: Thu, 02 Mar 2023 04:09:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617a68eb8bb8b1ab93ca9de116c7d22adcb04072699fcb1ad23a5f18e1ac0305`  
		Last Modified: Thu, 02 Mar 2023 04:10:33 GMT  
		Size: 95.5 MB (95477602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aea5ab66a030d09edeb6bd52a5d2d8c7ee9d2f179e47f3769d797ea1cec2eaa`  
		Last Modified: Thu, 02 Mar 2023 04:10:23 GMT  
		Size: 313.2 KB (313171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83267e4907f639f28f19da252316e35ac2d9754f0b1c072254ccbbae8c95aea2`  
		Last Modified: Thu, 02 Mar 2023 04:10:22 GMT  
		Size: 2.4 KB (2403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b408f45a9652713b3956f2c893ddb6bf2c327cde2e347d0ccd449062384917`  
		Last Modified: Thu, 02 Mar 2023 04:10:26 GMT  
		Size: 22.5 MB (22497086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
