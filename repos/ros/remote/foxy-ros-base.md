## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:6e776f1a869bccaee01cbd2397a6b9c74499f5ffca2e995b5ac6a1b894aefd56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:add9970136f8920882152f611577326f7e23b0ef9a7069b8152de089ee9ac730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250620496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208eebb028dc4838ab0afc9b35e3de393855272172cdf1748b12e3c6704fe16`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:03:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:30:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:42:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:42:19 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 04:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 04:43:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:43:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:43:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:43:57 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf19bc0e0d1d8bf1ec9b593eb3ddedecefdf4aff5f519ad585667a258956af1`  
		Last Modified: Fri, 02 Sep 2022 03:15:37 GMT  
		Size: 1.2 MB (1163757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff483ca449e233e69f18eb71e430f67ec1b4c8f5a965b4d7efc759a0ba2f18c4`  
		Last Modified: Fri, 02 Sep 2022 05:06:36 GMT  
		Size: 5.5 MB (5546993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f60b8d79e0ce080c903c48fa8296ecb53f67cdcf73d748ec8b454d8d7ec96`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152c32a5dfa1d8b81650a889c55e593122edd4a1b49983a5aae714fb567194c`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e812731a44ee6ed8eb6f479ee177db4e6f5dc9b8f586e3bec76b68bd87b057`  
		Last Modified: Fri, 02 Sep 2022 05:09:37 GMT  
		Size: 120.1 MB (120084257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ce07703bc6ca66551202ce709d2db142f2284d1758e1ae63b0089816db684`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1890f880d76adc2a15589d899c1971bfe3b8c53a24b095b14ff503208a19d2fc`  
		Last Modified: Fri, 02 Sep 2022 05:09:58 GMT  
		Size: 73.3 MB (73321532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1250a9090832c70a8cbb5b16a1c4fb04bd15cb731dc383b88e5e8920a07637`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 262.8 KB (262804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e10b955d6703772baf23131f34012e192b6651bae2f45d5ec1de94db2d65c9`  
		Last Modified: Fri, 02 Sep 2022 05:09:48 GMT  
		Size: 2.4 KB (2425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7586ba8a53515e3a1b9937feaad2e7fede1adbc084ac2d100da1e4a7babb88cf`  
		Last Modified: Fri, 02 Sep 2022 05:09:51 GMT  
		Size: 21.7 MB (21663632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1d667d617e8cf2205c98aec3d4e9667a704e7e1270e6ccceacff672383ee73cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226030547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3f71e64f6f4bbd5dfdb2c020a056ff2446a5c0468227138239c599b8f10b13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:04:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:04:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:09:20 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:09:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:09:23 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:09:24 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:09:25 GMT
ENV ROS_DISTRO=foxy
# Fri, 02 Sep 2022 06:10:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:16 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:10:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:10:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:10:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:10:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:11:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6679da592cfdf550fcdc4b85e065118bc5d71a57534760b4abedb490355889fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:12 GMT  
		Size: 1.2 MB (1165138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5eb560b76837a662c9463136466570590371e820399defb1c9bc087709ea18`  
		Last Modified: Fri, 02 Sep 2022 06:29:11 GMT  
		Size: 5.3 MB (5323438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b3ae8b95a7a2d08be20d992070269ef1ad4349f2d337fedfab469b6943e72`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930dd26a6d335c1bf1f6cde29714b2fab3f457e05a2adc40b520764ea272ee7a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6669566fcc115df3d85e1176e7e645889db7959d6a954ba485ed11367dc9863a`  
		Last Modified: Fri, 02 Sep 2022 06:32:07 GMT  
		Size: 104.3 MB (104266721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d0c7829bec3aa8e600c8677d001a505e7a97ce46e7e8d34a667fa41b38b06a`  
		Last Modified: Fri, 02 Sep 2022 06:31:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5f8d617cb17da8504e284767c00fc2feed07e2f35c7a7b4313b804d53e56b8`  
		Last Modified: Fri, 02 Sep 2022 06:32:28 GMT  
		Size: 67.4 MB (67449113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6935c838d5eb4cd0b713a76063e82036a165b8bc62634dec158e4729749a38`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 262.7 KB (262739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707611d281f0c907bf51272891d4009de29c408cf77e296e33d8b7dc31983b3`  
		Last Modified: Fri, 02 Sep 2022 06:32:18 GMT  
		Size: 2.4 KB (2378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a2c9bbb7d25390f08e6efb8200c4a037a6c8bd6980b91e33212c2d3378a6d`  
		Last Modified: Fri, 02 Sep 2022 06:32:21 GMT  
		Size: 20.4 MB (20366833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
