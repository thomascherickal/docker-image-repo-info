## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:09ce859b0e19f4123ba5ae2b278569b727bb4f9ab51a0933522b9f5ff1780b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:842dd332d217fb00330baef47ea597cefa08d1a80d2f1fa4bb02867750dab41b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141464961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b18dae841afdea295a3062214602f2694f104082135a307643b749068571096`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:16:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 02:16:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:16:53 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:16:53 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 02:16:53 GMT
ENV ROS_DISTRO=rolling
# Sat, 30 Apr 2022 02:18:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:18:35 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 02:18:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 02:18:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5d137ac3f4107166acc832d7edffb774a28a3a16ca4f1fbe1b4f3653c8824d`  
		Last Modified: Sat, 30 Apr 2022 02:29:07 GMT  
		Size: 1.2 MB (1191214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f742e0a4361e52c84f1a27d4d57685a19b201687e97de11e8308e3919dc6`  
		Last Modified: Sat, 30 Apr 2022 02:29:05 GMT  
		Size: 3.8 MB (3826919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de85e82a503b9baeed214acd1421f6eac09e02419926d5eb1ae3fd6863bb7a5c`  
		Last Modified: Sat, 30 Apr 2022 02:29:04 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d5c725f3312c7dd56c39d5af65304e67e94a82e1af69a06d8394c0d4f16be1`  
		Last Modified: Sat, 30 Apr 2022 02:29:04 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d31a21b45d6f0e10d726bc6c1f481fcf23761a65ea402b6a0e9267fd5cdf56`  
		Last Modified: Sat, 30 Apr 2022 02:29:21 GMT  
		Size: 106.0 MB (106023409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a3989c09346a5a894f45db69686559c0b440d5ccfb1bb9288f4bde7c9ab693`  
		Last Modified: Sat, 30 Apr 2022 02:29:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fbdfb4cc6c578f26264bd25d1f0dee739ebf7c799a6051764b6982e235e92f0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.9 MB (136939071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939b7344405c1ba5f1bad7ee3277b1574d8adec1f2eb8b1b7f26b50344646ed2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:32:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:32:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:32:29 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:32:30 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:32:31 GMT
ENV ROS_DISTRO=rolling
# Sat, 30 Apr 2022 00:33:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:33:19 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 00:33:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:33:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4339dcf07e4fd919aa10dc0e01fb8f44184f74bf6baf5aef6e8fdd30f5e603`  
		Last Modified: Sat, 30 Apr 2022 00:43:58 GMT  
		Size: 1.2 MB (1192681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0db3fdf5b04e561797500fc1d19d79a37ca0586b71bee71ce2acaee153d4dee`  
		Last Modified: Sat, 30 Apr 2022 00:43:56 GMT  
		Size: 3.6 MB (3594435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af71d8cd404a31e077722270696cf33d59cff54d35c9dad864264138bc3ac`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e01b1250d40bc108a995e5fc6c1630b0abdbfff31529a87a4096271f2a6115`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ae3a3b720aed16343416b9bb5eea4967087c21dee2c39948d0ca129037dd4f`  
		Last Modified: Sat, 30 Apr 2022 00:44:12 GMT  
		Size: 103.8 MB (103773129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be65bd445679ba8af650c6dd6742dc9a2d31871d4bac42819d92857e3a5892d`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
