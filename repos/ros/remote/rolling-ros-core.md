## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:2adbd236585a2b254fbef29dc4b788157ce3d4c2af8511f14b883215453183c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c9921f9a67468c9f71bea0ea8bae126f4cf407ab367adcaa37cca8e8cb438c4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155665688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26eb1d55ea08d3da76bccaf3a8a5ae07b8a8732340dbdc3ec44a22f87ffd7b29`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:23:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:23:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Mar 2023 04:23:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LANG=C.UTF-8
# Thu, 16 Mar 2023 04:23:54 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Mar 2023 04:35:49 GMT
ENV ROS_DISTRO=rolling
# Mon, 03 Apr 2023 23:22:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Mon, 03 Apr 2023 23:22:12 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Mon, 03 Apr 2023 23:22:12 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 03 Apr 2023 23:22:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad1f8f26857dba14fd27f7d8af8cd5f9ce4c25d5e4264090e4e33665838f4a`  
		Last Modified: Thu, 16 Mar 2023 04:47:17 GMT  
		Size: 1.2 MB (1169612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12f0c8d10d787a739ce0beb1339ad34542095ac563892b59872c9b9229991`  
		Last Modified: Thu, 16 Mar 2023 04:47:16 GMT  
		Size: 3.8 MB (3828398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f122dfff7592e93555f020a3ba95ce2e1d60b0b138d39e444d80b29e1fdce`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c195d49a74ea3cc9e44dd424ab6c5a62643eb9cc1fd60c335335d24eaee3fd`  
		Last Modified: Thu, 16 Mar 2023 04:47:15 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406973cc1afb21645698bc7cf99d59709094c778a695225530393d37f1efd4ef`  
		Last Modified: Mon, 03 Apr 2023 23:32:42 GMT  
		Size: 120.2 MB (120235298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f7cbea03df781b97c2e3b15b36c82aa25f249e4db3d062359ee77adda9aed`  
		Last Modified: Mon, 03 Apr 2023 23:32:23 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:663e17236101e1d8f141ac251ca5e046c605f691ba727fb74a709a26beadac90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155023347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b58fb0655b5f92256fd045d234b0538c79618c46802a2f44fa90d7aa45a0c1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 18:40:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:40:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 03 May 2023 18:40:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 May 2023 18:40:43 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 18:40:44 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 May 2023 18:55:25 GMT
ENV ROS_DISTRO=rolling
# Wed, 03 May 2023 18:56:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:56:10 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 03 May 2023 18:56:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 May 2023 18:56:10 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe39e5ef2f67d96ada5275fbc781d159428991d033cbee5a50e0b5b94ed1764`  
		Last Modified: Wed, 03 May 2023 19:01:25 GMT  
		Size: 1.2 MB (1240441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271495fcffa1108252b6f2555e695bf0ad66a1468909a8461002e1a31a1c23b`  
		Last Modified: Wed, 03 May 2023 19:01:23 GMT  
		Size: 3.8 MB (3800745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2e07c8e039094a3d58f02821bc3eff246bf32f8fb86ff03c65a9bde2bb7ab1`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb152ff223d153fa6d0817fe489190d70fcb6dd9df7b5d1a7163ac27e0fb090`  
		Last Modified: Wed, 03 May 2023 19:01:22 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344fd0345199b732007d1fd801848c7f86eaadf910174213af53e56be4d95dea`  
		Last Modified: Wed, 03 May 2023 19:03:41 GMT  
		Size: 121.6 MB (121590308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b879cb6b4af64e18cfa7544975f71141f8047683cf7dbfbfd66f5f2b7a64d26`  
		Last Modified: Wed, 03 May 2023 19:03:27 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
