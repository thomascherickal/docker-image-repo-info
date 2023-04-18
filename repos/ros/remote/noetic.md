## `ros:noetic`

```console
$ docker pull ros@sha256:2a6a1279dbefe704c75455ab745cee108d76d9a2928b59b1fb2f46dfaf0b1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic` - linux; amd64

```console
$ docker pull ros@sha256:f10dcf5c7de2ebdf90dc2fe1c0c17359ad44d184c307c37945dbf6868c74c1bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343151242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d932427105199181dca9d9ad90a855f7e395ad62ca98042928922c4b4c833dbf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:00:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:00:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 01:00:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 01:00:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 01:02:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:29 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 01:02:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 01:02:29 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 01:02:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:02:49 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 01:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ff3f6c5dd326a8361d5d9fba50621a210a6b840cadcc97c516817cb8cf8d7`  
		Last Modified: Tue, 18 Apr 2023 01:15:00 GMT  
		Size: 1.2 MB (1157164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b302bcd474554096ffccaf8412038965be0feec446d247de776919747c75591`  
		Last Modified: Tue, 18 Apr 2023 01:14:59 GMT  
		Size: 5.6 MB (5553578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b009b5adbd509635590b8ca3f676b6641b7bb66ab0512ccd4066db76ca60f5`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b0f9dac5dfd8149acea5db9be04cf12e33419619851a19de0dc33268bc543`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb5b823ac6a3ceddc3171904f453472228f5ce941332ae1c4c3a97b62399cb8`  
		Last Modified: Tue, 18 Apr 2023 01:15:25 GMT  
		Size: 177.0 MB (177015888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d72917faacc696317190bddb87cec63b461b7bbb280990ed04a1ab40b01565a`  
		Last Modified: Tue, 18 Apr 2023 01:14:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616856e05b972b9a1860c701a649c8178c883e876e7555fd8d7c2ffb639a3a82`  
		Last Modified: Tue, 18 Apr 2023 01:15:42 GMT  
		Size: 50.9 MB (50939692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27b2bae79f36c6b903ae1427cbaf54e4dce26b1dfb7325ba73541b10d1525a`  
		Last Modified: Tue, 18 Apr 2023 01:15:34 GMT  
		Size: 297.1 KB (297147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d72adfba67c09bba7be116aa4cd34b1519f68648b3fa6f0afc7e5a92979a76c`  
		Last Modified: Tue, 18 Apr 2023 01:15:46 GMT  
		Size: 79.6 MB (79606798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:e67e92cb18c95bba379dfc18c80f8c0a74fd5fcca4a46385857196e5346af8ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289226398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ca36166d90654bd251fd79f47436a0366dfddb369712dd9d6245bf6f34d118`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:20:47 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:20:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:20:48 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:20:50 GMT
ADD file:0da456bd328984fcedf5367b46a38da6ca4b43061baf6d1283380962cddc7481 in / 
# Thu, 13 Apr 2023 13:20:50 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:03:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:03:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:03:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:03:51 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:06:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:06:05 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:06:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:07:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e68c91cb250f35160f683afa80c3ada46f06948ded46a188be490ea3afff08f5`  
		Last Modified: Fri, 14 Apr 2023 09:34:28 GMT  
		Size: 24.6 MB (24586976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ecaa4a720ffd8b3f56038a2d5f616807fa7485f551442c1f40ea8fd3981476`  
		Last Modified: Tue, 18 Apr 2023 02:16:19 GMT  
		Size: 1.2 MB (1157196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7945fb40cca95a4e5c72309573289c0784fb110e1606688d25f64849ca28139`  
		Last Modified: Tue, 18 Apr 2023 02:16:18 GMT  
		Size: 4.7 MB (4679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c069a57904ca9856ac4e9d5b220c3c4b98c50fded7cdd74e670f2338c3fb330`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b1cc4dc29f69e7392b245372d8097dcecebafe0667c8f2726299a4de8874fb`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dd47d037bb6cd6982d83524e76328da32499ff9d59f265b0ec7756a8a52072`  
		Last Modified: Tue, 18 Apr 2023 02:16:46 GMT  
		Size: 157.5 MB (157503873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f3aa8b76ccbcd8b349669fc88b8205c0cd0f8a4d1c858519ae07119f9e4879`  
		Last Modified: Tue, 18 Apr 2023 02:16:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefc606d3dd23a8815fd1e238d5fdfe32080b4795073ba61cee804527816162a`  
		Last Modified: Tue, 18 Apr 2023 02:16:59 GMT  
		Size: 40.5 MB (40503298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc1f052e8af8e9f8ce3488131b6e3db7f4c91846dfc84d2f75688b69a04961`  
		Last Modified: Tue, 18 Apr 2023 02:16:54 GMT  
		Size: 297.1 KB (297142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb40216b8c1d941c1be2d7ab0be0dd7b2c40485ff30f2d5693e2c7bf59ee3f`  
		Last Modified: Tue, 18 Apr 2023 02:17:03 GMT  
		Size: 60.5 MB (60496479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d5ea21ddeb3a8263b55ff73a81ba0a53954362e89dbb5bc3070f7c55b5e8c6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322836771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc8c46b2872805b8ba64f84218bf3b7ff59ec0c72e34a2e11a8be1df5048b440`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:06:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:55 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:06:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 18 Apr 2023 02:06:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LANG=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV LC_ALL=C.UTF-8
# Tue, 18 Apr 2023 02:06:57 GMT
ENV ROS_DISTRO=noetic
# Tue, 18 Apr 2023 02:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:08:59 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 18 Apr 2023 02:09:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 18 Apr 2023 02:09:00 GMT
CMD ["bash"]
# Tue, 18 Apr 2023 02:09:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:09:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 18 Apr 2023 02:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d6dffce030c2c6f198ef16ad47e4720f0a13e866894c874704a268d67d9457`  
		Last Modified: Tue, 18 Apr 2023 02:22:04 GMT  
		Size: 1.2 MB (1157932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7244b6de4ee8515b3ee22913bcbdc5c6e96a2254103d3e5c26708af6de8624e7`  
		Last Modified: Tue, 18 Apr 2023 02:22:02 GMT  
		Size: 5.5 MB (5532603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89011a19d825c31dd1ecdacfff5418ea066cc6c3d8b16aa5495409bae017b1f1`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcf18013b664813b5e2ac52cbfde90f06a51486a530223919716ad97cb24c2a`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1809be61e23432d56e45874bfae781cc545d2889cf2d4a4ec837bbe62c12ae`  
		Last Modified: Tue, 18 Apr 2023 02:22:22 GMT  
		Size: 171.5 MB (171472211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29476e1a64f98957516be750445e8fe8dab41029f42b326871dad7c15a5002f4`  
		Last Modified: Tue, 18 Apr 2023 02:22:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9778a01d5ceece6c4f0c2c0c02cc6f090ecb6a15e4ae5b1ae330ee94589a570`  
		Last Modified: Tue, 18 Apr 2023 02:22:36 GMT  
		Size: 45.2 MB (45203703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd76f4f02f17a00aaef729800e659e052bf15f73a3a5e03cdb8c835a754761`  
		Last Modified: Tue, 18 Apr 2023 02:22:31 GMT  
		Size: 297.1 KB (297141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f09767fc16c06e81dd2dc318f6e7d1bb01562aefaaed477349db702168210`  
		Last Modified: Tue, 18 Apr 2023 02:22:38 GMT  
		Size: 72.0 MB (71974377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
