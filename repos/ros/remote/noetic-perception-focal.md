## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:c7947ce944885869049379863e337d9bc728223387521db916f911fb71377743
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:ab69286a981b4c72f6cfc5c3b5b915d7976c67edf8350649071ecc6a1855f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834986866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4e4bba5021550a163834d0d889b8f07daafecdaf9de04b4e27ca6f13665025`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:21:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:26:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:26:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:26:37 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:26:38 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 03:28:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:28:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:28:28 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:28:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:28:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:29:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:36:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ade01d9d7a3d8c0634326d89adaba6d97dd2884f45e985281ea88d141f73f`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 1.2 MB (1180875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4624fbd86c08e579fe05e18065911602478ec2bdc1239e5b786f8b5515dc6e90`  
		Last Modified: Fri, 22 Apr 2022 03:49:39 GMT  
		Size: 5.5 MB (5546643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a113e5bfc6a41a0f6d9401ad372ec451407fd55bff2862a2023976889322604`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c65e0abed62803e4b89b3aa305b9b4f0262f25940675f4b8fa7ad7bb9f01a9`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90362b1253ae0b3ad24a095a66a71c2437d714ea43529f9af6cf1f9ee26e7d6`  
		Last Modified: Fri, 22 Apr 2022 03:50:08 GMT  
		Size: 176.9 MB (176875279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da76ce8b30c3127dada4dbec6e2374d087e7e2b0951038c14545d05b87cc7`  
		Last Modified: Fri, 22 Apr 2022 03:49:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fb42a12f184b9b6ad2c9b99a06bdfba4eb6b8c9d97cb8eb224a20386496a4a`  
		Last Modified: Fri, 22 Apr 2022 03:50:26 GMT  
		Size: 50.9 MB (50933515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b9199749d47db40394c6f583da9bf1786de2f23b56c00534df5ab66d5e7ff7`  
		Last Modified: Fri, 22 Apr 2022 03:50:18 GMT  
		Size: 314.8 KB (314824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f59c451e50b55164b1df4f395c7658e7583fbee1cb10ac1d0c4231a7abf39`  
		Last Modified: Fri, 22 Apr 2022 03:50:30 GMT  
		Size: 79.6 MB (79602400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92599f66529a813a6e3e49ab12cf914bb5e22f6f03eff38e96f0b8cb317b249`  
		Last Modified: Fri, 22 Apr 2022 03:52:11 GMT  
		Size: 492.0 MB (491964919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:7d56f291986dc722a8e2a52e75fc12fb168773857ad4514cfc8932159ef3e72d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725580028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3353a655f04e0a031640a07211e1a91a7cd3c8602f430b5db605261eb69626`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:26:01 GMT
ADD file:be35fd9a0ef4a49afbe583edf1750187cad18b1bde4e7bf0ab344464740b5749 in / 
# Wed, 06 Apr 2022 03:26:01 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:32:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:32:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:32:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 04:32:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 04:32:48 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 04:32:48 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 04:32:49 GMT
ENV ROS_DISTRO=noetic
# Wed, 06 Apr 2022 04:35:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:35:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 04:35:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 04:35:16 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:36:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:36:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 04:37:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de340d6c69b8bed917b969ad75b8fe4fe951502bc050b013dc9151c3632fb704`  
		Last Modified: Tue, 05 Apr 2022 13:15:39 GMT  
		Size: 24.1 MB (24073792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce0b0d26ad7a918b36da73b2eddac1e8f316863bbccd547c7ccadf4c7b5b8e3`  
		Last Modified: Wed, 06 Apr 2022 04:51:28 GMT  
		Size: 1.2 MB (1181524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a650205a9690aefea5eeec6ae78f99583040431f6fab18289857cc3d63c1ecc`  
		Last Modified: Wed, 06 Apr 2022 04:51:27 GMT  
		Size: 4.7 MB (4676054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af4193a1277485335b3de17430e9866176d6776e23f4a3e0408f9d843c4bbb6`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d32a40c6e63463e77533412a4d8ed9f74793778c730bec91a7f5a9d14688d42`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fdf1f4ad453b3a18dd87e720f5c322b674889bef7f10ea87e6856841a9ba5b`  
		Last Modified: Wed, 06 Apr 2022 04:53:35 GMT  
		Size: 157.4 MB (157429225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfbfdf74b4e2df8963d7509f98192a343047402ec0d91f9d448a656ec970061`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddadecb4a27a3e0d593b52126b531eccca2f87e3620c832031450f532782c34`  
		Last Modified: Wed, 06 Apr 2022 04:54:09 GMT  
		Size: 40.5 MB (40500174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f7f0954acfa0e5e6880e529feb45596adf4c793185871dcbef7efb79fe8aaf`  
		Last Modified: Wed, 06 Apr 2022 04:53:47 GMT  
		Size: 311.8 KB (311831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1792acea348afad56c81f309974ab41d76528931ea68d24a5fde2c9beaee0c45`  
		Last Modified: Wed, 06 Apr 2022 04:54:27 GMT  
		Size: 60.5 MB (60481261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae128a9a72abbe77d4af136fb58ec21027d36cc7b27fcdedb82f2151d0f2bee4`  
		Last Modified: Wed, 06 Apr 2022 04:59:34 GMT  
		Size: 436.9 MB (436923754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:822d55d8e5db88b18a8402842e71b6281321f07469affbc499bfa930ce81dbb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784528201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d61056ee090fdeb21e163357da8bc408b4eaaf09b0d3e55c5d87489ce6dcb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:03:07 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:03:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 04:03:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 04:03:21 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 04:03:22 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 04:03:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 22 Apr 2022 04:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 04:04:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 04:04:20 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:04:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:04:46 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:05:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bb66f5b43cf438acc27a8b8900f7cc1c3dfaedb4ee818db8a59bf41c42fc6f`  
		Last Modified: Fri, 22 Apr 2022 04:21:48 GMT  
		Size: 1.2 MB (1182265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b068ea2e1ffb5b9a37280ef07a4c77701533e8fc89f0cff5ae1030fc9071642d`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 5.3 MB (5322047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ab2e139969bdbe43f26ec8ea626d0d45f664ba1ab5c8ff9b13d95125924802`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4947b27b9f783c78daa99ca2837e47f986eccba2ce07bb5c33aec2906a86368a`  
		Last Modified: Fri, 22 Apr 2022 04:21:45 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6fff6dcaa63ad76aedfc4a0eee7c83089c01e2e07bdc810aff2039e5cfbf6`  
		Last Modified: Fri, 22 Apr 2022 04:22:15 GMT  
		Size: 171.3 MB (171302301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dcb90c52e30ff30c02c16d4ed566a21a591a8ff0276fdd750067fd81f0af6`  
		Last Modified: Fri, 22 Apr 2022 04:21:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff39aa99dacf9ad0c1028c5203e1be7614e3bfa536edbf181e6f5bfc8db0ae8`  
		Last Modified: Fri, 22 Apr 2022 04:22:34 GMT  
		Size: 45.0 MB (44988669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4364f46644c0882bfedbfdb75eaace4c1b1b3cd6632f13486bbe5069e78c43`  
		Last Modified: Fri, 22 Apr 2022 04:22:27 GMT  
		Size: 314.8 KB (314771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac61d218e17129a0b8870e1e737227d84450631e4a4f8824a57d2b189883e2d`  
		Last Modified: Fri, 22 Apr 2022 04:22:37 GMT  
		Size: 71.8 MB (71753630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb63c1f2c9e055fd5f1dc6867393368659b889d9ee88fe4917338270821237`  
		Last Modified: Fri, 22 Apr 2022 04:24:13 GMT  
		Size: 462.5 MB (462493010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
