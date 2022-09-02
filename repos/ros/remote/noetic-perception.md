## `ros:noetic-perception`

```console
$ docker pull ros@sha256:4e3fde687b980590d7921509ecc36ff4c79f594bad9d0d38579e36fab317f80f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:92a9a61a2bbca7538207c06e045a7a5e686090a54831516ffa488a491aa1c4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835120913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536572ffb5a95c08ca27649d9209f61d60a1f36a15acdb55bfb3efe0650d171d`
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
# Fri, 02 Sep 2022 04:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:eec642114a0fb290bf0ad8660843fcd6f3653247c1aedf51d36e3b9afa30a2a4`  
		Last Modified: Fri, 02 Sep 2022 05:09:04 GMT  
		Size: 492.0 MB (491969560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:935ddcee58c9eb35e003fb6c6b68e687bdf79471978df21a0a25d65968eb9a1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726106884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048cadd7d13063c34d8777ebb2451790e3d6a6f1a37c19485910f29b4c991de2`
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
# Fri, 02 Sep 2022 10:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8660ad4359f03577971ce6066b4e2ba25eaa122b991d33ac1327c8247bd941a4`  
		Last Modified: Fri, 02 Sep 2022 10:29:19 GMT  
		Size: 436.9 MB (436889479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3a23640f0502b7ce1a14a1ce2fb0ca734787b52dcce2179726207994db47b046
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.7 MB (784702327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18c06d8aac74677fc646cd57ac4f15d1436576e7f99961067ca2b0b864f39b5`
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
# Fri, 02 Sep 2022 06:08:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b8b396b7a3bfa745d7c175ab81e6fefdc70dca400b25af857523fb7351d8252a`  
		Last Modified: Fri, 02 Sep 2022 06:31:35 GMT  
		Size: 462.5 MB (462535548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
