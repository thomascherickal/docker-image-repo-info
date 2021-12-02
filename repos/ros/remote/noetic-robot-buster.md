## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:63bc11974a1a57775aba120d7420d73cd3191d581130b995166b4f567084c4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:2d846916bb0383759f01489d06f1dd884fc933665df95bb6975ade4d93994a92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.5 MB (484506857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b440e63083c21cf88e00b7240dafcaa399827e9f41b8eaf1204cb538685d393`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 22:36:22 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:36:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Nov 2021 22:36:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Nov 2021 22:36:28 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 22:36:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Nov 2021 22:36:29 GMT
ENV ROS_DISTRO=noetic
# Wed, 17 Nov 2021 22:37:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:37:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Nov 2021 22:37:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Nov 2021 22:37:37 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 22:38:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:38:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Nov 2021 22:38:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 22:39:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f64a2cee9a8973db7ffaff43c62f68f0db43144b718c8339856ff2d039b430`  
		Last Modified: Wed, 17 Nov 2021 22:43:20 GMT  
		Size: 10.9 MB (10891910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d367fa9b39ce393432a2a974cff50cc6c0a295b0c00a6a71152b947621dfd2`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54972089aecf2d558033d5c01eb20f1a2fc64c872aca23ad9ab78f45f335f6e4`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d68c1a3d9a31ff02e5ed0caf544e9e047643eeaa48073c11c2aff158e93739`  
		Last Modified: Wed, 17 Nov 2021 22:43:56 GMT  
		Size: 239.1 MB (239087074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb488c1f6198579f8b779a8d04bba2ad192ec739f12e0996b08295f67e238be`  
		Last Modified: Wed, 17 Nov 2021 22:43:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95ec5664844d6b0b37d4f1fb00c8c3471f9ed1c9279b982e28e0bc5187c5d32`  
		Last Modified: Wed, 17 Nov 2021 22:44:18 GMT  
		Size: 86.6 MB (86566518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015f591fef24508ee575fa1a04719eedace93ecc69747c634ee129ab56e7afaf`  
		Last Modified: Wed, 17 Nov 2021 22:44:04 GMT  
		Size: 319.7 KB (319667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfb467cccf362fae16d482dedbaa84f68b710a3551e876a27d306cf8487b62`  
		Last Modified: Wed, 17 Nov 2021 22:44:16 GMT  
		Size: 76.0 MB (75976988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bb79def2eadb38d0deda1648bfb3ab04c5a950348eb0070e656d58887f98d1`  
		Last Modified: Wed, 17 Nov 2021 22:44:28 GMT  
		Size: 21.2 MB (21225186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:92f97070d120ab647b181921e2021caf7037c08a1ff550cd4c30cc5a8e49f049
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.6 MB (423621432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a95b640c4f46733eaaee4baf622dfa87af9aeeb2b028f068629f16f75751b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:09:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:09:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Dec 2021 14:09:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Dec 2021 14:09:49 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 14:09:50 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Dec 2021 14:09:51 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Dec 2021 14:10:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:10:56 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 02 Dec 2021 14:10:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Dec 2021 14:10:59 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:11:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:11:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Dec 2021 14:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e8f1f129dad6b169099626334d47f33bb82f4b4bb0546404f0e3ff9f29f589`  
		Last Modified: Thu, 02 Dec 2021 14:18:09 GMT  
		Size: 10.7 MB (10688015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a995ef6e0affa0efea1e9bab7ccb010f6b50dc0dd518f955224c42c80ca4625`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1a144f0e750af7280088604a588b33ca097d137deb1e9c165832bcc112ff12`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ff02a2b334915606915d72debb67ed7feaef6ab150ded7a474ed2a3847bab`  
		Last Modified: Thu, 02 Dec 2021 14:18:39 GMT  
		Size: 184.3 MB (184301599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4546300f0a7a750dcd6fdf3c875bbd66d4444983e525a6fab1105911104a496`  
		Last Modified: Thu, 02 Dec 2021 14:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce39833a554c81bc87396258be276032a0ac4732244ec5b32a4db5d81608ab`  
		Last Modified: Thu, 02 Dec 2021 14:18:58 GMT  
		Size: 84.4 MB (84350775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd88b221d2886e01923a8b183f4b803fb4ec24678841cd7286b5923f1e4a83`  
		Last Modified: Thu, 02 Dec 2021 14:18:47 GMT  
		Size: 296.7 KB (296670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49acb51cc416043d32385bf010918894706381ff1599d620af1262072a9e0edf`  
		Last Modified: Thu, 02 Dec 2021 14:18:57 GMT  
		Size: 73.9 MB (73864403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092f09e5b404488b9ae275db31f70f12a33ccb6728f552fc9f9c409acda3c21`  
		Last Modified: Thu, 02 Dec 2021 14:19:09 GMT  
		Size: 20.9 MB (20894555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
