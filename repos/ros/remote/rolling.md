## `ros:rolling`

```console
$ docker pull ros@sha256:237e50f8a5f85c1b8bb5e54ccf6fc54cb7ca7cef794135e9c50fd64c812ec26d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling` - linux; amd64

```console
$ docker pull ros@sha256:60f2a37f45af89cb5a543e58e191560ccc0da14b3ed1346578abc6873d702571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263707932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce213b690e983e6d1f65eec950595f8104e0b5a2a8c61823889ee8536220239`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:42:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:42:45 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 03:42:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:42:46 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 03:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:44:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 03:44:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:44:24 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:45:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:45:33 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:45:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 03:46:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341919f757e419f6142944f5ea95c19b61bf1ff648abdfff94ed8c99c0bfd52c`  
		Last Modified: Fri, 22 Apr 2022 03:55:07 GMT  
		Size: 1.2 MB (1191091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c8ef748e7b3e35f60511f8e8053ee76492c9a72a5afd00d55d351854556f`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 3.8 MB (3826746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b72761451ff916be9282f71adece9e357fc9710e86559b986d1f01583fd312`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3452459740e87b470a88f20122447689e1640a2b865eb50f2f4a866ad75d391`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2037c4fb46b3cec9022f679d45d7834d6c89ac325348efc7af3d5d92bcd7658`  
		Last Modified: Fri, 22 Apr 2022 03:55:22 GMT  
		Size: 106.4 MB (106381750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0221e7e4829eedc9594c53ce3492bccdc39ea2c1b77da83a10fdb689100c68`  
		Last Modified: Fri, 22 Apr 2022 03:55:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c7fbeb7e1d7385b2109f0df086ca744db3d917acd012c123fa8edc585a2080`  
		Last Modified: Fri, 22 Apr 2022 03:55:46 GMT  
		Size: 98.8 MB (98754384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b30b9dcc84973150cb0c195863fd24646a6ba41a76b5f0b33c806b25f12281c`  
		Last Modified: Fri, 22 Apr 2022 03:55:33 GMT  
		Size: 268.9 KB (268885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8e6a2755512e3269961eabe5ea4b4f1aec52de907316bb4f8654466d684b8a`  
		Last Modified: Fri, 22 Apr 2022 03:55:32 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba940d517ddac55ea1379c9f2cff56d93e8aa91f44e1303dc4a4261a1ef6810`  
		Last Modified: Fri, 22 Apr 2022 03:55:36 GMT  
		Size: 22.9 MB (22859264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3dfe17f949018783272b299a2a59c3e69c11fca5672006cc9ebb9edf2188879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255944624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51069cd265c1e26edf301600ec514b3b806b206530fca8cf5b20fc19c589c66`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:31 GMT
ADD file:31ce105f73c45fb89d7f254c71800e97a4774b64b3dfbc215bfb05848493ecee in / 
# Fri, 22 Apr 2022 00:54:31 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:15:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:15:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 22 Apr 2022 04:15:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:15:56 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:15:57 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:15:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 22 Apr 2022 04:16:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:16:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 22 Apr 2022 04:16:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:16:47 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:17:30 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:17:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:17:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 22 Apr 2022 04:17:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b5ca5a85338a7c13939e3609f3880b846d36862cce227eecd4c12af971cde8f`  
		Last Modified: Fri, 22 Apr 2022 00:56:28 GMT  
		Size: 28.4 MB (28376083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb989802917175cdb271141f4e081fa8e989cb5709d21d8ac4153b95085d52c`  
		Last Modified: Fri, 22 Apr 2022 04:27:16 GMT  
		Size: 1.2 MB (1192171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283604da4b314ff67f723c5bf1ba2a93801b4ecd9373906ace9b9accc2ce21b6`  
		Last Modified: Fri, 22 Apr 2022 04:27:14 GMT  
		Size: 3.6 MB (3593959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497a2e9ad1660ac6f4277bb83eb2b381668a1df22804fcc63dc3c87b2fb0b5b`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac029af969ad05ee2f310912643789cec16385d1820a3f5d52a4fdb0f6e8a2`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b7f771226a391368da04fd28620f186d7424276903e001d9ccf0d49568f34`  
		Last Modified: Fri, 22 Apr 2022 04:27:30 GMT  
		Size: 104.1 MB (104118226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976669ac24504d62fd730fdc9ae05cc6fb959bbbc0dc1ad0f2f65954450b1681`  
		Last Modified: Fri, 22 Apr 2022 04:27:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd1da39f9ae593499b9a4d3531127fd53836895c5cd5275c1e46e049e3c6b4d`  
		Last Modified: Fri, 22 Apr 2022 04:27:54 GMT  
		Size: 96.1 MB (96127137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a2e403ab0fabbcad25bddedfb2766fd50209e4c0e4af10d8aa5896d14a5260`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 268.8 KB (268831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfec5e8b47fa43a40b056c79b5047743be8d33a0356894a46708b23a5f805bd`  
		Last Modified: Fri, 22 Apr 2022 04:27:41 GMT  
		Size: 2.1 KB (2129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2398acbb01abaf3b5232dfcdc0535d9e2d2d0a8c4d6b0d419803ee2c398f4a6`  
		Last Modified: Fri, 22 Apr 2022 04:27:44 GMT  
		Size: 22.3 MB (22263722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
