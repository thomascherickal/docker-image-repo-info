## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:26ab3d4f0c179600d532cddb3e7a302bc078b8832c5326b005f23d90ec294ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:9c5263688f810644ca2b574aaea20528a8854a7824aded3f8bcac45e4bb1cfff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.0 MB (291990947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5895e7229f09cdc6495dce8551b0f865b3a8512108c62c987bc4149b0409143`
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

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5f3987ab48ccd606364b53d6c197c52dc936598e195011659206011bbb722bc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.3 MB (266260149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e51dfcdecf577d494317e257a7779e5f06d3e8a3afec9f43f4847d650c7f0297`
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

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f4fdb424228f37cd137ffadf7b95bd312186d5f425c4d1ae7631c8acab304086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281564631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748356f92137700ffc2e8451c39d156388a6474e6e4aafe39f6a49c3c69a2cfe`
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
