## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:778b7ac964b3b287e4e1774cb04092b792ab1997be19fbd5e88791f1aaa0715a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:69de2426ae25917fd135e13b693c4fdb995ed36691c8670b0fb3dcc403adebbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742717028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b850365c8337f4ca3e77104a142de5d83d2264ef2a7ee4efdfe7a79cd45de127`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:58:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 00:58:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 00:58:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 07 Jun 2022 01:02:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:02:27 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:02:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:03:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:03:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:04:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:10:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd145b316c1fb7c938c3e1e06f5ce778bf9b0051a70db477ca7a8c7c01a026`  
		Last Modified: Tue, 07 Jun 2022 01:44:58 GMT  
		Size: 4.9 MB (4875695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598864753f0cbdc3bc5352575f8c0d1b6c501c07d44c5127932ca01c31c875d9`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3485714346b9f0f8a36485f223b93e4f06586b8eae6ae6ec8a66b7e7e75fdc`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab3a5eb67d539589601e0fc081dd6b4c37895928b80ca7a3091b0ce46c24005`  
		Last Modified: Tue, 07 Jun 2022 01:45:33 GMT  
		Size: 259.5 MB (259452207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9573725ebd5e712abd6f511e5ab7e0c71c4de8f3b5772bbe4b825f95eb98de`  
		Last Modified: Tue, 07 Jun 2022 01:44:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a68755b20fa638646cbc2cd697f406c0272ad07806d806fad4f3c1fb27824e2`  
		Last Modified: Tue, 07 Jun 2022 01:45:52 GMT  
		Size: 70.2 MB (70246372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa4ee8bafcc8a148ea13c35a18a93a2916a788e882df1240801a488f2c5ed7`  
		Last Modified: Tue, 07 Jun 2022 01:45:42 GMT  
		Size: 280.9 KB (280922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9246d39f4c75714c673a4472b1a858abc20c63bbae81f24a3e477dfcef7f50e`  
		Last Modified: Tue, 07 Jun 2022 01:45:55 GMT  
		Size: 75.0 MB (74994714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8583c777c2fa9f287b0cfe01be8ccbedd75f900aa5c5134e7f291f2c35e39e1d`  
		Last Modified: Tue, 07 Jun 2022 01:47:07 GMT  
		Size: 305.3 MB (305314414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:43dd4d072ac0a44d6e8eb50e47024d8a439498d5c3f54c1de39567256437d967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.0 MB (645961486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95099bc8e1c117b21861ff7804ed59d45f73845be87836b04fe287f005e6ab4f`
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
# Tue, 07 Jun 2022 10:11:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:11:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:11:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:12:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:12:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:18:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:18374d7a96f4a689496a4283a3609e1d0238b5cf7b80d726dcfe9f3c21438945`  
		Last Modified: Tue, 07 Jun 2022 10:31:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aa9ec29b8faadf1492a1a0125309eadc60db62c9fbdb4bb4f2e4a920e019da`  
		Last Modified: Tue, 07 Jun 2022 10:35:14 GMT  
		Size: 54.7 MB (54710964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b412c7fd952ecf2e53ccc51db68fb37bd5f15b271b1c0adb3f91e827297da7`  
		Last Modified: Tue, 07 Jun 2022 10:34:44 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4679bc15953db8db7e6e485b06c1ee4894c618ac0d101b40ec9262cc6e89dc`  
		Last Modified: Tue, 07 Jun 2022 10:35:29 GMT  
		Size: 64.7 MB (64746333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095115930d6f97863ff374209b9cbefb42259f476e4dafc9e4d8282496ee069a`  
		Last Modified: Tue, 07 Jun 2022 10:38:45 GMT  
		Size: 260.0 MB (260042028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:59fd27f3698d3ad83f834b8e90068125606aea13384d53cdd527c873ad6db0dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (703005048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0beae61f293f59474674e7ab7f8749666423d3d25a9201658d9abd59f2fcd9fd`
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
# Tue, 07 Jun 2022 05:49:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:49:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:49:30 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:50:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:50:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:52:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3ba45e675ef36970c7566157a82c9773fec38abb8e1dc9c1ab5228c5c333d1b6`  
		Last Modified: Tue, 07 Jun 2022 06:15:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f068196edb1d7b534e8104afff942478c06340976dcb3d4e4a774cbebf82daff`  
		Last Modified: Tue, 07 Jun 2022 06:16:34 GMT  
		Size: 63.1 MB (63076750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29281438a7a6ff1ad4878920abcef2cbb4ec2aebca524554f5785711059fc857`  
		Last Modified: Tue, 07 Jun 2022 06:16:25 GMT  
		Size: 280.9 KB (280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52abeeddaef7b2bf20aa09a0de360fd0cee28343a09578cd2975aa04d87cd5bd`  
		Last Modified: Tue, 07 Jun 2022 06:16:36 GMT  
		Size: 67.0 MB (67001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d94c12966b3c16bedcf101969ae88fa956b72b32ef7e29b343021cc195aa7a`  
		Last Modified: Tue, 07 Jun 2022 06:17:48 GMT  
		Size: 291.4 MB (291413974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
