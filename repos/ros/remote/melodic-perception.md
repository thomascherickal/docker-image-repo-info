## `ros:melodic-perception`

```console
$ docker pull ros@sha256:115ab5f5f161e764ec7b03ce10ca88f7b661254974275efd330e539d4113af4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:f3bb12938726ef959ceb40850475e5f1dcd7d482a9077c3c7e442896abf8f9bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742712938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2bf826514bce311c7072e360d4817decc828157256ba044fd82daaa772863d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:29:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:50:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:50:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 01:50:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 01:50:17 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 01:50:17 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 01:50:17 GMT
ENV ROS_DISTRO=melodic
# Sat, 30 Apr 2022 01:52:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:52:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 01:52:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 01:52:55 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:53:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:53:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c6e4dbac2549834f9ff8126148bc819d27a613ba3783701cdafd265b966467`  
		Last Modified: Sat, 30 Apr 2022 00:47:48 GMT  
		Size: 839.0 KB (839025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97750bfec14ebe2ac09d3d8401c48f6689d33bd9e3776dcd77c16866e8b1e`  
		Last Modified: Sat, 30 Apr 2022 02:21:21 GMT  
		Size: 4.9 MB (4872315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82b533a056ad3d5f39043b0e0cac00952c22926b3fc062cbc57a213b59738c6`  
		Last Modified: Sat, 30 Apr 2022 02:21:20 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22c7cc428a638fe1a1a9cafcb40081713643062dc270ebf1337aa25f4b43795`  
		Last Modified: Sat, 30 Apr 2022 02:21:20 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739fe81fc30f4c76813c7537f2e12ef342f058d376c52b590983f80f20054191`  
		Last Modified: Sat, 30 Apr 2022 02:21:55 GMT  
		Size: 259.5 MB (259454842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9455a270bd5c7a726fb011d30284d87cc7b6cfcd14a04c735b5812d8a95ed4fd`  
		Last Modified: Sat, 30 Apr 2022 02:21:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea826bf6a039027845f5ad9234a15f787c8d26737b6c9bd63ce1cb7a27355d94`  
		Last Modified: Sat, 30 Apr 2022 02:22:15 GMT  
		Size: 70.2 MB (70244494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb9465c7cbf4fe34a39aa2a32bebcffb89420d392d040b130a57babc7ab2239`  
		Last Modified: Sat, 30 Apr 2022 02:22:05 GMT  
		Size: 280.0 KB (279969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cf4eeaa107a0a2e0fd53dd924322b54ac8e758607d35e2764a466912a04bd9`  
		Last Modified: Sat, 30 Apr 2022 02:22:17 GMT  
		Size: 75.0 MB (74994845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55317f21e3a1712e80a5ff6a1baa0d201d28c374a56543cc1c694abce13209fe`  
		Last Modified: Sat, 30 Apr 2022 02:23:33 GMT  
		Size: 305.3 MB (305315927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:cd396be2ca46cd7dfcde32f48d42a211db6e312784912e3628744900d6b0c2b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645946166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:859f432cda36e5a6f96e8a2d4597ec613a7e4cb99907a711467d08e775f9e5a5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:28:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:28:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:28:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 00:28:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:28:41 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:28:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:28:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 30 Apr 2022 00:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:31:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 00:31:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:31:55 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:32:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:33:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:34:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57ab3231e4fbaccf7df6d1d44ef88608a6c1b716de9810c8e2ad6b7dcc9f5fc`  
		Last Modified: Sat, 30 Apr 2022 00:51:07 GMT  
		Size: 840.2 KB (840158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f529e0e8ed7433413f39308a48052c609e82179d4d22b76f62189c616e5fe14`  
		Last Modified: Sat, 30 Apr 2022 00:51:07 GMT  
		Size: 4.1 MB (4086200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59f023c86c2016dd149f7a89f71dc59cb35eeaf64c75eadba638336b28f6abd`  
		Last Modified: Sat, 30 Apr 2022 00:51:05 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdf654803a8e788e4166c4bf287b5137ec541b313ce50e4d9401f0bd63fc8d`  
		Last Modified: Sat, 30 Apr 2022 00:51:05 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa17f883dcf2090ca188521c82e8ecd78e6182c5c0af353b2dee9a1b0e0c44e`  
		Last Modified: Sat, 30 Apr 2022 00:53:38 GMT  
		Size: 238.9 MB (238937435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27e0b0ee020522ab3317cb8094bd430e3fb49425c99d1cfafe5284f0562f68`  
		Last Modified: Sat, 30 Apr 2022 00:51:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c89127f2ab55d40e6d39537412903ef429801ea54d6baf3a6439a6bb01692f0`  
		Last Modified: Sat, 30 Apr 2022 00:54:21 GMT  
		Size: 54.7 MB (54710630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108adfc0916db7aeda7a39615caa2cee9b6fbe75cd66aa27a2ac82eaf1e6e9b9`  
		Last Modified: Sat, 30 Apr 2022 00:53:50 GMT  
		Size: 280.0 KB (279967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ab1dc1feb0f323edf28a08fb0fcfc3796eb524ac698714b37837180467e312`  
		Last Modified: Sat, 30 Apr 2022 00:54:36 GMT  
		Size: 64.7 MB (64746523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d75072f0ae1c4ebd364e5b399abd459ffbe79508b5305949c7e203edd68958e`  
		Last Modified: Sat, 30 Apr 2022 00:57:57 GMT  
		Size: 260.0 MB (260042387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ca807f065cfad860bd04db915ee044c80c79ad8c20e9cae96a25a022007580ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (702991669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca9aa4207c71c21c1033211abdbac9667291fac2ddc21690b6bcc11f58379cf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:15:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:15:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:15:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 00:15:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:15:31 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:15:32 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:15:33 GMT
ENV ROS_DISTRO=melodic
# Sat, 30 Apr 2022 00:16:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:16:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 00:16:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:17:00 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:17:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:17:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:18:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9119a950b820c04a3c9309fd9cd748b4a1c924ef00ac90dcd01791d857977923`  
		Last Modified: Sat, 30 Apr 2022 00:35:56 GMT  
		Size: 839.8 KB (839766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54865980d811f13a848975797615c6b0c5f21fed029eb255b5a1b3a0566900ec`  
		Last Modified: Sat, 30 Apr 2022 00:35:55 GMT  
		Size: 4.3 MB (4264191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d745fee38250cce36d1723e6eb3964a525bb738eb2c82b501244732a881913`  
		Last Modified: Sat, 30 Apr 2022 00:35:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbae97ea1f2eea13534851ba6f58745635c465f6dd61681051632a7cac4bc8c`  
		Last Modified: Sat, 30 Apr 2022 00:35:54 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccf8a195bad2001e20b085a797b257c60b2e4020d738441e352b661525e5029`  
		Last Modified: Sat, 30 Apr 2022 00:36:30 GMT  
		Size: 252.4 MB (252383482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4c7449338629d393daa386d56eda7c00568a57dd328cd7df0410b5e398458d`  
		Last Modified: Sat, 30 Apr 2022 00:35:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9440733505277e8f3f7d4bc2ad385b06e37093582b77feeef90fbf8570dddf3c`  
		Last Modified: Sat, 30 Apr 2022 00:36:51 GMT  
		Size: 63.1 MB (63076164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8b76e35d4800cba2ffd96b6e5766991c5f6f8df302a89558162e2756996fac`  
		Last Modified: Sat, 30 Apr 2022 00:36:42 GMT  
		Size: 279.9 KB (279913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240a0f2f7118df62260d84e096be2a18536d017cef9a31f1ecdb65a6c2608eed`  
		Last Modified: Sat, 30 Apr 2022 00:36:53 GMT  
		Size: 67.0 MB (67001910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dea0e3098d641876fd5b669fc706eb09153bbfc9a9965819f7887cd6e57416`  
		Last Modified: Sat, 30 Apr 2022 00:38:05 GMT  
		Size: 291.4 MB (291408787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
