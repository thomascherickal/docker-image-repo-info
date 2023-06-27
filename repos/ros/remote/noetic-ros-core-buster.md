## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:4e760786e79c3a9e0a888de499f0c326e934e686707ac7a50f4fe30e13fd81d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:01b186e3cb098181d56105de494565c91befca6fdb9a0cd0a0a413db5f305be9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300597073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229d3208f89cfcab4653948befc7fc0a1c11f082a4d7db1fc1990c8b8fdd648d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:19 GMT
ADD file:54838b3dbf7839dadd0b29835bbe53ecbfdfde657ef8671ec5ac3cf5867ea069 in / 
# Mon, 12 Jun 2023 23:21:19 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:08:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:20:49 GMT
RUN echo "deb http://snapshots.ros.org/noetic/final/debian buster main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 27 Jun 2023 01:20:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 01:20:51 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 01:20:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 01:20:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jun 2023 01:22:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 01:22:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 27 Jun 2023 01:22:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 01:22:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ac8bb7e1a32398e26c129ce64e2ddc3e7ec6c34d93424b247f16049f5a91cff4`  
		Last Modified: Mon, 12 Jun 2023 23:26:48 GMT  
		Size: 50.4 MB (50448512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cf5c15547519baec38e96827f04dc5f08cfb702fc8765dfa47ba9b8eb2bd`  
		Last Modified: Tue, 13 Jun 2023 17:17:32 GMT  
		Size: 10.9 MB (10897084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca51b4c58c0584ed69a618914b0b2c4f50f9d813aa45705d26d84487111652`  
		Last Modified: Tue, 27 Jun 2023 01:36:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed4c52cac8a0cefc5f1c09a110eceba6c8c2dd67b0794fac78a8a76c6eab152`  
		Last Modified: Tue, 27 Jun 2023 01:36:31 GMT  
		Size: 3.2 KB (3221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06558bc538997bfde288afa7ad8dc75a26bf86a173687d8ecb4835c1604a1ed`  
		Last Modified: Tue, 27 Jun 2023 01:37:02 GMT  
		Size: 239.2 MB (239247831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4de4055bb55cdced21af8b9bd8d7208db93781433edb09ec77f762f66a4a7`  
		Last Modified: Tue, 27 Jun 2023 01:36:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:411877c67df0826901bfad2b7cbc34b87ae38c5f336f73be47edfbc5dae38440
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244612580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427e1e2f216655329159059122d62ae6749376e249f43362b9a8ba2ea1a500ed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:41 GMT
ADD file:bb3cb9e6abc423742d7c1b6bc006a7cef70038c5621c71a90a2ae7c1ea29ec63 in / 
# Mon, 12 Jun 2023 23:40:42 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 13:42:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:14:45 GMT
RUN echo "deb http://snapshots.ros.org/noetic/final/debian buster main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Tue, 27 Jun 2023 02:14:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Tue, 27 Jun 2023 02:14:47 GMT
ENV LANG=C.UTF-8
# Tue, 27 Jun 2023 02:14:47 GMT
ENV LC_ALL=C.UTF-8
# Tue, 27 Jun 2023 02:14:47 GMT
ENV ROS_DISTRO=noetic
# Tue, 27 Jun 2023 02:16:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jun 2023 02:16:35 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 27 Jun 2023 02:16:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 27 Jun 2023 02:16:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e8371d57f7426517aead21bff5af0cf321625cac166c86214c439fb67db84243`  
		Last Modified: Mon, 12 Jun 2023 23:45:01 GMT  
		Size: 49.2 MB (49238409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03375f4355e227cafbfa908999c3ddc516dfece8850f794cbfee3d98a3b0e4d`  
		Last Modified: Tue, 13 Jun 2023 13:51:27 GMT  
		Size: 10.9 MB (10902698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45b1051edd106997caba4f1579a4b2d4504d49a9f038bd54e527ed3c6af1f20`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69434a5448d8f4de484bef98eebf3d4c5b06d3e23a551a42d2ffa417bfccaa9b`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 3.2 KB (3220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d304c38e18c1dc16bf7685a133b35ef5a4146eda4daf5588d8e10614644dc11`  
		Last Modified: Tue, 27 Jun 2023 02:32:16 GMT  
		Size: 184.5 MB (184467829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb2d67a4b4053020362b7ffdebed6f8cdcfc288a27b86a226d683d27bb74c3`  
		Last Modified: Tue, 27 Jun 2023 02:31:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
