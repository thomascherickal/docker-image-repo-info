## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:d7440c005855172ec45e4263a007280a6fa88c96a1998caaa10ccf7b36efc02f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:f004dbe4702adbc42c8c299b5431dee4a23bbf5e220a0bd3c7813d95f51ec58f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161879020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d500b8ee85c194cf8917560934588da4e4a97f06879703c6de87418331368fa5`
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
# Fri, 02 Jun 2023 02:14:11 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Jun 2023 02:14:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:14:53 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Jun 2023 02:14:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 02:14:53 GMT
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
	-	`sha256:17f648e5f783f5f36ef3f74417ba45a66c66ec8042c4f22f81e7fb89ab6dbc05`  
		Last Modified: Fri, 02 Jun 2023 02:25:01 GMT  
		Size: 126.4 MB (126405400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cb1fbf3c1eeda6610da778d3946bc8a6fcaf4acb94f51338938bdf1e4b2d9`  
		Last Modified: Fri, 02 Jun 2023 02:24:41 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bb06b912e5e9892c99ebea166c68b7eed9c19ef3ecceb1877f7eb50fb785e107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.1 MB (157123743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cff6c785807159b668e1afc7ebc1c8a0a81dba30218ba22f3ff41e01f71864`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 22 May 2023 17:53:00 GMT
ARG RELEASE
# Mon, 22 May 2023 17:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:53:07 GMT
ADD file:f0435ed8dcf91cc69ec63b6b16d9efac56e5a6a7ec518e1fcc3df7457d3113ed in / 
# Mon, 22 May 2023 17:53:08 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:19:59 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:20:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:20:18 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Jun 2023 00:20:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:20:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:20:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:37:33 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Jun 2023 00:38:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:38:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Jun 2023 00:38:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:38:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6c7698a779f6d8c45a39a6721fb5cce267d66ff8ab5181c55aa6d02c8ddacd01`  
		Last Modified: Tue, 23 May 2023 02:05:13 GMT  
		Size: 28.4 MB (28389044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755c90e9cf79faad5cb53bf52c5426df1ff04c218894ffbb077e2524f6d717e2`  
		Last Modified: Fri, 02 Jun 2023 00:43:37 GMT  
		Size: 1.2 MB (1212932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35deec7a88f66396ce147c78c621f166491b3bb0d43295ac2a27879c9d37369e`  
		Last Modified: Fri, 02 Jun 2023 00:43:35 GMT  
		Size: 3.8 MB (3800450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef7ef73bca581875e598a71ca009ce9fded1b1da4ce3b0c008979125eb05d7`  
		Last Modified: Fri, 02 Jun 2023 00:43:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037d33ca89bd5d376d834aebec1592a65631f40a1423a08a248d2b1c8df162c6`  
		Last Modified: Fri, 02 Jun 2023 00:43:34 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ae22005ca62c74f2251e85c2a21524375ba0becb6d508e2607b5db093ddfe0`  
		Last Modified: Fri, 02 Jun 2023 00:48:11 GMT  
		Size: 123.7 MB (123718906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de066b41a04e9f87e1fd43528b4563aa6325aaee7ec59e952fba8c66d3d89e51`  
		Last Modified: Fri, 02 Jun 2023 00:47:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
