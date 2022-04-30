## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:34fd1d3019dd741f76daf20cb08ef1fe7dbf444eaaf46af1cf16533c0ae5f1a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b52870fad6fa4e6f253742250dc2853588e3acbd0effdaff267e59e027971459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291877703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c24685eafb1855f4a9b6f54373512077d8cb2714166e101bff032dc9e8ff72`
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

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:acf689ff37ed4dca35a9ec4f405a80509c2ad86a4a8ed564049ca49476567f19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266166659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd942724ced67c41e9e3a662aad99a1ecc5b0d8b27170dce8a888bb6fc63e01`
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

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f80bd2021f4064e73fa6c8288e28e79addf215f802688837c08c207a8391edae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281224895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f5d03985df014cb9760c418e73f445759afa99fac7fa0c6bb83780b33d83ae`
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
