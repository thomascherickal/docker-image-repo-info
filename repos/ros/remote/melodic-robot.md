## `ros:melodic-robot`

```console
$ docker pull ros@sha256:e7d79a50b13dedc64deaaa0a71007e6485fe816001e1faaa607e93ce2f71f334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:85bc4c3c605d67ba0ef9275c4750d9cf8af7bcb8a3b01be2a686cb56e570bd51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448601669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8721d889104c51a26ed1d5208079740f172ba6c73512808b54b32fa72fc2397`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:20:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:20:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:20:07 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 04:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:22:43 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:22:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:22:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:23:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:23:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc21f3c6df3e09da41edf5cd277be198a0b9ce9de84590bce7c7f8169fe8458`  
		Last Modified: Fri, 02 Sep 2022 05:04:14 GMT  
		Size: 4.9 MB (4873660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601897ffb3e3526f97b7f3ac57655aa3b636d8d501e997e89629b654dd7e8dc`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02d512a7003472763130f30478d4f0c5e440cc42c6e111764af77b527686d5`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a32123d45b8f75cdc98623e79fe3c15f9f2da76e2827622e844770c38afa4`  
		Last Modified: Fri, 02 Sep 2022 05:04:53 GMT  
		Size: 259.6 MB (259559627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abce6b68d4012a79d622c3088e409f52f46a4c2d57e7d45df885e9a566a052c`  
		Last Modified: Fri, 02 Sep 2022 05:04:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0804aad7d24aedc9674dd262573672ffb24e77bd0b94b38774dd4c1344a65`  
		Last Modified: Fri, 02 Sep 2022 05:05:12 GMT  
		Size: 70.3 MB (70259712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4c705dfb136d0edfefa4b6ea486990b27430cb1acb7e7aa9c680225f5845c`  
		Last Modified: Fri, 02 Sep 2022 05:05:02 GMT  
		Size: 284.7 KB (284711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463d8179e60fd0676ccb9cded217236342e7d2d9185a56f2f003efb6d1e597bf`  
		Last Modified: Fri, 02 Sep 2022 05:05:14 GMT  
		Size: 75.0 MB (74995198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f95ccd28b67e6e24906599991ef70fb02811a4e3873615747bd8af8017f7bc`  
		Last Modified: Fri, 02 Sep 2022 05:05:28 GMT  
		Size: 11.1 MB (11085842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:ae62006b64e3a2c4d27b36f7496af360bb245b87db3fd7e86e14d127ca21c773
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396118357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26cff1365117644feafac15d1e9c78e6c80535736fc97e681ff24a87e798957b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:11 GMT
ADD file:93826239c43c79f307094d84d6fc79733e950dc0c0a332320254a2328eb5fff9 in / 
# Fri, 02 Sep 2022 06:08:12 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 10:12:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:12:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:12:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 10:13:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 10:13:00 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 10:13:00 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 10:13:00 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 10:14:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:14:38 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 10:14:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 10:14:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 10:15:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:15:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 10:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:16:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7347571ddfc71927a9f2ae03da3d05d7d68457aa24b5e18b6c7545fb65f4d034`  
		Last Modified: Fri, 02 Sep 2022 06:09:59 GMT  
		Size: 22.3 MB (22305684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d21ba002f653bb60bdd9a197bbdef9eb24dc5d74a0bd81cda0547264f0e56`  
		Last Modified: Fri, 02 Sep 2022 10:23:59 GMT  
		Size: 832.0 KB (832038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ec8cd2c14b36b5f8974b41cb188422a0e381f5c969da0cc2896861a8cf5d`  
		Last Modified: Fri, 02 Sep 2022 10:23:57 GMT  
		Size: 4.1 MB (4088189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8368dde21d27908fc063b589bde2efee27b4f1342ae83c7429e2e09bedec966f`  
		Last Modified: Fri, 02 Sep 2022 10:23:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6908835ef967d8210b8e4e75bf0d297eaffcd1ad61b90abb3e8bcfc59d786d24`  
		Last Modified: Fri, 02 Sep 2022 10:23:56 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc331ea79a9fd58f9b66d49b91b6e4ba3f0b4c7458b0be78099556b443090a45`  
		Last Modified: Fri, 02 Sep 2022 10:24:47 GMT  
		Size: 239.0 MB (239017199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb3c8d59630dc34d314e9f7e8072876de85786657a7079bd1d1468a06540037`  
		Last Modified: Fri, 02 Sep 2022 10:23:56 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af26fbf63b59a1847b256edbb186bd499accbc44f19c28141bb0faed284a75ff`  
		Last Modified: Fri, 02 Sep 2022 10:25:09 GMT  
		Size: 54.7 MB (54720925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c87beddd5e5faf1418121fd2d86d7ce30389d364c8461bf963ce74a0b7c462`  
		Last Modified: Fri, 02 Sep 2022 10:24:59 GMT  
		Size: 284.8 KB (284762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986fa9f5c46ad6bac693ab6c06a2ccdc325c7100b841b18a780554b477d77def`  
		Last Modified: Fri, 02 Sep 2022 10:25:15 GMT  
		Size: 64.7 MB (64743689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d956538aae39591073c9b773179fbfc07aa2893ca7fa49152bc8e56b37a57d0`  
		Last Modified: Fri, 02 Sep 2022 10:25:32 GMT  
		Size: 10.1 MB (10124024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3dc563618f94c289ff4fb6380b08ac5e419824dd9ab05ee85824d9fda47a01de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.4 MB (422448964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f87df4ce0f85310e58f4b79d8592460a43aafc45d9dc8e8909fe84ced5eee8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:58:33 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:58:44 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 05:58:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 05:58:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 05:58:47 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 05:58:48 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Sep 2022 06:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:00:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:00:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:00:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:01:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:02:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741c1db167ba98dcc4f0b1dce059664982999c77d7cad916a075711462e7e58d`  
		Last Modified: Fri, 02 Sep 2022 06:26:53 GMT  
		Size: 831.6 KB (831649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4f808c51f1cf44217d8ce4ebca03255e969acca4cf09dff77aee0d3f3a816d`  
		Last Modified: Fri, 02 Sep 2022 06:26:52 GMT  
		Size: 4.3 MB (4265983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19873eb8e73732ae72ef6128c3fa94f987527a5a1439d57eb398f1cb5f4df`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fea62807d8351d36c0b83cdd41872e4d80c976755fa7a501da8e7e7437ad6c`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181336855135b72b6bf5b30d7c1e5beebbdd63f1fe6c933ab551f4a196e800f1`  
		Last Modified: Fri, 02 Sep 2022 06:27:26 GMT  
		Size: 252.5 MB (252504641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284d05b44a890de734833cf20b5313f89437f66ee971f29d55252b3d63572a19`  
		Last Modified: Fri, 02 Sep 2022 06:26:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5912bc4d8ce79891b6639473d128eac65e87986185897f1cc258c457ac8e7ca1`  
		Last Modified: Fri, 02 Sep 2022 06:27:46 GMT  
		Size: 63.1 MB (63088909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767c5618f004c047c357ca236bbcdb7d205c11b960f1d0d7e69a5b074923fe7`  
		Last Modified: Fri, 02 Sep 2022 06:27:37 GMT  
		Size: 284.7 KB (284651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbb5ba813f9800cb0ccc8cc793a2a5a75588b1ba651ba7a58afd3b8c9f2115`  
		Last Modified: Fri, 02 Sep 2022 06:27:48 GMT  
		Size: 67.0 MB (67001363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e000c44a6a1b7e651141833ad6b8b222dcb51bff6496e03dd8a4420a6836cb`  
		Last Modified: Fri, 02 Sep 2022 06:28:04 GMT  
		Size: 10.7 MB (10735885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
