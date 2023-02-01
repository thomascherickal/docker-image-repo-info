## `ros:noetic-ros-base-focal`

```console
$ docker pull ros@sha256:3e95165652987da802b4b70b24a5e68da5381de86a3ee5b5b73a9566c7b0abdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:093dfb05e09d5198362a3f1a69e887c0873c1311bf065fb33816fdc73989743c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343190067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9a9bf50e26daeaaee850bb232ed2a4376df3419ca4ef731987d5afbb0fb13a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:30:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Jan 2023 19:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:32:46 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 31 Jan 2023 19:32:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:32:46 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:33:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:33:31 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:35:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804981d9bf482904db4b4d104296f3927c0fec21315768200c549e60779cfc1b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b32c4d8969e5d55023be486caf122cd9d5087fe207766e38640e00eef95b89`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8112d9bcc28c8015cc517eaa9d8fa13b7f81c56a16cc1ad99377486ea883d1cc`  
		Last Modified: Tue, 31 Jan 2023 20:09:10 GMT  
		Size: 177.0 MB (177012436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69af09dbb1547496b02120dafb830cdca8c96bb6f57f6c825d29cabbe61bcc9`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6d27d12c31896425b068abf5aa177ae41dfa12615cf7d2ab85f7a9d4e409c`  
		Last Modified: Tue, 31 Jan 2023 20:09:27 GMT  
		Size: 50.9 MB (50939989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d0675f14db1e48e7d2d1368064952427c6f9db0a5f0a4041fe0529c67da8d`  
		Last Modified: Tue, 31 Jan 2023 20:09:18 GMT  
		Size: 342.5 KB (342485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c42e45b24027e16138a0b07603a15c2800a3a4961df245293946b7ae01dd37`  
		Last Modified: Tue, 31 Jan 2023 20:09:31 GMT  
		Size: 79.6 MB (79606644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea8683583e242df0297c9b3921ae5cd4a67ce45139a231f5cd59186407b2af91
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289276893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5790bb8151cfbe7c196aa9550d6d53fdfb33e9fb064738db698e49a610ff4b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:28:35 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:28:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:28:36 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:28:43 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Wed, 01 Feb 2023 11:28:44 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:40:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 18:40:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 18:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 18:40:54 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 18:43:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 18:43:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 18:43:08 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 18:43:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 18:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d38494d0ff859e08a20d76b60e8639e7e35ad96ab3b04e66d13a2aaba579`  
		Last Modified: Wed, 01 Feb 2023 18:54:09 GMT  
		Size: 1.2 MB (1154619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a2dff765a03ebe05aa136562726b90b245f2353ca418465e2a7732d11eba74`  
		Last Modified: Wed, 01 Feb 2023 18:54:08 GMT  
		Size: 4.7 MB (4679046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f825ebe5ff085753f3efcb043a5f188152a8e93efb957b7a80dacb0a5935667d`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c29fa2aebcb932b5c4cabe32cfab431e7a304b8771a491de3a04ee20bea9c60`  
		Last Modified: Wed, 01 Feb 2023 18:54:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05665683cdbff07eaf530ef1f7ffcfae8735da02f891050c5b7fdb4dc3d249d5`  
		Last Modified: Wed, 01 Feb 2023 18:54:41 GMT  
		Size: 157.5 MB (157513162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce443632c832866bdb905b5064d93c75053bfab8f7000948308e7145f06d00`  
		Last Modified: Wed, 01 Feb 2023 18:54:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71e93a572f5afe612d28c2770c1bbe9d3f8ae07c63c18564f57ecad266fc4d1`  
		Last Modified: Wed, 01 Feb 2023 18:54:59 GMT  
		Size: 40.5 MB (40502372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a3f4210fa6dc76dc5ea517dc60112d9a6198feec091e04ba7ca12918504e9`  
		Last Modified: Wed, 01 Feb 2023 18:54:53 GMT  
		Size: 342.5 KB (342503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f0c865e9957fd97c112c32e13bc25c430fa69c1f13451d1181eb01b9964b6`  
		Last Modified: Wed, 01 Feb 2023 18:55:04 GMT  
		Size: 60.5 MB (60496457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87fe54a6ded5be95e141e9a11f8bd23cc13088e3e01244cf46c98c1e807e72f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d3994a361be4ea5cbd11474d8877364831d3bedc228ad3ac2a76e8d7ce7eb1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:14:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:14:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 01 Feb 2023 19:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:16:52 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 01 Feb 2023 19:16:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:52 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:17:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:17:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:18:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11990ca89946b756459e20c82f5fc261762d88e876a1f0c27eb98f53d9153fb2`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b170ac8cf94364aab1121aaf45d3688ff63fbce08a0782fa4d85e8e7d732259e`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80cc2bb1bc502e7e227bea5135ae1c886b723f01a277660913b6aa73010f374`  
		Last Modified: Wed, 01 Feb 2023 19:31:12 GMT  
		Size: 171.4 MB (171445562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0dc1f7d500c6b071331b1a17db16f89a772224e3481efdcfe4bdd03544c481`  
		Last Modified: Wed, 01 Feb 2023 19:30:49 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f807d9f223f664ac6195a8bf1e925337c9764ab6bacef01913205b446356cb1`  
		Last Modified: Wed, 01 Feb 2023 19:31:26 GMT  
		Size: 45.2 MB (45203022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000cc58540f38d23dbdee1770d2662efd9e3ba1bb45d80f8c947bba6bd616e91`  
		Last Modified: Wed, 01 Feb 2023 19:31:21 GMT  
		Size: 342.6 KB (342564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb784b7cdf9eb88f1483d6ae533e2cf9ae323876fe36f32475a2254b28de75`  
		Last Modified: Wed, 01 Feb 2023 19:31:29 GMT  
		Size: 72.0 MB (71973643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
