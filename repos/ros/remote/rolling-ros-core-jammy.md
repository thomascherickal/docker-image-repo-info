## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:1db1c9a3127ddf6ed5b86be14d78a7edbb025d06fa369c4a5731e606fa204483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:f0db02e019e6a4b3934609861d6bd367d4d7ea1a5e549d9d4bf61b728a97d80b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141823212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15372d384c90753f1c0cffc69b1eab508dc0a8431ff96bb212b34f8218fd8b52`
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

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4cb42493ab078a7338cef0a920df6a02850c0ae562532644ca0439f0f00aaf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137282805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afaa184a751f99ac19d1e1f7ccaba533e7422cb55071c3f48a0f3a601561c90`
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
