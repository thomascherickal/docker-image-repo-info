## `ros:iron-perception-jammy`

```console
$ docker pull ros@sha256:c06629c4d15658f8e2a666fc8983ec3e4c0d8c075cfaefe50291efa425334491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:iron-perception-jammy` - linux; amd64

```console
$ docker pull ros@sha256:2b2f9d66370cfda7a91d8e0e6ee55af2b27ab2487382ac63edd19d477bc0b5e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **959.7 MB (959704912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46f035788f2871ea56661de3c07768a00b3aecd34403a57401e703287e75bdf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:33:10 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:33:16 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 01:33:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 01:33:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 01:43:28 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 01:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:14 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 01:44:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 01:44:14 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 01:44:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:44:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 01:44:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 01:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:46:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47086b0f36cc3913cae9fd9a64b76b6129a2606dd36083ea54931e271e7446`  
		Last Modified: Sat, 02 Sep 2023 01:50:36 GMT  
		Size: 1.2 MB (1212988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce8b5b88e015c84c9a67a934f7df859d067527ea2af03630538139167a0512`  
		Last Modified: Sat, 02 Sep 2023 01:50:34 GMT  
		Size: 3.8 MB (3828806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e4c2aec0b05dc7aa86106527a8efdc0f0315ee0879765aaf12f0b2b116b10a`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37a5c0d84afcb36509046b20e6bd1f755a5b271715dfd3d1ee82a8cf78eee1e`  
		Last Modified: Sat, 02 Sep 2023 01:50:33 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f697250a3e61ca29cfd335c1563eebce2ccaab475cabf328dabfde771bc23a8e`  
		Last Modified: Sat, 02 Sep 2023 01:53:20 GMT  
		Size: 124.1 MB (124144205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5ce6717e87e5f504b5991d38b8ce3a4179ee6440bc77575cc7aa0a2313bc73`  
		Last Modified: Sat, 02 Sep 2023 01:53:01 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32443c3ac64e04b22d6797ee761ea18ca5c4749eb5a2dcae8266d2684aaed2ce`  
		Last Modified: Sat, 02 Sep 2023 01:53:39 GMT  
		Size: 85.2 MB (85155437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ac734be63315b3b63b781efcbaa8722df32b756426076cd7162d668e0c33b`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 301.8 KB (301785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443793671c0c8e8e8c531e037c8fee594f63f987915e16e3453604520da34b50`  
		Last Modified: Sat, 02 Sep 2023 01:53:28 GMT  
		Size: 2.4 KB (2429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571dcb4ca7607bd065dfecf00e9fc01451d08d3c1625e0088df997582acb24c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:32 GMT  
		Size: 23.7 MB (23725382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b027d64a215a4fe959ba8f55d39ff5b6fdf732f0bca77b1d446e0ddb154d54d9`  
		Last Modified: Sat, 02 Sep 2023 01:55:17 GMT  
		Size: 690.9 MB (690892485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:iron-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:96868053101d2313b0464f09c9e478ffd49487b41f4c2ac007dafcee702ded5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **920.0 MB (919973844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d3c4ae393fe7c8927bd220b4d15dc36e6b9a0baee35080d72f2487f7ccdf00`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:23:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:23:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 02 Sep 2023 00:23:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Sep 2023 00:23:43 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Sep 2023 00:35:55 GMT
ENV ROS_DISTRO=iron
# Sat, 02 Sep 2023 00:36:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-core=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:36:41 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Sat, 02 Sep 2023 00:36:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Sep 2023 00:36:41 GMT
CMD ["bash"]
# Sat, 02 Sep 2023 00:36:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Sep 2023 00:37:04 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 02 Sep 2023 00:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-ros-base=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-iron-perception=0.10.0-3*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459959187d1cd1ed01b1de7494f5bb59b926b9976aed48c10c5e308b617f3a64`  
		Last Modified: Sat, 02 Sep 2023 00:43:02 GMT  
		Size: 1.2 MB (1215524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f0140b644ef647ab4b336f96b8f557b1b5b55664bc032127b6dd99046456b`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 3.8 MB (3802894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee378876d0254603b8b7793ae409c0503de6acfa52cc70d5e7855dafbdd1d783`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb175d09d5d9ec6033b5d0507062ba5aeb144487d0679a1f01cb2f5b08e768f4`  
		Last Modified: Sat, 02 Sep 2023 00:43:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48558794d076ebc8d1292a959ac39a17e7683b2b9a85b38a6553e7667413408`  
		Last Modified: Sat, 02 Sep 2023 00:45:43 GMT  
		Size: 121.6 MB (121639017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4068f1ecb356b50671aad74bab133f4c7173d2c5544374a926bb511c509d0a6`  
		Last Modified: Sat, 02 Sep 2023 00:45:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcb57bc4c7d7e86f5a699347526dd36d6d6a796ca281a1c43190a17b675f70d`  
		Last Modified: Sat, 02 Sep 2023 00:46:00 GMT  
		Size: 82.8 MB (82840292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f472afd96ac321a5e6cadf1a1f9d0468065b38db7177e38ee01ef8f5caa1a426`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 301.8 KB (301784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792c71e1cd7464d234a82b207e6d65c1d368e11b7d519a91a05eed7c028cb33d`  
		Last Modified: Sat, 02 Sep 2023 00:45:52 GMT  
		Size: 2.4 KB (2436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3335d0568506900d516401d3bb154f04e931bb4304218a71377ef3c4a8286c`  
		Last Modified: Sat, 02 Sep 2023 00:45:56 GMT  
		Size: 23.1 MB (23115925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2223c6ec49752449f5935b69b8908839a7f8afd293ea6e1b278961e66b9129`  
		Last Modified: Sat, 02 Sep 2023 00:47:28 GMT  
		Size: 658.7 MB (658660577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
