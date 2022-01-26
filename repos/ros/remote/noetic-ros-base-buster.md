## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:5ad7dc461716c49ba524307c74df5605df471b66356ca46996311139d625b49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:f289e65e384ac984d82fb032f56a6f95129aade492622c6f1b0a6a0e5b184f1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463263278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:903008d9ac6b3bdf3a598858fe90a23c9a9b461835734c25c70f8e972a09fcae`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:56:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 21 Dec 2021 23:56:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV LC_ALL=C.UTF-8
# Tue, 21 Dec 2021 23:56:21 GMT
ENV ROS_DISTRO=noetic
# Tue, 21 Dec 2021 23:57:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:57:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 21 Dec 2021 23:57:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 21 Dec 2021 23:57:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:58:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:58:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 21 Dec 2021 23:58:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a21eb75d0e3012979c6611472ad2ce77f9603178d355b33e3a29b873c09cd17`  
		Last Modified: Wed, 22 Dec 2021 00:03:48 GMT  
		Size: 10.9 MB (10891938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a0355b4bb6623abb06a5060650fda200f613e82ff0c1660f1dd412468468d`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428381b1469052a8549b56c928ac7628c4b0b3212ab6a0e15cd9a7cb0836f7cb`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb2dc8dfc87f5650375873e92661d1220cf0d1ef485c60f8350795669a60fb`  
		Last Modified: Wed, 22 Dec 2021 00:04:21 GMT  
		Size: 239.1 MB (239089267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5280b24f54ae8eeabff880a2eab6ce4c01ea397fe51e158a984ddcc9b1812a`  
		Last Modified: Wed, 22 Dec 2021 00:03:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384ffdd3a88cfad1dba9934a89583cde7175d36b67c35c33b81f4c51b4929654`  
		Last Modified: Wed, 22 Dec 2021 00:04:42 GMT  
		Size: 86.6 MB (86566404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e7347f2acf99a04e2a51ce3ab3a4fdf9b42d547819a739899ee16bd110ff06`  
		Last Modified: Wed, 22 Dec 2021 00:04:28 GMT  
		Size: 299.5 KB (299501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2bbb76c6ff423ad3e4b2298c17b2c64a171419f8c2c1ad315e018fcc912963`  
		Last Modified: Wed, 22 Dec 2021 00:04:40 GMT  
		Size: 76.0 MB (75976617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c93ca6155cb88a8496cea67ea2eeec68b6d4541e0fee83b1f301a84cc71a793d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.7 MB (402735896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7479069555b7b81015b03ef73244324cb06a7307c9b7be05520d892cb2b3c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:43:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:43:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 26 Jan 2022 07:43:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 26 Jan 2022 07:43:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:43:58 GMT
ENV LC_ALL=C.UTF-8
# Wed, 26 Jan 2022 07:43:59 GMT
ENV ROS_DISTRO=noetic
# Wed, 26 Jan 2022 07:45:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 26 Jan 2022 07:45:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 26 Jan 2022 07:45:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:45:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:45:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 26 Jan 2022 07:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646734dd4c9771207c4468eadc7ddcededd306975b1af9c589d4cdcda9b7c07b`  
		Last Modified: Wed, 26 Jan 2022 07:52:46 GMT  
		Size: 10.7 MB (10688073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aad39826b43f6faf1264f98a0a52a206ef90890c6834072d8d9f87d882868d`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8a7e03b40bfdb16508119c9ee410dd3684b3a5cf4bc31f5f6dd1597a12fee`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e34cb56b02431259e0ed70e5f2a62c5cbae86038cc51c240276d1c687014f`  
		Last Modified: Wed, 26 Jan 2022 07:53:15 GMT  
		Size: 184.3 MB (184306695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86270cb85ef2ff4c03d623ecfac134b2c9cc1bbd6a17a0d9a16eb961841ab45`  
		Last Modified: Wed, 26 Jan 2022 07:52:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead2d175559e1deb0533f1a26d062151a70ee020c83b271d672febcae2962201`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 84.4 MB (84350117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ee083a5f0a1bb7f96a6fa942a09843a7a85dd23f6c421fc1030cc2233c1fb0`  
		Last Modified: Wed, 26 Jan 2022 07:53:24 GMT  
		Size: 301.2 KB (301224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f310f444237727027c0400435c277b87c69c67df7b68e96da508934404d5a1`  
		Last Modified: Wed, 26 Jan 2022 07:53:34 GMT  
		Size: 73.9 MB (73864375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
