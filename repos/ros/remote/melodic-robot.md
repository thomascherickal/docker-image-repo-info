## `ros:melodic-robot`

```console
$ docker pull ros@sha256:8fb5d5ae193f0e00ae7b88a0b8b8574bba37d5b182d666d5aace3784c2864e97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:4f77b7983751f82229d2167f2601f19ea9dfed600d2add2e4e62144f401f0dcc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448429857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7534e98061854591891289aacefbe4665c302c0e18eb2b95c9b92f7a99f3a9b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d3de5e357728022b59ffac5d209fb766dabf58ab4d6ca073e371d82256056e`  
		Last Modified: Wed, 14 Jul 2021 02:30:52 GMT  
		Size: 11.1 MB (11077547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:61e98cbf3268458279d81c99b2242d25879e5abe6c39488bb5e71de2c2b92a1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395994921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79342d85c4ffce61a75fa2d3cbbfee3317b043c12b2543231fd968b32da4cec0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f163f6facf7915ed1361c02ce023903ec332843f27d78246993b5bf15fe0efb`  
		Last Modified: Wed, 14 Jul 2021 01:15:46 GMT  
		Size: 10.1 MB (10120489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bcd6dbc4c225ebbe65b2a969eb95f9197b3c3af9c5c59935cde8b859c1f591b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422669461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b895d9e92f835cb0cb94a210aa510ab0f274f2163a3643c010678ff169b563e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:26:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:26:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:26:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:26:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:26:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:27:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:27:41 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:28:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:28:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:28:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41769627f180322e716b3023e5ef1ae59239c5ec3ba63d3feb96951d73d5878`  
		Last Modified: Wed, 14 Jul 2021 00:47:53 GMT  
		Size: 841.3 KB (841282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63f135f6f4db75ebf1ed14bf2422b3e612ec51db4bc3162a3a75a8b8df7b1b`  
		Last Modified: Wed, 14 Jul 2021 00:47:51 GMT  
		Size: 4.5 MB (4453635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3d85ee829fbd9be39df324330a8fe50c97a4b0c1247389b35c752404e77956`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c861f823f51f0edd135ae9cfa7425e5069eee2dc8641b3295ac532e11f81a`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0bc4e6e6bc21814066b9ec7467ea608909aead56aaf7d7f6972cc89eefea9f`  
		Last Modified: Wed, 14 Jul 2021 00:48:44 GMT  
		Size: 252.4 MB (252361492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767e94dd377ecd0bbcfb7093ad56d12b9939dcd7e13e05dd7670d173f21a2c5`  
		Last Modified: Wed, 14 Jul 2021 00:47:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757b61452d8eae6c89294b87e561cbfba03e0e55970cafa498482560fb4b149c`  
		Last Modified: Wed, 14 Jul 2021 00:49:13 GMT  
		Size: 63.1 MB (63057473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ae03f3e351dc5e7ad9a7a7326828f929507da72882680dde4eb7b4b257d66a`  
		Last Modified: Wed, 14 Jul 2021 00:49:03 GMT  
		Size: 269.6 KB (269565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd788c193bc11dec6b0622c8def99e36c29b17a5c68360cc67bca0a52b5d74`  
		Last Modified: Wed, 14 Jul 2021 00:49:18 GMT  
		Size: 67.2 MB (67222233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0073605ff6b06de0753d62a4d3f35f3df0d0a298ab337cca5b9e16c8f832543`  
		Last Modified: Wed, 14 Jul 2021 00:49:39 GMT  
		Size: 10.7 MB (10731868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
