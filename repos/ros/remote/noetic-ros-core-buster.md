## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:bad4044bc668cd6eed1fcc56f771c626a9038dbe8725ed2395ffc2841f1f4c7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:7785269a093c90620b0dd7d1f33e681c451d7533ccf299ec651e41a0031b80bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300588636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1146a51e430cec8a22d8d8ad7332fc4e618b36b40ab651202f07f910aa0b4fa5`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:55aed9d35e66b740bdf5d6a7ec786f7b1ccc2b86f82a298a18d07c98335a87a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244571461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aa8fae09c5ca8a3e3ee00729f90344c724e58db573c46921dde685023ce1f8e`
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
