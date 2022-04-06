## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:7247098894b5b8f8d4ff67e979fc54c7018fcad0ca671c47c52ac01fbceae3e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:1625afb24a4b2845e6fe57ca3b68eb72790504fe3a60cc825b7c6c1f46bdc166
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291879437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6302dcf86949ca52c7d76fd0959130adb1b2b959902b5b1a33fc4af97a46f894`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:41:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:12:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:12:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 02:12:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 02:12:29 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 02:12:29 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 02:12:29 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 02:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:15:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 02:15:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:15:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b732c52c0461890d4114ac1d6f5a90dc52c395a65c4bd758b0c8ec6d738eac1`  
		Last Modified: Tue, 05 Apr 2022 23:59:27 GMT  
		Size: 838.9 KB (838902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656b41acd8def5851e0236575b2ccbf5ee29c14393fdb041320f87b027121b91`  
		Last Modified: Wed, 06 Apr 2022 02:43:13 GMT  
		Size: 4.9 MB (4872183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c31bef3c8aea03bf71158539e4a26a0e727f69f59f36cad07a341c67386dbe`  
		Last Modified: Wed, 06 Apr 2022 02:43:12 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d8f3301e951a7dfb9cdbab62a9aac23cb0a8a720896539c823bc63779b6dc0`  
		Last Modified: Wed, 06 Apr 2022 02:43:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20428422782224ecc939df68824f15aa7ee865a5d8e9f903d7b937641b4f123`  
		Last Modified: Wed, 06 Apr 2022 02:44:00 GMT  
		Size: 259.5 MB (259456999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8708c288ed99d371db1e1762210ab955ce82139acb17447766a6f8ce668db0`  
		Last Modified: Wed, 06 Apr 2022 02:43:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:108a9eba9023a15c84ff0c3de4b6bbaaed7d3b5d0a7dd41a9d54fc9629783560
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266164784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ec9de21be64c0d590eb0ff8c18840aa6a6860e1555ea9c5493fc31d4ca94e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:25:38 GMT
ADD file:3230d8a499e37ff816595cbac3892a80005afccf8a55053c28e24989d52de08b in / 
# Wed, 06 Apr 2022 03:25:38 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:21:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:22:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:22:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 04:22:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 04:22:08 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 04:22:08 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 04:22:08 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 04:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:25:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 04:25:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 04:25:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:419a71fa3c92c7dd0e8cfbfdf694362de1c27dafed508aeb2e5bc9ff8376fc98`  
		Last Modified: Tue, 05 Apr 2022 13:12:06 GMT  
		Size: 22.3 MB (22301415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a162be1c1e08f96d0b744482cc8ea911a59b5c915fff0f162674de69d7dfec01`  
		Last Modified: Wed, 06 Apr 2022 04:44:24 GMT  
		Size: 839.8 KB (839819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ff94372f98929867eb27c75aacf2dcb73c9ebb69048809947955507b28e457`  
		Last Modified: Wed, 06 Apr 2022 04:44:23 GMT  
		Size: 4.1 MB (4085911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0937b2511b635d32459e8503e109907f45c153c0bba95cac38bd7b919ca97df5`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f184306a6b3e4850d73085a52f44ae5d7109134640429bb555ed064aa2ccb09f`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e6e094f9f6f883c0c73aa3d5feac7a3f16f33d067dbe521f52633b79ad0fc7`  
		Last Modified: Wed, 06 Apr 2022 04:46:56 GMT  
		Size: 238.9 MB (238935223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a3ef67c69ec977d8faff06a9220e6e78ff582bf828c458605a4510e0764d0`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33d2cbb7047d20b67dcf0b2fff7728a300f56475a30dcfbbe5724195e3ab8c9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281218153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4e9eb6cac1a79430e37b149143cb842cf64b4add41eeaa5da6cfe44c849d787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:51 GMT
ADD file:bb36cf2c131b65fcf3f10eac5cb640ad749d77110482b30bff982a284aa9e9ec in / 
# Tue, 05 Apr 2022 22:40:51 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:02:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:02:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 00:02:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 00:02:15 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 00:02:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 00:02:17 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 00:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:03:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 00:03:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:03:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d35feac4abe85b38af36ec148f2c2dc7a795f9862a0b6dcf2a1511b752a44996`  
		Last Modified: Tue, 05 Apr 2022 13:11:37 GMT  
		Size: 23.7 MB (23730866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cafe3bc9ff724c70f720ff738c3e724cfa285eacc5756b11e4ec83f883d345`  
		Last Modified: Wed, 06 Apr 2022 00:22:28 GMT  
		Size: 839.7 KB (839677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e7b86a897351a28097247359d6d356b04139c42ff35871c740b3a2a7a5380`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 4.3 MB (4264068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7784583ca0c82d8e7c3c30fc4def03aea35cd0704da7b1abe916b5de2a264e4a`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ec1168691379152172f56c4f702252d305664a82ff13917f0bda00c26c15`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e5728f7c984b33f56560ff16dedaafc3e2a66fecb6f35f06ba609e8ee8f71`  
		Last Modified: Wed, 06 Apr 2022 00:23:02 GMT  
		Size: 252.4 MB (252381175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de082d48add89480d196d0adce610edec0e7c4b754f7dd74ab3c0b9943398c5e`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
