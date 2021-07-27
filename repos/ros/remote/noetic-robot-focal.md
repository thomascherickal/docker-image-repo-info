## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:69f0203828c107fed52e9f54ba7a9e8636eb2def2879fb104935030394513601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

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

### `ros:noetic-robot-focal` - linux; arm variant v7

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

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd9e4dc5a97b8683c3165e7d8794162a65533b496812c94d5d84f4c2626047f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334167154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4f1f852293947f134b97038a717079ef453df5e42114df4ee741ebc96891fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 23:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 23:03:31 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 23:03:32 GMT
ENV ROS_DISTRO=noetic
# Mon, 26 Jul 2021 23:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:25 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 23:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 23:04:25 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:04:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:04:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:05:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47ae118bf19cf825ac83647c1d65d099e24417c73620e6553806e36aa26d8c5`  
		Last Modified: Mon, 26 Jul 2021 23:20:22 GMT  
		Size: 1.2 MB (1183453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74becffb9ea2d3b903303692f91a3abc607df25339bd7464db56343eefb622e`  
		Last Modified: Mon, 26 Jul 2021 23:20:20 GMT  
		Size: 5.5 MB (5512652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d28ea46fe795b56172879ee97757cb6ea98226a43662f62f5bd8e1490c4fb`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1b73a67b1165693bd1ae07bace3301ab4fb82cfe1b5e61e2b536d3e2f75e47`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2161207e597e1e7621916bed37a91d2ed819071ecf81902fa5f9a199d8581048`  
		Last Modified: Mon, 26 Jul 2021 23:20:58 GMT  
		Size: 171.1 MB (171140053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab310c95b66fdb5ac105888d128d19608c8cd336dad6a23a85eee7e7b3a3e8`  
		Last Modified: Mon, 26 Jul 2021 23:20:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a92eab614e3b9eeb6dafa9c74d6549e3f0dae57bdac2230eb29df020a27579b`  
		Last Modified: Mon, 26 Jul 2021 23:21:20 GMT  
		Size: 41.5 MB (41520773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122ab38b7bb1545dc49ffeead82d684f27e43bd0881738800aa0c8bb84590cde`  
		Last Modified: Mon, 26 Jul 2021 23:21:12 GMT  
		Size: 313.4 KB (313419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0468d318c5f7ccddaa45f1306287d14921ecd8e72c5a532713085cbfde2131`  
		Last Modified: Mon, 26 Jul 2021 23:21:24 GMT  
		Size: 72.0 MB (71972776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c66dec020980c4a0606add91e864f375b616437dd803afd9fe6259f3a6e3ef`  
		Last Modified: Mon, 26 Jul 2021 23:21:44 GMT  
		Size: 15.4 MB (15351357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
