## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:ae066a7092dacf493d8d96af7d016797eb4ea50fb7658b4dacc2b32161ddeb05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:12474f93b72af1d2a90ffd3a83465c2d7fc062f71e1bbd8219a4fbfd9465445f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291976007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79acfd9a4048a562c4c833120a1741045623180f05bccd1f022b9196a1f31802`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:57:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:57:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 12:57:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 12:57:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 12:57:48 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 12:57:48 GMT
ENV ROS_DISTRO=melodic
# Tue, 02 Aug 2022 13:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:01:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 02 Aug 2022 13:01:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:01:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa6fbe30fbafa2fd890f1a634056fab84382d475fe85716949a1a44cc77f087`  
		Last Modified: Tue, 02 Aug 2022 13:52:33 GMT  
		Size: 839.1 KB (839126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d6485ffdcfd34d9790c5e9f1e3deb6f1e01cd88b3ed1c2c4bfd798ce679c6`  
		Last Modified: Tue, 02 Aug 2022 13:52:31 GMT  
		Size: 4.9 MB (4873542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d651da90ea517b4e41ab1754a0657cd17842014153817571fad7f62a21dd8`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8310f03235adb2a56f2ca99fcd6f4bf9c29d94663f625b160ef3534ffc2630bc`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f613727d0890c231f392123401bfc2194872d710cd8d8a8740db383fc8a599f4`  
		Last Modified: Tue, 02 Aug 2022 13:53:17 GMT  
		Size: 259.6 MB (259551224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ab03995e2e9bff9b259a370e6c30525ec9bc8cb87b98f29e3d3de46a99b36e`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d4a0131748a7ffb924a003845b10921ddd3f5d963a6cf71d497c3851b7e94fc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266181333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f444660baa7a35fb7cadcf6ccdcea8d9e4436dbba5c800cf8304c755244cd158`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:07:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:07:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:07:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:07:59 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:08:00 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 10:11:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 22:58:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 22:58:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 22:58:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddc7f6bb12de3f6e55c81fc14d7ebc77e5e7612bd09a2770d4cf1feae55f3d6`  
		Last Modified: Tue, 07 Jun 2022 10:32:01 GMT  
		Size: 840.2 KB (840219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc3e315dd2fd37157023b5350340af87fe236f4bcd29db3284eb3e86c37c85`  
		Last Modified: Tue, 07 Jun 2022 10:32:00 GMT  
		Size: 4.1 MB (4089918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b851bde5be9d93cd5bf76737b14ccdf776ace9a4d8ed7b1e11b042c22452a1`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883aed8a39d8c90c486aec03c1809aa36c891e812219cf617b59ece7f9165291`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd559c545cdb93ee204c62144d4375db3f0450040d3ef61a8ac599ffb1f043a1`  
		Last Modified: Tue, 07 Jun 2022 10:34:31 GMT  
		Size: 238.9 MB (238943066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6affb1b3206339bc5b43342d1c9945b174998df8674effb3cfb95da2c03bd8f9`  
		Last Modified: Mon, 11 Jul 2022 23:15:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c328dc0017ebf84de901c8af6dc983fcd8836e90337a60bd939ce59d23423fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281232232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be79d1120f2efaf731e5b68ac3a5faa39387620497b18f9e806d0ec0694f276c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:47:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:47:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:47:50 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:47:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:47:52 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 05:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:44:07 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 23:44:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:44:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b57592ad601b709b6d4af02430444d1ce166e53a2c06e41b70d06e27b5ec2d`  
		Last Modified: Tue, 07 Jun 2022 06:15:41 GMT  
		Size: 839.7 KB (839692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352bdaee988c61b20b656df8008d4be213733165c725560536714f21e8cf2ad2`  
		Last Modified: Tue, 07 Jun 2022 06:15:39 GMT  
		Size: 4.3 MB (4268418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e95ee74d62367ac78bdf552d35893b1bfa0b8538f69894f4ca7d5c558975e79`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0702606dc329e1f145eeaad6f2f9524dc0917eb5ba25853c54f2e8025773e2`  
		Last Modified: Tue, 07 Jun 2022 06:15:38 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025651dc59757e03c16f059d8f61cb6a4f6ba0e81af77f6ad318d2bd7e0722fb`  
		Last Modified: Tue, 07 Jun 2022 06:16:14 GMT  
		Size: 252.4 MB (252387652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec0035a4765f4a1f16c48462fac335ce0511ec4e712ab4bb067d948b16ea7d8`  
		Last Modified: Tue, 12 Jul 2022 00:10:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
