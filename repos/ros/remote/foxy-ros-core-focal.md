## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:fc0710a38383b8ceabe029a87b522a975c13f24edf4859d6ffb0cf850aeeb440
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:2e19996a9381e3f98d5dd5681f4d4e4aab8e91764b6644537b226b82f7690d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155642679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d5695824b395ad401e6c40f70e642860f157682ac3881d682e1d3c06ee529c`
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
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
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
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8d993a8d8ddaab94f857c7eeea4817209d7fa3f7f0028b82cd0810202243ba2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138440709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd69454231214178e8a50eb5ff795a92a57d203699ddd932390f3126d6bf8dc6`
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
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
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
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
