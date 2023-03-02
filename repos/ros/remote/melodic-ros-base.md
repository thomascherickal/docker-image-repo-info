## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:2b3882e1f5797d6595a18e66f892fc51d274bdfb938189f5d36b01d82bcf01a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:93ff17f047b26c4000ff1e18878fa6b7a9382144a3c7da9a35ba6a91daa48f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.6 MB (437556445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d941256e42ae81c23437fb91cad81c68d0add57857c039dd828856052add40e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:17:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 07:17:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 07:17:41 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 07:21:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:09 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 07:21:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 07:21:10 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 07:21:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:21:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 07:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d3083a206086f721888a54dea32baf21c2cbc9155b39a9bac8631b20fede9`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 4.9 MB (4878631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3996b56577fbab1f217c1223e4ebab884c63ce1386b54be8a894044ad014a1d2`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff9d7fdf49d225218831b48c5847ebec87cb5bf3ea8cf9ab3eea0d1ef0e50a3`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e996788e40044c1f9c625c87249f7c8e303e5b8ed46020cad2d20e09982229d`  
		Last Modified: Thu, 02 Mar 2023 08:02:00 GMT  
		Size: 259.6 MB (259580317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9e9a8cb8917a1575d0a91f4e93b6a1d90ce64013c9d9648ad09eb9ef72e24`  
		Last Modified: Thu, 02 Mar 2023 08:01:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360c9e013d6493daea567582a2a448f49a706cf4fded3acfd62c562004627daf`  
		Last Modified: Thu, 02 Mar 2023 08:02:18 GMT  
		Size: 70.3 MB (70267262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11487da93620b5bdb7d2f78eaf417d53227fed9b51f79df5cbbbdde4cd0da6`  
		Last Modified: Thu, 02 Mar 2023 08:02:09 GMT  
		Size: 297.5 KB (297495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5f20223785c1f0757781aa7972ae767a9cbe64b3311b544ee8051d7e6a4c1`  
		Last Modified: Thu, 02 Mar 2023 08:02:20 GMT  
		Size: 75.0 MB (75000741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:e44ed680e0f8a8017636396ffdd9014c8c8942aee80f5aca1a37be4933236ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.0 MB (386040880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9ff6e7934d64730587cd2da4d4ff2af00304d1805a1dc514b9be9dec6fd9a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:12:28 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:12:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:12:28 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:12:32 GMT
ADD file:69c0e030717df18a709c66c528354d7f774a9ec9299f6492fb8ee79990ae36ff in / 
# Wed, 01 Mar 2023 03:12:32 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:59:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:59:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 11:59:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 11:59:43 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 12:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:02:56 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 12:02:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 12:02:56 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 12:03:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:03:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 12:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d135ced6a86bc1c2ad6bb917f597c1ebde88181cbedd039f2c3cb656aa79d00`  
		Last Modified: Thu, 02 Mar 2023 11:54:28 GMT  
		Size: 22.3 MB (22304070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b0874a47238c32833a1eb83551fa898735b969e33ba525c389d76a5973f18f`  
		Last Modified: Thu, 02 Mar 2023 12:27:23 GMT  
		Size: 819.1 KB (819062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca96c8d5fedefbf017ce0e41cecd02d40bb2d5b9093183b5889473daeda03`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 4.1 MB (4089642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c69e7b7b6ea014cc49dc25e4e3ad18bcc240bc2e96cd077a9618bfab8816e`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a769aaaa6a5a307f498af8c8bc3c3992f64f37b6d9f716dc2c0eddf7a13c2`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39727381991a44c63174e1b8193e9cc4386b91a936cca3b942c67cb58012e6d7`  
		Last Modified: Thu, 02 Mar 2023 12:27:54 GMT  
		Size: 239.0 MB (239045530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134249505ec9b290e4986fd60e7b3bf9da3ea895cf2609ef3b8a4f9ced66eead`  
		Last Modified: Thu, 02 Mar 2023 12:27:21 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f49c73b5c2e574db7cbb840ea3132a051626d8ea7f869ead59ebd1b8448f601`  
		Last Modified: Thu, 02 Mar 2023 12:28:12 GMT  
		Size: 54.7 MB (54733714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a64e4ebd696ce4cef7a0e94e6fa5022a1d218ed4f1ec9fcc479ccb03dfb26`  
		Last Modified: Thu, 02 Mar 2023 12:28:04 GMT  
		Size: 297.6 KB (297553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce032e347c9e1d2bbe0065495e4253363c1c7d7f8bf6a27570b03729f482058f`  
		Last Modified: Thu, 02 Mar 2023 12:28:15 GMT  
		Size: 64.7 MB (64749464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e270a7432c93f738fb6cb42ae04726c84dee53c855f2cb43c9fae71d373a7a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.2 MB (412192920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afc8882704f4a7b5cd865f8bffa9416bc6ddb23ffdf7cbf0d0a81e4be623b99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 03:17:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:17:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:17:55 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:01 GMT
ADD file:0061a9f9e2cbc9ae8577d57391acc2948389599590aa542eedf9a6b8cd0f79b0 in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:16:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:16:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Mar 2023 03:16:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:16:20 GMT
ENV ROS_DISTRO=melodic
# Thu, 02 Mar 2023 03:20:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:20:16 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Thu, 02 Mar 2023 03:20:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:20:16 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:21:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:21:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:22:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9de1bca73074c336fb93a7688a40903c720a195929a0da27bd4ea424d5817c78`  
		Last Modified: Thu, 02 Mar 2023 02:09:51 GMT  
		Size: 23.7 MB (23733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcb6c39567ec9b2c7ea7bca3bf033f2f41f3a4c07d089b9de2d8a14bab3292`  
		Last Modified: Thu, 02 Mar 2023 04:04:42 GMT  
		Size: 818.9 KB (818853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c5391c267d74199876bc0f614d5b80ad1e03948938fecf4d80e0ab49f7c90`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 4.5 MB (4461697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65a69abc68e01cb3f3e8e00001fc0ff966cd84b753e82111e495e9d319ee03d`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b151a1078cd0202754dec71f67746b6c116798ceaaec93e1fd31ae3fd305b501`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a2b2ae19293c39a9abe7ed81542deaf9824db2f84b81e2cbe87c4b55e01fb8`  
		Last Modified: Thu, 02 Mar 2023 04:05:13 GMT  
		Size: 252.5 MB (252548696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae119db2c7c4ffba52e20aea0bf61b6e9bb6a81bb69236b7177610e3d8d3faf`  
		Last Modified: Thu, 02 Mar 2023 04:04:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf304e76035eea24e63c6f8df3b3226e6af34ae05635d41819e5084f1ad6717c`  
		Last Modified: Thu, 02 Mar 2023 04:05:28 GMT  
		Size: 63.1 MB (63096257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce94d2b7b5f6ce75418a3f1a7754706762dc89fb5ac7ae79de0c100223e5b594`  
		Last Modified: Thu, 02 Mar 2023 04:05:22 GMT  
		Size: 297.5 KB (297502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75def227e2b8440db3d1998106b192c98342ceab881d620f4a43be96b5876616`  
		Last Modified: Thu, 02 Mar 2023 04:05:32 GMT  
		Size: 67.2 MB (67234530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
