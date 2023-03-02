## `ros:rolling`

```console
$ docker pull ros@sha256:8a3378bafb6c6a6d530da9b14de17f0016e9bec37d6906a7cc7c64296068091f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:c9c3d1f71ee0e8129b4b01a60f28940324e0c358c84908882bf74b402402e7cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263048236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad19d33c21d926e1d9968c16cc3a41ec7f73c932b979f36182254a7b11e4f22`
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
# Tue, 31 Jan 2023 20:00:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:01:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 20:01:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 20:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bb6b909dcf612dd7292278d51e2aaa53308f2ec52dd9c9bfc178125ce9eceb32`  
		Last Modified: Tue, 31 Jan 2023 20:15:53 GMT  
		Size: 84.9 MB (84915070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a0899e286d8fed703554f8d5887507e2f13408a045817b81dfd9571837879`  
		Last Modified: Tue, 31 Jan 2023 20:15:42 GMT  
		Size: 298.8 KB (298805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07434028456fa3fa86ce7bf3537a45c9126091eb2482bd9db5e474f327edea24`  
		Last Modified: Tue, 31 Jan 2023 20:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8bae09c66c54facf036f53eb067ef4a64073c991441f2a457fffe8b21749b6`  
		Last Modified: Tue, 31 Jan 2023 20:15:45 GMT  
		Size: 22.9 MB (22909564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9f2826ba3c870ae4ddb1e82dd37a6f89a8c89846628c65bd7184a0cf41b09db0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256116645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dd48b3834ba4c4459cab11b489a03d8e8ca71fba3fbf16b12a986b01486b5e`
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
# Thu, 02 Mar 2023 04:01:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 04:01:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 04:01:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f25f9d6b96f8c0438546063d06191220803549e5b0ff9459d3e87bbe78c5824b`  
		Last Modified: Thu, 02 Mar 2023 04:12:47 GMT  
		Size: 82.6 MB (82628848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cefc12879615a02e1af0dfc5696868758fe87d9adc59064496024233964af4`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 300.7 KB (300740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ddc9b5c11c2319392bec026c322582406cf8a604872d0758472866c56950b`  
		Last Modified: Thu, 02 Mar 2023 04:12:39 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d224cc5443868b83b2ee7dd1eda419b6b2c07247b45b1a59f7cb938bb27f0c6`  
		Last Modified: Thu, 02 Mar 2023 04:12:42 GMT  
		Size: 22.7 MB (22661232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
