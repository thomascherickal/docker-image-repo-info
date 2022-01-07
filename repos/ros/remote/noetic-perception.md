## `ros:noetic-perception`

```console
$ docker pull ros@sha256:0c7f8ff67f8ba3997601c3023352dd5c3143717282f876a81b899620f31866ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:ae7a9381ec90cabd6293626b4d4dc7a7c3a2928b05d259df1398e749a767f310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **830.5 MB (830492053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e4a30e7a04b988ce6dd6d676724f1d468aaee1c114880010b2491af6e0c814`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:09:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 04:09:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 04:09:27 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 04:12:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 04:12:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 04:12:09 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:12:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:12:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 04:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:22:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f179e9829abe90277c32bc8a0ae588e6e8cc1695c6fc68725929e756102e57`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 5.5 MB (5546941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c70e9658293d6c6994b6a7c4cdaa6377ff6c88e8aacb0cc925a437b7f64d`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b560e1d79dbdd0e1849bd0bf9e744605e7fac17d52d9eae6a2eb85191f795c`  
		Last Modified: Fri, 07 Jan 2022 04:34:46 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19690a1594bd61dff284097ca83119bb45eb8440545c32da4c0922132b07a310`  
		Last Modified: Fri, 07 Jan 2022 04:35:27 GMT  
		Size: 176.9 MB (176882711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f25217df1dd04bb397f3964b212a7132b0589c74df28014755ac8a8242d39`  
		Last Modified: Fri, 07 Jan 2022 04:34:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ffdfe95d3dd2037023009ce14081cded135d4297f961ccfeefd666265cc7a`  
		Last Modified: Fri, 07 Jan 2022 04:35:51 GMT  
		Size: 47.3 MB (47259832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460a4cc48907ba7a3f48875ff90081588a2252332a03cd88eaa72be2ae16c0`  
		Last Modified: Fri, 07 Jan 2022 04:35:43 GMT  
		Size: 305.2 KB (305157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406044e053161a2f909c8a24c374019c518eb7ecc7541ad0de4b194271415c57`  
		Last Modified: Fri, 07 Jan 2022 04:35:55 GMT  
		Size: 79.6 MB (79602648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1ce7466821e5a5d0e3561de4e5a4cc3a4aa853d74586fa50d9c8fe7ac4bbe3`  
		Last Modified: Fri, 07 Jan 2022 04:37:32 GMT  
		Size: 491.1 MB (491143690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:7c6c88a1d0bb98f2392fd70c79935ee6767576383924a1a13fbbb4d36922a4f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **721.1 MB (721109316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6028632106c6e4cb54ec03431de5a4e7ca6cd0ab5f3cfd24dc29340ef38c668f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 02:26:25 GMT
ADD file:ac83e0dc7e48a0dc1805c0fd7b71b8eb119b3eeafd1fdcab93e11fbc9c0bcda0 in / 
# Fri, 07 Jan 2022 02:26:26 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:53:03 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:53:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:53:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:53:38 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:53:39 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:56:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:56:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:56:18 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:56:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:57:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:58:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 04:04:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b8080fa0945580f29aa3abed4664f8ab849229eca04510b5d259a9e29616064`  
		Last Modified: Fri, 07 Jan 2022 02:30:39 GMT  
		Size: 24.1 MB (24064434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542f65e85cdaf2541613579d209e8ddfa8b797d8edd23c4b1b3e430580dfb8c`  
		Last Modified: Fri, 07 Jan 2022 04:13:02 GMT  
		Size: 1.2 MB (1183516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc20ad2d3acd4173d1357bb75d2d434c2cf628930746de1b638775ce5b3f169`  
		Last Modified: Fri, 07 Jan 2022 04:13:01 GMT  
		Size: 4.7 MB (4676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038a958a9812e6ad8943ca985ee5fc0fa712bd2bb652825668f1e805642250bb`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14895cbe261aa62a0bacb72a62e26758d9c4917efcc5e712fc9f8a815cc2b2df`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05603c4fd7f49169b1f830d906412ac1eb62f339ab3b8518b04e0d0df814b72`  
		Last Modified: Fri, 07 Jan 2022 04:15:07 GMT  
		Size: 157.4 MB (157422125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4937926a5187427a5b557119d517c0cb7b07dd1ec423d7aa471bbf95e1fcfe8`  
		Last Modified: Fri, 07 Jan 2022 04:12:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c707c45473b692c29e259d0c26776db6360563b1a2d369a2e46e30f9e6f053`  
		Last Modified: Fri, 07 Jan 2022 04:15:41 GMT  
		Size: 36.7 MB (36693115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4d7df5c0cc0093b02360bb46f1cf1e7f633acd03cf4ce2cc15d489a0039acb`  
		Last Modified: Fri, 07 Jan 2022 04:15:22 GMT  
		Size: 305.2 KB (305155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9129d7514384ec5dc914d6cc465ffc40283fc596a024219bbd74ecb6ecf66c50`  
		Last Modified: Fri, 07 Jan 2022 04:16:01 GMT  
		Size: 60.5 MB (60482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717ce4b02e355c16404348953d4d926519f98473bccc7cb58ac5c30b8e18b3c7`  
		Last Modified: Fri, 07 Jan 2022 04:21:08 GMT  
		Size: 436.3 MB (436279449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:eb5d4d883e52520819da468f310545e580d9b8d063f73e8573f3addd710ae069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **780.1 MB (780106767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9a0b5f335bd160a4a319a25f1c844783f88048a4d4b6b03841d19e16757cb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:15:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 07 Jan 2022 03:16:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 07 Jan 2022 03:16:02 GMT
ENV LANG=C.UTF-8
# Fri, 07 Jan 2022 03:16:03 GMT
ENV LC_ALL=C.UTF-8
# Fri, 07 Jan 2022 03:16:04 GMT
ENV ROS_DISTRO=noetic
# Fri, 07 Jan 2022 03:17:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:05 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 07 Jan 2022 03:17:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 07 Jan 2022 03:17:08 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:17:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 07 Jan 2022 03:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b5c31769a3e9a4ae40d97f3d7edbb0e388c814d495803544ea752c6e9d6ce`  
		Last Modified: Fri, 07 Jan 2022 03:35:30 GMT  
		Size: 1.2 MB (1184196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94701350f1a3f3c228c3daa7b1471a93f50e71219e0bf9152dedc5131dbdc27`  
		Last Modified: Fri, 07 Jan 2022 03:35:28 GMT  
		Size: 5.3 MB (5322571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3843c054baee6fdbb1122ab1ef12464d44642d23fcccbdf9dcb77a02e41bfc7a`  
		Last Modified: Fri, 07 Jan 2022 03:35:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f924ca980605e9e62baf57692a5657c36e9189d8794573f729f971c5ed32bb`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0b0eece4cf7bea41c5acd111a551c273d6e153407fcc2744b14a155e05366b`  
		Last Modified: Fri, 07 Jan 2022 03:35:57 GMT  
		Size: 171.3 MB (171326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a972d654bf4928ae873620e2c0012b7fb3d477f39d368d27ad70a7083fd8a2`  
		Last Modified: Fri, 07 Jan 2022 03:35:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978c5c6ccf265e99aa4eafe327bc1a79aca0405c567834589c5f2eb1f4a7da`  
		Last Modified: Fri, 07 Jan 2022 03:36:15 GMT  
		Size: 41.3 MB (41306233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5587d30d9aed449ad7397931e249b18f034edf5cc07d2ee00610e1972a388f9a`  
		Last Modified: Fri, 07 Jan 2022 03:36:09 GMT  
		Size: 305.1 KB (305107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814684186464d45ad335516ea3732d0f22a6b4c201319d425fd6324ba9a5e67`  
		Last Modified: Fri, 07 Jan 2022 03:36:19 GMT  
		Size: 71.8 MB (71753993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce42ea2594c2658568488e507dbab59fc44b7afbf9177364a2502ca7a4e60d`  
		Last Modified: Fri, 07 Jan 2022 03:37:57 GMT  
		Size: 461.7 MB (461735208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
