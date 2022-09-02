## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:5946e40a2f0c55bca931a65d8538fd12c2ad458015cdb3d92ed32ac69f77a7f6
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
$ docker pull ros@sha256:fd59aeebca77bf32abbf9eb6512f2f0823f077f02291f9b039679d0da17c3a8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303282656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1626cbea0be42ac6675d4510f728e4c9063817632856b10eba0aeab63ff2291`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 10:18:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:18:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:18:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Sep 2022 10:18:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 10:18:20 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 10:18:20 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 10:18:20 GMT
ENV ROS_DISTRO=noetic
# Fri, 02 Sep 2022 10:19:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:19:19 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Sep 2022 10:19:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 10:19:19 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 10:19:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:19:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 10:20:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 10:20:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2728e151d700852a4e3785ed979fbca05aebfa838997bbfb6208dac2baf0be`  
		Last Modified: Fri, 02 Sep 2022 10:26:41 GMT  
		Size: 1.2 MB (1164705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea485604404c82ae7a2f2b9727554ea35d445dd4cbeeaccef029347c75a31a`  
		Last Modified: Fri, 02 Sep 2022 10:26:39 GMT  
		Size: 4.7 MB (4676623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba218441b7bd8233673d1400fb8680f70b7ea7b544413e35a9b77721eaced8`  
		Last Modified: Fri, 02 Sep 2022 10:26:38 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a65ee78d700318acee75a82c045825dbc4fd919af3f26b2d49f42e2b179ed16`  
		Last Modified: Fri, 02 Sep 2022 10:26:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a6d872569136597e54453ae5b3342d12f39ab83c48427772b9955e842e21ef`  
		Last Modified: Fri, 02 Sep 2022 10:27:16 GMT  
		Size: 157.5 MB (157471800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d431d2220c1d4633ae54c0ff2313b6c33ac62a1fc987657632054d763e35c2ab`  
		Last Modified: Fri, 02 Sep 2022 10:26:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf70c92a20f52607c496f6d3dd3f9356018df2bbca47784b18fb4d39c72c3d9e`  
		Last Modified: Fri, 02 Sep 2022 10:27:36 GMT  
		Size: 40.5 MB (40506172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e2cd1304a712507b28aa65a90a2070fa7724b97f8094037a9b644f01384761`  
		Last Modified: Fri, 02 Sep 2022 10:27:28 GMT  
		Size: 325.7 KB (325746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233f46cc3767a0e7e87109e7864e973fb75be53a37135001058671518d0670ef`  
		Last Modified: Fri, 02 Sep 2022 10:27:40 GMT  
		Size: 60.5 MB (60481203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe8686746a1c3171bba152a0f77321f3277915dc809fd9f00ad241f65df1208`  
		Last Modified: Fri, 02 Sep 2022 10:27:58 GMT  
		Size: 14.1 MB (14065251 bytes)  
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
