## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:96777be5f3eefb281999d0d174e5e3fddcb84b94ef979ef5384f412a16070b45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:a28bc3f892f1dfeecae7a00ba6304b00add7a4f48d9ecc1357d7bd5a3f87a2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448477280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec5677d8005df5c0680c12d81e6e284c12cbdf56cd93577cbf4d460cf52bd33`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:21:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453ce09845a35fb485ffe49a62e58ecd3d528a9aeb7429bdf7fd6941e6eb3ffa`  
		Last Modified: Fri, 22 Apr 2022 03:48:30 GMT  
		Size: 11.1 MB (11083036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:fddf912a33c82b1543471eae076ad06cf16b35a42e3148bb26fe1a6c9b4f54ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (396028177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ec100476c77a1d1449d13f1fef83b0aa56ae785d5cfa2f1916d65d1ef420a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:51:56 GMT
ADD file:4b33ada37adb95859d134226d5b4c6e5ffef998aedb9a3458a11343c62932bf9 in / 
# Fri, 22 Apr 2022 21:51:57 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:52:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:52:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 23 Apr 2022 00:52:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LANG=C.UTF-8
# Sat, 23 Apr 2022 00:52:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 23 Apr 2022 00:52:42 GMT
ENV ROS_DISTRO=melodic
# Sat, 23 Apr 2022 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:55:57 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 23 Apr 2022 00:55:57 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 23 Apr 2022 00:55:58 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:56:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:57:04 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 23 Apr 2022 00:58:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:59:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34c8e4a8441a3ead578ea0979cd16b5e2ce41f1e30b62e3a67d21ba35122cf87`  
		Last Modified: Tue, 19 Apr 2022 13:11:05 GMT  
		Size: 22.3 MB (22302622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78dac1740dba277c20962158ffedf2d8e82402d348696905f021677f39bd2d3`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 840.1 KB (840127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5447846f00f27591b8e46d3b38ffebbff66bc31e9de9cf2c3b5e5a6c14c337`  
		Last Modified: Sat, 23 Apr 2022 01:14:59 GMT  
		Size: 4.1 MB (4086202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41932a75eb917577391976ee9f49725c710c5157e50fdd6ccb6b9c8e098e1d5`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ac0943d34178ee3600408ee4a6a4b32aa4e30704b3bff3a8f6e40a3e46a56`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac4e7b6c165cebc6c91b5e3d400dd9147d7c1c26dd83393a05537b58bde2d7`  
		Last Modified: Sat, 23 Apr 2022 01:17:32 GMT  
		Size: 238.9 MB (238935832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc930c2fa1439a72c7a7da7b411c5475992f870282be102bba7f54333a793f`  
		Last Modified: Sat, 23 Apr 2022 01:14:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111b17d5c1cc72a6871a06f276198b0d5dc5568883736ed039522545225b719`  
		Last Modified: Sat, 23 Apr 2022 01:18:13 GMT  
		Size: 54.7 MB (54711205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5e29dfac7a05eee60d0b464fbfb3608ab32ff8d854f238cc1b4535562b3c`  
		Last Modified: Sat, 23 Apr 2022 01:17:44 GMT  
		Size: 279.5 KB (279458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809fbd8225af2ccbb532c67e0ffb0dbb45c882651e657c991b49e357aef159f7`  
		Last Modified: Sat, 23 Apr 2022 01:18:28 GMT  
		Size: 64.7 MB (64746974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e98b064e5e1e5a43843cc6fa030e1e15c6870aba0bde15440c84e01a8b72d`  
		Last Modified: Sat, 23 Apr 2022 01:18:52 GMT  
		Size: 10.1 MB (10123339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9a9e3ee3227232758bccb1d3fdf9d549d273aa592bb8e91b604709ddc8560cb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.3 MB (422316119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fd080112e8b140a1f7f8bdc44ec527dca5d2546246cf064aa9ce9d86308aeb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20abf96d320289bcf7aaa0d966c1f356ae4f571e3954978baa1dff37d0ccde36`  
		Last Modified: Fri, 22 Apr 2022 04:20:34 GMT  
		Size: 10.7 MB (10734069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
