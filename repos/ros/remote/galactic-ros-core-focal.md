## `ros:galactic-ros-core-focal`

```console
$ docker pull ros@sha256:4e2809cdcc7af59431e0d7a2078e94b2441812ea8b6f905c7e27e143f2689241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:ca6d08f25fc4045ab6badd6401e4f48b41df0392c18b75acd63e10a611ecae48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138929413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459837a92d8240e96cdcdfa7a775c3e626fc7703324ae049861a215467f2b863`
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
# Fri, 01 Oct 2021 06:17:26 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 06:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:18:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 06:18:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:18:13 GMT
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
	-	`sha256:d9822a4f6cce53e502f5d2f90766f69c34822c58ef403536e917a5764f0da7c1`  
		Last Modified: Fri, 01 Oct 2021 06:28:28 GMT  
		Size: 103.6 MB (103627341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851399abce02bb2417f097f4b9e221270de786a2e80c2dc8fcbcfb1cb020ba9a`  
		Last Modified: Fri, 01 Oct 2021 06:28:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3b0fdd8bf86851bd4da361bfb1d9b5fdb989f169b1a756366a7952bde75ae273
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea9506a9ae0089fae05bac2076051fb643004efc0d0f3af33486b90af02baba`
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
# Fri, 01 Oct 2021 04:12:32 GMT
ENV ROS_DISTRO=galactic
# Fri, 01 Oct 2021 04:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:13:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 01 Oct 2021 04:13:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:13:15 GMT
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
	-	`sha256:f54decf9b73cbac297a45e39fb0f0a1737a8362434870dc3738d10beb0a2889d`  
		Last Modified: Fri, 01 Oct 2021 04:25:29 GMT  
		Size: 100.0 MB (100019555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5222af82eed2e3ce5f12efb7bf53fe5a36cd902d1aad23496451e2e5b7008cb`  
		Last Modified: Fri, 01 Oct 2021 04:25:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
