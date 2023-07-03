## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:6ff5bbef95a9f44589ed642a7b01ad5621dcea3da50569cbf931c10f626516d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:f20110db44563528486b919197d2ace26dbb768374d193cf37f62b417437b42b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.5 MB (743487700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea660cee3be0fea18dba191d8d826d30534b4d63c276b3c3234bacd84cc8738`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:55:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:51:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 01:51:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 01:51:13 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 01:53:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 01:53:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 01:53:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 01:53:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:53:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 01:54:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:58:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc27456075680427d55e79ddce0ccec278d1f81ab5181d13386de5ac3f085b90`  
		Last Modified: Fri, 02 Jun 2023 01:02:13 GMT  
		Size: 818.9 KB (818915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c91ad7650f55a57d952458067fa5d43fc42f60aa1300eac0321468efd7f1d`  
		Last Modified: Fri, 02 Jun 2023 02:17:44 GMT  
		Size: 4.9 MB (4878354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56880df8951662a18430445a0e7468b38fa19051e1a794dc42acd993c654fd7b`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c446f0efbdf1c500e962b4679d40098c4c78b579337a83db9751a38b81af7977`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca30d8fccfd9d0b20ea4671a7149e2fdeafd9ee437142de1c9258ee630cc8a8e`  
		Last Modified: Fri, 02 Jun 2023 02:18:15 GMT  
		Size: 259.6 MB (259624496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ae89dc938d7ae36da910586975ad26b87e5df2518d41458f036579d59e3bcc`  
		Last Modified: Fri, 02 Jun 2023 02:17:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b828d11571bf9a2dc34d01f3e018cfbed980a688e0eb6fd7bdf4d501881a0ca`  
		Last Modified: Fri, 02 Jun 2023 02:18:33 GMT  
		Size: 70.5 MB (70459587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7216ece951b98edd7bcceb7db17617751c38d6588b4d2d74d8a7eb422c043f9`  
		Last Modified: Fri, 02 Jun 2023 02:18:23 GMT  
		Size: 283.5 KB (283472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c51a5623d92bc9baa994ddf65fae7b7f119507f0ff98b7153b8366b19881542`  
		Last Modified: Fri, 02 Jun 2023 02:18:34 GMT  
		Size: 75.0 MB (75000399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397b7c71c1be86e2bf8ae268cce09ff4347e4d71c72e1711c7aa099ca1d1510`  
		Last Modified: Fri, 02 Jun 2023 02:19:38 GMT  
		Size: 305.7 MB (305703271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:06e5ec5b16d971455af1a0510658fdec5b94c3a1eb948d1fbcd2b26c7ee1ef23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **646.7 MB (646699906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c5a16eb2ff6b4abe2b15548e8e5347eadcd4641965013edf87bc88886e80bd5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:52:11 GMT
ARG RELEASE
# Tue, 30 May 2023 09:52:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:52:12 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:52:20 GMT
ADD file:d570ab6bd7d664cc6547b6ae228cf825333d9d841969911c7d62afe3ed440803 in / 
# Tue, 30 May 2023 09:52:21 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:03:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:03:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 02 Jun 2023 00:03:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LANG=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 00:03:53 GMT
ENV ROS_DISTRO=melodic
# Fri, 02 Jun 2023 00:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:03 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Fri, 02 Jun 2023 00:07:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Jun 2023 00:07:04 GMT
CMD ["bash"]
# Fri, 02 Jun 2023 00:07:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Jun 2023 00:08:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76bc0c6b06fc92c1f911be6147b55b6430301b80e4062178329c4fa8a0f79f51`  
		Last Modified: Thu, 01 Jun 2023 23:54:31 GMT  
		Size: 22.3 MB (22312178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f87f37d6a7831a2d27cf9ba67dbb404857632b477ce335ecbe521cd84db2d`  
		Last Modified: Fri, 02 Jun 2023 00:15:23 GMT  
		Size: 820.3 KB (820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a424966fc7947ef55ca4db8ed69abeb762dbe613d82cb7b6c248b55d4a76fe8d`  
		Last Modified: Fri, 02 Jun 2023 00:15:22 GMT  
		Size: 4.1 MB (4090754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f2b5759d6a592db8d9e7c54cea41255e28a308bb00dd901b0b89e127833484`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe4f77d9ba9445f2717bc343def12bf6a5abffaaea9978f6a7cd08e9dfdd96`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed06e4959894fd0c27932146a90ade048f580b919f2003dc021fe1a3b771c7`  
		Last Modified: Fri, 02 Jun 2023 00:15:54 GMT  
		Size: 239.1 MB (239083601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028706c953b925fc2ae8b0353286f1e65b796003820978cacf6b3fafd5b523d3`  
		Last Modified: Fri, 02 Jun 2023 00:15:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6586e09f1cb6a3e98681e7381415216b056728fc1638e63d0dfb7185bd95e`  
		Last Modified: Fri, 02 Jun 2023 00:16:10 GMT  
		Size: 55.0 MB (55033923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0b06f450c92b4d108057aa9ea1678dd83381dde934812520c7557e827262f`  
		Last Modified: Fri, 02 Jun 2023 00:16:03 GMT  
		Size: 283.5 KB (283459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e9ec93d69d137562906fd1dfdef9c60300d24a8dc97255f8d2d9621b30a922`  
		Last Modified: Fri, 02 Jun 2023 00:16:13 GMT  
		Size: 64.8 MB (64751236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594b3855b25b075922bf634e58c144589bc3d8b64d02fa234977253e79ce764e`  
		Last Modified: Fri, 02 Jun 2023 00:17:10 GMT  
		Size: 260.3 MB (260322573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:449681c53ff4136c59d6a975ac4478e4a736aa89f0d0c676eb688afda5ccf294
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.4 MB (704353620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564d239811a89435a03b6cfe936fc147f9e68c53be7fb058950ec8a851fd07a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:07:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 00:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:54:30 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Mon, 03 Jul 2023 18:54:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 03 Jul 2023 18:54:31 GMT
ENV LC_ALL=C.UTF-8
# Mon, 03 Jul 2023 18:54:32 GMT
ENV ROS_DISTRO=melodic
# Mon, 03 Jul 2023 18:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:00 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 03 Jul 2023 18:59:00 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Jul 2023 18:59:00 GMT
CMD ["bash"]
# Mon, 03 Jul 2023 18:59:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 18:59:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 03 Jul 2023 19:01:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 19:07:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5d58f6c858f92b45f1d3e366bcabef3c6821ccaa9ee17c59beb643029cb4d`  
		Last Modified: Fri, 02 Jun 2023 00:41:19 GMT  
		Size: 819.0 KB (818994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e738cf9edf30ed3cf9686d84733d2d3d3ee28a85c58ada09fabd9660ed336`  
		Last Modified: Fri, 02 Jun 2023 00:41:18 GMT  
		Size: 4.5 MB (4461671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb15c91065685951357c563d50225475bf62ccf00e185b08b5d5aa0d828f9e9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddaf40387f745b8b6c023a4647f5ce4a9f784107d4ba1d4356d41f6ccd21a5d9`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 2.4 KB (2404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d28df4590da4d1b3e217e5b8b28fed95ce13c54228ee8335465c1b72839ef3c`  
		Last Modified: Mon, 03 Jul 2023 19:09:17 GMT  
		Size: 252.5 MB (252524042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffda3f020806b222794eaaa7b5f1cf412f7ebf13aad2e650fd36980f6649787`  
		Last Modified: Mon, 03 Jul 2023 19:08:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce65a51b0331e8a1ff1c5bd34f6cf61bb21789c246ed43c0465eecddf10e14`  
		Last Modified: Mon, 03 Jul 2023 19:09:32 GMT  
		Size: 63.3 MB (63279594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5c3f121b18d97b4bd63e2476c9c60549acd8148c5c11fd04bd08f5c70d877`  
		Last Modified: Mon, 03 Jul 2023 19:09:26 GMT  
		Size: 284.8 KB (284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a658836e677ca17fd290d1d7bb810935536e4e53a459435294c426cad64b3`  
		Last Modified: Mon, 03 Jul 2023 19:09:34 GMT  
		Size: 67.2 MB (67234662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598fa718252c092ab10ae79ff168cc8abd04d179e020bdaeb6c1dbca1aae9de0`  
		Last Modified: Mon, 03 Jul 2023 19:10:26 GMT  
		Size: 292.0 MB (292006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
