## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:4ac19fe814f4fcc14484aaa2ceeed2006a0295f052ecf31bcf7aac4cff0f4c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:bf0fba36da1ab60d2a1f54479ac9827729238660a3d33139ec57f51b46fe317f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.7 MB (484685923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30da8c8d1452a1dcd694f99f784dc52e0a117c88a7a55e4b9cffa8ae146aaf1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:09 GMT
ADD file:9ea7d74fdfdb29946ab72e1aea5810331debe27db7e50a0fc4e0d5a192ab6166 in / 
# Wed, 01 Mar 2023 04:10:10 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:01:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:01:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 17:01:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 17:01:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 17:02:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:02:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 17:02:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 17:02:40 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:03:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:03:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 17:03:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:04:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8a6bce2a40cb0c3e3cc6646bfeccfb2ac5b303c39ea70d67e30406d270f2009`  
		Last Modified: Wed, 01 Mar 2023 04:14:42 GMT  
		Size: 50.4 MB (50449101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1ffc835f48ecec7c683701866277b285e39a42777bb6819d705ba54c9b7ee`  
		Last Modified: Wed, 01 Mar 2023 17:09:08 GMT  
		Size: 10.9 MB (10896984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab4ec3b1ff1518ff16c31e9e4f4b239089fdad9819bb1b0806733d42d30b73`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9841b85e22a255629ec6b026e828d764cdc3c990de2d2c70eef2cfa655083074`  
		Last Modified: Wed, 01 Mar 2023 17:09:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fcea5877730e4a516a82878a4f5f98da043bd4cc6f242e907c49f88c966f58`  
		Last Modified: Wed, 01 Mar 2023 17:09:38 GMT  
		Size: 239.2 MB (239240139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e461f854cd1f5763471d57c32aadc9f1bf067ff5b25408ead48199dee31c5f5`  
		Last Modified: Wed, 01 Mar 2023 17:09:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2b0f357d817701e8f5aa5dcd9f07b1ac984f80f3c9a9524a119394f9f67e49`  
		Last Modified: Wed, 01 Mar 2023 17:09:56 GMT  
		Size: 86.6 MB (86623675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25a2a9e7feaf23a3d2bf9cef272554c05d1f79eb0dfb7cd0de7dc9c8eb0d42`  
		Last Modified: Wed, 01 Mar 2023 17:09:44 GMT  
		Size: 339.1 KB (339063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983285871d052c66975bf9eb2cbe185a844c7f586fd82d3003a0d5e980f6f61d`  
		Last Modified: Wed, 01 Mar 2023 17:09:54 GMT  
		Size: 76.0 MB (75978363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc393ef17f1c6bf4420e3ff6a2c30422a37cbb1f13df86c8d971e33dca19fe4`  
		Last Modified: Wed, 01 Mar 2023 17:10:05 GMT  
		Size: 21.2 MB (21156186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5f60b45ccb6ab1271ed9cc7efb6f11e9c0ca8b891e82b4f9881db630ae240030
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424215617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e48551368ac4ebee90f1cd089e2569e2739814ed992ab7a6fa66da36d51881a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:46 GMT
ADD file:bf5b2f8cbddd98de6093dde190b043c3e2b58a5063d1acec0aba091e7d203dbd in / 
# Wed, 01 Mar 2023 02:20:47 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:29:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Mar 2023 12:29:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Mar 2023 12:29:13 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Mar 2023 12:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:30:41 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Mar 2023 12:30:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Mar 2023 12:30:41 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 12:31:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:31:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Mar 2023 12:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 12:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06cfbde07ccb39d53563bd87f3c2b50f04ddd0c8f6cd52be3c7089a3413688e1`  
		Last Modified: Wed, 01 Mar 2023 02:24:34 GMT  
		Size: 49.2 MB (49240002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fbcf95c26646fbabe7bb6f29416ca2663c0cfd87e1ccac361a7459568915`  
		Last Modified: Wed, 01 Mar 2023 12:37:20 GMT  
		Size: 10.9 MB (10902711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46d425485295faa6248cc3b6ce203089f5c51e6d6bd9ec2c65a3724f0986ba0`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de7b8f0c8434b3ef1c87e53a130007029f5fd37ea81634299d1e8226d10b4d5`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b26d79f53cceae9c1d805e9d806a04c531a4290ef45b9f07bdc82202a1edd`  
		Last Modified: Wed, 01 Mar 2023 12:37:41 GMT  
		Size: 184.4 MB (184426336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e132bc958bc874cc517925ada16c2f3e782550fa85b319f3c4d921c3056fa77`  
		Last Modified: Wed, 01 Mar 2023 12:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684edd9821b7de6b481112fbe45042cad36413aa11363fb633886c635a8f9671`  
		Last Modified: Wed, 01 Mar 2023 12:37:56 GMT  
		Size: 84.4 MB (84394773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca3197ee040ba7fb24fa4bd78b4b5706f52ca48e0aa05792b4d71282bf02b8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:48 GMT  
		Size: 339.1 KB (339066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66c8397888300bf62815d64b821ce057d0870bdde305763d3b14c7c7531f8c`  
		Last Modified: Wed, 01 Mar 2023 12:37:55 GMT  
		Size: 74.1 MB (74090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb6cb0f9628a2810ae12f64de2ed0d14b86dab3b639e2568dd649b652a664ea`  
		Last Modified: Wed, 01 Mar 2023 12:38:04 GMT  
		Size: 20.8 MB (20819697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
