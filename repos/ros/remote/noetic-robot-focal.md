## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:ed00f1c0e6c2f074587303dc200ef98cf93e6808b96bccd791a44263bf7f9701
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:669c18fe44b20f61149f51771c40553202d44d46ec86a74600eb1e7431000bd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359011850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d33234d459a19d3a4bbe5ae8699e82192f9a9f50eb461757a4dbee1be52429ab`
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
# Fri, 02 Sep 2022 04:30:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 04:30:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:30:46 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:30:47 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 04:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 04:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 04:32:46 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:33:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:33:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 04:34:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e933af47665655d97d902ecb6d264063a041b2c12dfcbaf849a05672cafc9044`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916d550484243d392ddc6fdca4ba34710bd3305a578bf9d241f2ad6d944c099`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d152bd7bb3b1335dd05a53828858de8ceab15c85e96fdc0181b2e38f72323b8`  
		Last Modified: Fri, 02 Sep 2022 05:07:05 GMT  
		Size: 177.0 MB (176996015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edc8aa6732f94d22820aa0f96400c620b51e015fa6a940c03e9b579f0de306f`  
		Last Modified: Fri, 02 Sep 2022 05:06:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38aa1dd8b74095a973aa1b1fe9d7495fcbf895f954b66adbff905119d10103`  
		Last Modified: Fri, 02 Sep 2022 05:07:22 GMT  
		Size: 50.9 MB (50940098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5cec93c265dc40fb6eb4790e71c25ac877e2addb6eddf96377e4336554651e`  
		Last Modified: Fri, 02 Sep 2022 05:07:14 GMT  
		Size: 325.7 KB (325719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca383d78ab41bd8631ac0ef8afce8de1b461c6b95a74094926636a7d8ff9c57`  
		Last Modified: Fri, 02 Sep 2022 05:07:26 GMT  
		Size: 79.6 MB (79603671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0626adf2cf42b6dad9a292e7d21a2c1206ef600a05e321e33d906aee3aa891cf`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 15.9 MB (15860497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:d047da019eed0ae7d07f4483f4f6dca6ddb5aab8834d63bcee903ecff0073bc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303305191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388f41565b185241b75e7dc046ca9f15971530341e6c9d8aabf93ee93145659`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:53:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:53:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:53:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:53:47 GMT
ENV ROS_DISTRO=noetic
# Wed, 03 Aug 2022 22:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:55:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:55:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:55:11 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:56:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:56:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:57:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d345e3aeca1c4dd8930e961af9d46712aa474a7ce53acba4f54b4ff3b113a84`  
		Last Modified: Wed, 03 Aug 2022 23:09:30 GMT  
		Size: 1.2 MB (1181992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cf40d14b8b7f81b4f192b1708fbdb0a57c3626f5b72be630a041c1f634f266`  
		Last Modified: Wed, 03 Aug 2022 23:09:28 GMT  
		Size: 4.7 MB (4676289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3223d85d87ee35ea3ab4535feef031631e281f3c617de4cdc218c4983c9b6f`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5bf7f51f5d7e24eec5395780a42aebd0c726cb0466dd5e0b2c492c6d0c84b3`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c66f511399e2f2993ed8fd014bb457c6d6a9483ae665aea0e9eb01fb0a54b4`  
		Last Modified: Wed, 03 Aug 2022 23:10:06 GMT  
		Size: 157.5 MB (157479986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa138f7b3214bda7dc2ae9534dff610b8c2a41d8de8dfb7c8a69ab5eba596887`  
		Last Modified: Wed, 03 Aug 2022 23:09:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e956f29112fb883f35fde1c1d67fc064ab659310ef5bc2f894fd7fabc7cb1b53`  
		Last Modified: Wed, 03 Aug 2022 23:10:25 GMT  
		Size: 40.5 MB (40505939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b4fa88c4ff97cf49d78a40c699333d1182e8a7a0cdb62a65b76e6d6ba39208`  
		Last Modified: Wed, 03 Aug 2022 23:10:18 GMT  
		Size: 323.5 KB (323517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f054c04c983a4aa345e62e3a2df78c234e061aab4b29b964612f3ff52473c`  
		Last Modified: Wed, 03 Aug 2022 23:10:30 GMT  
		Size: 60.5 MB (60480770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714bead958c0893197e557905b695ea7e2e9f9a621b7b00a14bc25d104d1e307`  
		Last Modified: Wed, 03 Aug 2022 23:10:48 GMT  
		Size: 14.1 MB (14065011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7115e6f5880c00e61f39bffe3417db74ca7d9d2c08fbf76d3693a0dd38cb54e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337615813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f84482c105f51b121ecf76fca749f92f777fd4925b639fa1eb780db6014cc9`
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
# Fri, 02 Sep 2022 06:04:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 06:04:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:04:14 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:04:15 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:04:16 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 06:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:15 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 06:05:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:05:17 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:05:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:05:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:06:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2e14c9b385a2e2a1aaf2e3e0e96bb0ab19b0ae4bd1ba4df6e04bd247b310d5c2`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb230fc3fead8135d54463448100608dff8db563117ce648ff536d58028e043`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a441fbb85ca0fc9351965d962c26631f0c0fdd0a80a5de4349d0a2fe39cdad`  
		Last Modified: Fri, 02 Sep 2022 06:29:39 GMT  
		Size: 171.4 MB (171414641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cbf101495077c64a07b49123584c92c50e4eedbf37c6fe039a5c96c1a45fa`  
		Last Modified: Fri, 02 Sep 2022 06:29:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e164058f5f6b26f33ca86e472799ca95df650c8044c529338423424b38ea4`  
		Last Modified: Fri, 02 Sep 2022 06:29:56 GMT  
		Size: 45.0 MB (44988847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fcd9c3e7122e87ef29f417d198e443a1892d621f1fe005f9cbf9072b5d3b9`  
		Last Modified: Fri, 02 Sep 2022 06:29:50 GMT  
		Size: 325.7 KB (325657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65599a689993fa62149f8b2028498730ddd14125298b858124751013f37cdba4`  
		Last Modified: Fri, 02 Sep 2022 06:30:00 GMT  
		Size: 71.8 MB (71754873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18121c479bd23f9bed87b73dab18f777737e353710d6bc6fbea8ba53d4921f2e`  
		Last Modified: Fri, 02 Sep 2022 06:30:17 GMT  
		Size: 15.4 MB (15449034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
