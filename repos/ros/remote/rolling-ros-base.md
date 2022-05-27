## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:2559c202d253757770655f00b50a55dd785cebbf7483ade1f6d02501d0b52ad8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:8ec7644738b52d23f63d169cc53105352558757433095c4361539c080982a7ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.6 MB (263594785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176e46adf99710d4fe16aea9578bf3f317b5cf394e08c42dcbae6cfe3c92fed8`
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
# Sat, 30 Apr 2022 02:19:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 02:19:46 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 30 Apr 2022 02:20:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8b2c839950e5aad8d8c6bde76bfe949fe19894336e8a3b667618817614680915`  
		Last Modified: Sat, 30 Apr 2022 02:29:44 GMT  
		Size: 98.8 MB (98771070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305711873b5971c3e7f1d23f9a7a60a4f27793eaf8e52917b82d5387cb8afac9`  
		Last Modified: Sat, 30 Apr 2022 02:29:31 GMT  
		Size: 269.8 KB (269815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b026e225a8e2e8b023dc64c56eeb0a2c97a0b8a477cb787f6d0ed29c20f8f7`  
		Last Modified: Sat, 30 Apr 2022 02:29:31 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38e2e7098e2788af6746af593e775f066a530906007fa2931cddecc720e4508`  
		Last Modified: Sat, 30 Apr 2022 02:29:34 GMT  
		Size: 23.1 MB (23086729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b8f9f5f7d780bb6fa5a46e03b049d3eaf125128d96f0cefbc19085dfeced544e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257494582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5341bd45c056deaab818656b22a4f6be407b12332cff43de93b6fbe7e5b730df`
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
# Fri, 27 May 2022 00:01:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 27 May 2022 00:01:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 27 May 2022 00:01:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 27 May 2022 00:01:52 GMT
CMD ["bash"]
# Fri, 27 May 2022 00:02:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 27 May 2022 00:02:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 27 May 2022 00:02:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 27 May 2022 00:03:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:cb42783cc3927279718097f695acb188af7247f4635771cc2e94fd788d4b0118`  
		Last Modified: Fri, 27 May 2022 00:10:41 GMT  
		Size: 106.4 MB (106386146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c9f41ded8565c1f327636498d36859881d62a32bdc9dff5b92e047d59012dd`  
		Last Modified: Fri, 27 May 2022 00:10:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de34af377d115902131c5b5ca87d21c9fffb69370e16847717d2e1a2a40bd4`  
		Last Modified: Fri, 27 May 2022 00:11:07 GMT  
		Size: 95.2 MB (95224066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ff29b8d2944a451a664aa964b37ab3dae63c3ea232467461df0af1282e4e8`  
		Last Modified: Fri, 27 May 2022 00:10:53 GMT  
		Size: 271.5 KB (271498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ba5086e791ab84c3886a744c998db4d34535d380f06dea5be896569e00b76`  
		Last Modified: Fri, 27 May 2022 00:10:53 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736e7996fb31e59ebb99c1d6d574b039f8d52c9d6e1e6a665c4f3e7ca7ff604d`  
		Last Modified: Fri, 27 May 2022 00:10:57 GMT  
		Size: 22.4 MB (22444755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
