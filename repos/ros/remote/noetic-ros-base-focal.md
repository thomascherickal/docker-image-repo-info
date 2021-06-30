## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:3e6a35f079698f09470bf68987e85399dbe6a221322c375406b93dc8cc944e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:c9560582e17e8eed4a72bb18433d1e6f56b70d62513d307993c776bb886d1a78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334891393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950431941162e51c6aa584d795928655524e74288527c44ba2202809e19b0301`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:57:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:57:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:57:51 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 02:00:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:00:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 02:00:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 02:00:58 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:01:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:01:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 02:03:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2bdf44548ac5fc0e44b69348d2e10929673915bf3217b590b7535feaf9d95`  
		Last Modified: Fri, 18 Jun 2021 02:27:00 GMT  
		Size: 5.5 MB (5546913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b805325df4d3716458978c48a5566aa6f2dbeb0be999f44c7f2eb4f6df55e11`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64023780da8e71f6b88553fcffa3bc15bf627c1b1fc0aaf8ddc9af812128ec9`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d4726d161eb1b509db57b293c81ce05ceff9931bed70bd4faaa996412b4e`  
		Last Modified: Fri, 18 Jun 2021 02:27:39 GMT  
		Size: 173.3 MB (173312527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ea8650d58e6131af39d81de66161336ce9c8fc6fd3b3ef3430f6b0c2bda02`  
		Last Modified: Fri, 18 Jun 2021 02:26:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e80c4f5578a19f588ad6027bb260daf83091fb9f24409dd71d4d31ec276489`  
		Last Modified: Fri, 18 Jun 2021 02:27:59 GMT  
		Size: 46.4 MB (46383706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114571870237830af2427dc7692d57b06140899ae969d0c462a35df493e39dd`  
		Last Modified: Fri, 18 Jun 2021 02:27:50 GMT  
		Size: 307.2 KB (307182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a8de6086cf9af436698858140f30da4b4024f10b9f5270bf4b25bf77950f`  
		Last Modified: Fri, 18 Jun 2021 02:28:05 GMT  
		Size: 79.6 MB (79602485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:fde1ae78d99d46536c911daf516f6c0d73352c48869689cac97063169ad93d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285237237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949e9fedc86e0217b5840546b26cb295850dedb52e92f951e1b023ee1f278c0d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:53:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:53:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:53:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:53:39 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:53:40 GMT
ENV ROS_DISTRO=noetic
# Wed, 30 Jun 2021 02:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:03 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:56:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:56:04 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:56:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:56:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:57:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce5f21c6f106c12113dc525e925b89cc9535446d92c7075e4a662e3072cca`  
		Last Modified: Wed, 30 Jun 2021 03:19:33 GMT  
		Size: 1.2 MB (1183552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1bb638643e4649f6f3e64c7b898c73861a8ab112bfd3ad9236a4c6a87bc690`  
		Last Modified: Wed, 30 Jun 2021 03:19:32 GMT  
		Size: 4.7 MB (4676668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13d794ef85d45ee4aac8309697831cb2b0f9af19011b5b2ef60f87f4ff05f09`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9b321708870ed4300bbf05be9c67a4c34ac53de42cd768887724e4f5e45ab`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8659dd12dfc530e25e88a28dd63f72bb8245637129e2ecc91ab80e2b1dfe5b`  
		Last Modified: Wed, 30 Jun 2021 03:21:44 GMT  
		Size: 157.8 MB (157839188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c708ba5f097a8b0453d114dbae210814d65b70f3f79be22d745289e9739f3`  
		Last Modified: Wed, 30 Jun 2021 03:19:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5747898ddd1da4724961a6831f28bf8cd6501ca2eb50d17596f571470492c9`  
		Last Modified: Wed, 30 Jun 2021 03:22:18 GMT  
		Size: 36.7 MB (36691567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e07c5854ce6a7a7ced7b74f9e04fe8b5b798ff30fb7d03bd86b3f9198beaeb`  
		Last Modified: Wed, 30 Jun 2021 03:21:57 GMT  
		Size: 309.9 KB (309931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb478c4a9f1b7e6b34af4347c04a922ea45de5245a3ce46ca1fe73a4b58cd0b`  
		Last Modified: Wed, 30 Jun 2021 03:22:39 GMT  
		Size: 60.5 MB (60482175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2cacf86423c2c0975315fed27525f218224e20bd0872870472187b72b9577a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.6 MB (314579790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1e70451757ae814799c9bb72e863aa12b8011a49c6049366f2c86e7c86038c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:16:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:16:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:16:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:17:00 GMT
ENV ROS_DISTRO=noetic
# Fri, 18 Jun 2021 01:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:17:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:17:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:17:48 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:18:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:18:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c561e77a6581855b0d4bcc7b9679a0821de33d9475c1aafa35306fd01018cc`  
		Last Modified: Fri, 18 Jun 2021 01:36:32 GMT  
		Size: 1.2 MB (1183649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b8cb9206c66daa80abb822d79f1304b0788918a2f9ba31628d947338478acc`  
		Last Modified: Fri, 18 Jun 2021 01:36:30 GMT  
		Size: 5.5 MB (5512873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221feb81eb1f2a726e60f133308042f938d56c17d93bb58e579331ac82db4361`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e854a63e407af8a98ce9423f465f741b1391622ab778b194ffdd73b401d1f09`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31e769dc6dc1b2825400e8c4f1f822c2f6793a851ccb1f5befc9d365546b54f`  
		Last Modified: Fri, 18 Jun 2021 01:37:09 GMT  
		Size: 167.8 MB (167791425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b59e42fab796f88f9034141f4ef8b681764faa78cdcdd15e6fcc841e712c7`  
		Last Modified: Fri, 18 Jun 2021 01:36:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d19dcde6b5d00235d5458675c834b27246ded78afbcafd52415832b238c527`  
		Last Modified: Fri, 18 Jun 2021 01:37:28 GMT  
		Size: 40.7 MB (40650604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55e8737df32cfb68aef8faf31c80e8a806987bdcb9b01ea2c40c56f0261092`  
		Last Modified: Fri, 18 Jun 2021 01:37:21 GMT  
		Size: 307.2 KB (307169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80366f56b9dfbc22e74d7236626b43457126c0b3a4021691dbf536679e15f025`  
		Last Modified: Fri, 18 Jun 2021 01:37:34 GMT  
		Size: 72.0 MB (71972855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
