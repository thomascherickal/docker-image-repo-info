## `ros:noetic-robot`

```console
$ docker pull ros@sha256:cac7431a907c43e4bb3bd022d806bff1f7c2370d481168407c10e795a00c8ffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:adea3cc00b209b6593981d24148705d0359e181f6c6858e92ce16d6ca06a93fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.9 MB (354908217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84870c73cac7e080a24ef027e5e15a8f787e57f2d863ef675db254f80ded325`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:04:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:06:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 02:06:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 02:06:27 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 02:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:09:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 02:09:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 02:09:25 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:10:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:10:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 02:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac0af9608ebe50db5c9883ba2cc0fb4d341457cd84787a41bcf8a4a1559fed`  
		Last Modified: Tue, 13 Jul 2021 23:17:15 GMT  
		Size: 1.2 MB (1182378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f5caef8790a621811a988200a5fd602b684440a7817c5bbcaac24368ec66a`  
		Last Modified: Wed, 14 Jul 2021 02:32:13 GMT  
		Size: 5.5 MB (5546936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc149e3ee734eaa227c577708e79be620b1cfbdc44eba44feb059be8d49971`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0c2a7ad34c303dcb8348811e3ee140f0bb94723bdea38c27e3cfa94c838602`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa62a799c06ad3c3011c26d06d55762eb5765bd81835e8989d55c8c7fc04806`  
		Last Modified: Wed, 14 Jul 2021 02:32:50 GMT  
		Size: 176.7 MB (176700701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360166355a7d9f55f98c1058cee3cef1c4ab76332ab13cf582f2993c8a40e881`  
		Last Modified: Wed, 14 Jul 2021 02:32:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6360a9085b12f4ed8ac487d8b34824d7238d62178791afce5c3528eff7846b`  
		Last Modified: Wed, 14 Jul 2021 02:33:10 GMT  
		Size: 47.3 MB (47259111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f6269c2be5c26ee8b44ee2f34dfd7425a57f8a93678ac249222838d0dda7e2`  
		Last Modified: Wed, 14 Jul 2021 02:33:01 GMT  
		Size: 311.4 KB (311426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535103c95d968dd78f20089095f78c0ae8f47704a8680927b3e321c01564d6b`  
		Last Modified: Wed, 14 Jul 2021 02:33:16 GMT  
		Size: 79.6 MB (79602525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e76fea2ad07f5de223daeb1b7ba4b90eceea87f143acb5a234ba9b0b9ed3dc`  
		Last Modified: Wed, 14 Jul 2021 02:33:32 GMT  
		Size: 15.7 MB (15736865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:60637874699daa2683541796ac4718fe8342902c616a98e3457ccca8a6cfdb4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298574628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e985262ef637bc5ae04d487a6dac768c5e674470613025d23c0428876754e9c4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:00:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:00:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:00:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:00:41 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:00:42 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 01:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:02:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:02:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:02:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:03:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:03:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:04:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:05:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ef2a91707578a7aa5e67bde1b1ee25c43d3e2005c3514859d532dabeeba08`  
		Last Modified: Wed, 14 Jul 2021 01:19:08 GMT  
		Size: 1.2 MB (1183409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f09bd680e7527c5536e3230907946a5aa58e56eb96ad044ecdea7e8de6f17ae`  
		Last Modified: Wed, 14 Jul 2021 01:19:07 GMT  
		Size: 4.7 MB (4676456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0314c569a7bfdae2ebb0dcb70368ff20da4a4641f48f7eb29871f5616511a011`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60830c62be41d8614c4359151a1187cb0f2341edefe989e8854fdf7da34765b`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cb8d0e16826782c8658ccc6b607e60dccc7a6671377b04b9ed908e42c5300`  
		Last Modified: Wed, 14 Jul 2021 01:21:18 GMT  
		Size: 157.2 MB (157205836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8c442e11344f7e8c76f4beaff7faf0c960a0067648aa8da2da8fa44fc3ed03`  
		Last Modified: Wed, 14 Jul 2021 01:19:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879dc1c1cf3f6722a9a613abfa5e2dc0d952c41aaaa0643a79a7287f61b7eca5`  
		Last Modified: Wed, 14 Jul 2021 01:21:52 GMT  
		Size: 36.7 MB (36691143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bec4f202fb03053e9739c7176bcf25a69aba7c750bb93e09640c0378cd4e547`  
		Last Modified: Wed, 14 Jul 2021 01:21:32 GMT  
		Size: 311.4 KB (311429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2883f187e8c7f1f285a7d98023e857d0c52b4914a15b2184adecc907c0795b`  
		Last Modified: Wed, 14 Jul 2021 01:22:15 GMT  
		Size: 60.5 MB (60481826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2d2e1516fd3ed66de5e7409b55f60dc3063b6a8cf213ee9e9ed34782703bd6`  
		Last Modified: Wed, 14 Jul 2021 01:22:42 GMT  
		Size: 14.0 MB (13960052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a305257d71a2d242cf088acda5b112f391dcf652eea4a79a45a2d9d6510d19bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334165507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40781401db230b03e4d695ed840b6e8f715a7737ac0e721d33efb20ffc8e5ebf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:31:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:31:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:31:28 GMT
ENV ROS_DISTRO=noetic
# Wed, 14 Jul 2021 00:32:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:32:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:32:21 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:32:48 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:32:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:33:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:33:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bd0b8651798cb4d0976958a5246313036e99ce8a86f838db32c9153fd835cf`  
		Last Modified: Wed, 14 Jul 2021 00:51:06 GMT  
		Size: 1.2 MB (1183629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f458519f531bdd6341b9ad9100e6ac84e79acb2d3004e0defa963f9aa536e`  
		Last Modified: Wed, 14 Jul 2021 00:51:04 GMT  
		Size: 5.5 MB (5512805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c16bac23518e4abf60d1c392e081256894df83fb7cddae089cfaf7131e2101`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db12b2dd1b010b5d533dcf3aafc411ceaf8c995dc98159511b4cb32f94c27c8`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f940dbd5b4415e8d2641c3154a2ae919cdc2b9fde7c70677e48453e3f349b29`  
		Last Modified: Wed, 14 Jul 2021 00:51:46 GMT  
		Size: 171.1 MB (171141545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59698e949a60aa162ddd3ef9bf411fcd75f8055472fe660a8191034d8525c5`  
		Last Modified: Wed, 14 Jul 2021 00:51:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8eff17984ce9b4d02bbb30b90dd2f14b922d2c80af7394b157c0d136aa766`  
		Last Modified: Wed, 14 Jul 2021 00:52:06 GMT  
		Size: 41.5 MB (41520897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4174f757f3653a6b2fde53f1fc1b10284fec87f13eaeb286475643d600b9d743`  
		Last Modified: Wed, 14 Jul 2021 00:51:59 GMT  
		Size: 311.4 KB (311365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84169b7479a191b9f2919dbc47e7f6a10d328878886100eba2a445d8533c2261`  
		Last Modified: Wed, 14 Jul 2021 00:52:11 GMT  
		Size: 72.0 MB (71972680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44ec7b7f6e0363e1b00715552ee9caaf2ea50968c6e8e1ba02f0b2f1f951531`  
		Last Modified: Wed, 14 Jul 2021 00:52:31 GMT  
		Size: 15.4 MB (15351096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
