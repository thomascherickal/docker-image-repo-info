## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e0f2175cf9be5a46691b862fd29a2e0beffec1439df08c60b05f6e83c8bb9300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:1125d4c624347752ce3fcf3e0556fbbf8c56fc4663e983fd67ff76129a50436d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835169484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768b4f8635c79f42cc5ee59f765f2d66c485156547018c19fe160247d9b45c20`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:29:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:29:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:29:47 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 07:31:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:31:54 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:31:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:31:54 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:32:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:32:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77756bcc9e33a789cac2bc5a2a8ed6113862c692b4970d04b04b0bf239d09b9d`  
		Last Modified: Thu, 02 Mar 2023 08:03:37 GMT  
		Size: 5.6 MB (5553670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0752ff12fc1879563f6c3a37566aa1d63df61d32a482e1122678d06111c6c704`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb64a2fb206ee95fea7407d2fa098f13262e2dec6bd6acfc406eb3c7f3ee1e5`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2059687f395790fbfedafba19c2e4f73dd81bccae9ec7df3c7861b1df6886ca`  
		Last Modified: Thu, 02 Mar 2023 08:04:04 GMT  
		Size: 177.0 MB (177016208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1445ae9867c355c105face7eed407747aa39c1481c7133429c4c53f35088f16a`  
		Last Modified: Thu, 02 Mar 2023 08:03:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d980596d1b73b63dea8c555dad924aed845b5cb90d0c7a4efcac51afe9a2f9a`  
		Last Modified: Thu, 02 Mar 2023 08:04:20 GMT  
		Size: 50.9 MB (50940124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a47bd281f5ba44bd21eda0d09fb13887e4d6c4fda7c69a3178992a9c83f88`  
		Last Modified: Thu, 02 Mar 2023 08:04:12 GMT  
		Size: 344.7 KB (344699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9ca0b3eec34631f459c101dd52259cac12e5132e1706dd716cef22ac1fe5ad`  
		Last Modified: Thu, 02 Mar 2023 08:04:24 GMT  
		Size: 79.6 MB (79606966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc947c6624bf33d024b55571718244719b9a5edd2cca1c27afa1a4b480423782`  
		Last Modified: Thu, 02 Mar 2023 08:05:56 GMT  
		Size: 492.0 MB (491972823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:93e63c8844f4360dde7f320e76167dea05ee8f18a1bb7216fab4cccf901f4383
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726200713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00b6305eebbad3d0fab34023a1646dc566a9bdf217beef3b18b78bcf440064e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:41:15 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:41:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:41:16 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:41:18 GMT
ADD file:e066e7492699b78467000ed6a4a902a41599ea2d7aa291332c3f76729a1e798e in / 
# Wed, 01 Mar 2023 05:41:18 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 12:12:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:12:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 12:12:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 12:12:46 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 12:15:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:15:45 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:15:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:15:45 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:16:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:16:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:26:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f229fa8347dd45ed1a1495c295e3cef520b6fc0a5929756068638d7d3ef82193`  
		Last Modified: Thu, 02 Mar 2023 11:06:49 GMT  
		Size: 24.6 MB (24586448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ea6bac35a1ab81469aabdf6a1f6f860ce1c9ed7e82625c53a6f8b1a64e823c`  
		Last Modified: Thu, 02 Mar 2023 12:29:30 GMT  
		Size: 1.2 MB (1154650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14af9ed8fe780bf6b1681423e06ab17566673bef9750c0b5591b03a7e12484`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 4.7 MB (4679133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4bc1671aa822702e1cd36abac0e9193c7a18d0ee42c398e454c47b02f193d`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b751eaf15e5904ee56e930eb3d87c9cc4ea0e10a3ae4f87ff3282b2c170f018`  
		Last Modified: Thu, 02 Mar 2023 12:29:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a025315ed3938804103cdb57fc646fce4f4deeb9fbad47a00f203886109060e8`  
		Last Modified: Thu, 02 Mar 2023 12:29:56 GMT  
		Size: 157.5 MB (157509036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f6dbad8263386860670ffb777d531e98c9c6fe16503702f9d54f3e12f90e59`  
		Last Modified: Thu, 02 Mar 2023 12:29:28 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d249e5b32be6ff0d611151ae4d2b63c966cef66818158da38c4091987a90409f`  
		Last Modified: Thu, 02 Mar 2023 12:30:15 GMT  
		Size: 40.5 MB (40502552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca015739736a2bd72291f44fcdb02fad7bb42e0f3d175dadec86956b6db0ac4`  
		Last Modified: Thu, 02 Mar 2023 12:30:09 GMT  
		Size: 344.7 KB (344697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30691ce4ba2eb6faf749bce8089a569dcb2925e478daff5e14a6824e0de2d8e3`  
		Last Modified: Thu, 02 Mar 2023 12:30:19 GMT  
		Size: 60.5 MB (60496631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7b459fcfdca04b978505b7554f91d5d445a8883b151efd6443e40960489415`  
		Last Modified: Thu, 02 Mar 2023 12:31:45 GMT  
		Size: 436.9 MB (436925149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4826891ed564df798ff1b4aa5407feac941f6a54dc98a853ec9036856f9463cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785456931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9848de65ec4cfa6ab50210233a2530b2cc55a0f9ab478501b85b976c1e923dfb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:29:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:29:55 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Mar 2023 03:32:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:32:40 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:32:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:32:40 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:33:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:33:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13947cb4d4fb29ac4bbd3748e79ab20da65033b2563147127613ccba352ba358`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a630cbcf281c994586155784a2c5c8a5c02f75715b54f9ec0fdd406eed859bf`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72441278ae08e882e2a05bfd9029475e9242e17a2f6b6d22859299db3b3e7f`  
		Last Modified: Thu, 02 Mar 2023 04:07:06 GMT  
		Size: 171.5 MB (171486823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee1963dd3f45dd61f69960595462707cd1dbabe500bcd3fa2b7cbd8ca6d63`  
		Last Modified: Thu, 02 Mar 2023 04:06:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5d1a2bcf7618178b56d1446e6c04fb2115af48f4fa2867c6789f1e58fca9e`  
		Last Modified: Thu, 02 Mar 2023 04:07:21 GMT  
		Size: 45.2 MB (45202848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5fd00223ed309f05c64722f2df17f2327b9ee0ba7dad3204a61b8d28f08af6`  
		Last Modified: Thu, 02 Mar 2023 04:07:15 GMT  
		Size: 344.7 KB (344683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c981817b61382e14bd0208b60a2a288ac8ae59fc2941e85d8179eaffda1a938`  
		Last Modified: Thu, 02 Mar 2023 04:07:25 GMT  
		Size: 72.0 MB (71973530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7950975947accb838c9965d22e2f50224d5b91a7bde53b6d7e48b00e18469ecb`  
		Last Modified: Thu, 02 Mar 2023 04:08:43 GMT  
		Size: 462.6 MB (462565670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
