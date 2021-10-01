## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:8e9098074e85331503dc6644d6158203df77a60776f1328d83ee6901c49aea6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:971b28b6d4e0595f615c6362188b66f003e9e17571cc24798ed7a41ff5d1b2bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155281145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127b322a603b2a42aea08bdef92c8ce5d6b3f93292788ab143c7a981031d011c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:14:41 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 06:14:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:14:52 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 06:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:16:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:16:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:16:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe3314eae3636a83a175622f5ee93d41381af25d5201e7fb77518f504348b6`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed232d940ce0dca7a045676daa5b6f75ca20f1f218fa69fc26eb95d6e625d2`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a11bd747cd1c0f05aaf05f86b0b071e211e24fee36a2d1eba6287b56c3d495`  
		Last Modified: Fri, 01 Oct 2021 06:27:34 GMT  
		Size: 120.0 MB (119979073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048f14944693ffe48c11da0fab1a89302596d8549c164cbe52e259248057d6e4`  
		Last Modified: Fri, 01 Oct 2021 06:27:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f03c5cfea7fbbec6ac09aaee15eb8c0b436bdc364a0b4eb9732593e6ed040dd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (138025307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5969317ce1a30737f8e0e460aa31d369a062d4f2cdf3528755cabc468f301c2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:10:13 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 01 Oct 2021 04:10:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:10:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 01 Oct 2021 04:10:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:11:00 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:11:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:11:01 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f6bb99f825bcf3317a0b34e2dc1a4a5e29d1a809722d3d925e0854b098518`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd308002f060ef67048c13d059b7b55b15e9842c70fb6f42908d2b93609acbb4`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02714a0c044608ab1f7859767d58d255098ee9cebea2c7c5fab4ff70a31b6c`  
		Last Modified: Fri, 01 Oct 2021 04:24:27 GMT  
		Size: 104.2 MB (104153975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55c77ae30f9470c54c6ec75c59610b1c692ac602c8d71470e9ced72ae29481`  
		Last Modified: Fri, 01 Oct 2021 04:24:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
