## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:bc12f1bdb6b404e520da458ab68338a9fb27f66d3be680e1eeff284419f83821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:a956ed38fe8397f86ac8c9147efc1dc750606b2e4ec62418ae2bfaf1ec5300da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.7 MB (840663651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3c6313f3972995513a0d6c3dc5a3884b4ad432be54979a96e0d3f25972f26fd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:36:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:37:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 04:37:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 04:37:15 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 04:37:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 04:37:15 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:39:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:39:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:39:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:39:49 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:40:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:40:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:41:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:50:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a41ae3b013398d2c13b5bceb3338e9582560c6d0ffd908463d766628be0a9c`  
		Last Modified: Tue, 31 Aug 2021 05:02:39 GMT  
		Size: 1.2 MB (1182916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8296a87df0b7498eeb5c80b365dfd866191372bea87427717ea787d78a5a7`  
		Last Modified: Tue, 31 Aug 2021 05:02:37 GMT  
		Size: 5.5 MB (5547451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99851257d3d0d2af7b11c2c45f1d102b8c4afaba687a286b13733fff91617ad1`  
		Last Modified: Tue, 31 Aug 2021 05:02:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301bee90670066d34cd712db73dc54fd8483644f7ee1ca01917630b7c3426e7`  
		Last Modified: Tue, 31 Aug 2021 05:02:36 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853f7eafaf492a87fe6a6a39ea78b0ea439052fe7b2e9438def69dbbe0b5692a`  
		Last Modified: Tue, 31 Aug 2021 05:03:05 GMT  
		Size: 176.7 MB (176709798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a0a941c4ee49c2f1d73dda50251237a23b05f95a0c923dbb787d434f98f49d`  
		Last Modified: Tue, 31 Aug 2021 05:02:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36cae12ae4fd3e4164478c14996f207e6a1a67f86f96a3fe33f2f3219d23a7`  
		Last Modified: Tue, 31 Aug 2021 05:03:24 GMT  
		Size: 47.3 MB (47259633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa4091a6d76df14f052f72f6c4b56cea6f82d72161748dded90d5ee4e151b85`  
		Last Modified: Tue, 31 Aug 2021 05:03:16 GMT  
		Size: 317.9 KB (317858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e1c66b7b2cab748988f9f11fedb7b035f9a6cd68d50f1302e32c9e775a5f00`  
		Last Modified: Tue, 31 Aug 2021 05:03:29 GMT  
		Size: 79.6 MB (79602869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d590ccf7b12765b090b9c84fc65ad1ec8f11fb171a676c3160c685d2abeaed`  
		Last Modified: Tue, 31 Aug 2021 05:05:09 GMT  
		Size: 501.5 MB (501470636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:f40be954b42fdbf2c8658b0378454aff44e042a9dd0cd047fa1faf526993e0ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **730.2 MB (730245800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d65f25fc22d5b0aa108a74c05817159af01187025e7ef2e0e00644a7274356`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 04:01:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 04:02:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:08:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7610242426bc226b21c63941458db4760063f2536207c80d92f79642ede166d`  
		Last Modified: Tue, 31 Aug 2021 04:20:05 GMT  
		Size: 36.7 MB (36691316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d75fec186326e68092c8c944a4991cf20df280505668146aeab88ef75f42f`  
		Last Modified: Tue, 31 Aug 2021 04:19:46 GMT  
		Size: 317.9 KB (317853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891bd701076db5d3efe95bd46c285b538fbf4d20a17a3fdde54216d561a397d0`  
		Last Modified: Tue, 31 Aug 2021 04:20:24 GMT  
		Size: 60.5 MB (60482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb6760ee5d1314fbec6f42620c54f10eacb13ab219ff411714d6e2706987a45`  
		Last Modified: Tue, 31 Aug 2021 04:25:40 GMT  
		Size: 445.6 MB (445606636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:78cc89e14e3a8e59a88f8843fd284b27ba8c94ffc993b9b54218ec8b5d3c0173
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **790.9 MB (790931348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6860a9d9d5f78146fef318e473ef718697431dbddbfda597f4d0f30025d7f49d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:35:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:35:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 02:35:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 02:35:49 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 02:35:49 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 02:35:49 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 02:36:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:36:38 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 02:36:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 02:36:38 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Aug 2021 02:37:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b869ca97320a7af4e9ce7c382543a1b04a7005c70779507cbb85ace89adde42e`  
		Last Modified: Tue, 31 Aug 2021 02:52:34 GMT  
		Size: 1.2 MB (1183579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7b498b8e70b033b401f685710eb46ada1aab199891dfe061488eb0ba40831`  
		Last Modified: Tue, 31 Aug 2021 02:52:32 GMT  
		Size: 5.5 MB (5512786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6b11a7bb7f78e22996a184b764b32e64f3f4ef7d41dc571d55d606cc1a6ac`  
		Last Modified: Tue, 31 Aug 2021 02:52:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aada428d5fc8dcbd529a9a5a2d09d46e75fde1b0cad9c895dfe9e81109657ee1`  
		Last Modified: Tue, 31 Aug 2021 02:52:31 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca561674e29ba9be5ab00aa2dc9f3cf19a9b9c521d7e84bebdb5c285317079a`  
		Last Modified: Tue, 31 Aug 2021 02:53:09 GMT  
		Size: 171.1 MB (171148029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee245aab371139d97caaba068958d119f132acdb5c08cec9c17f2c9db9c6ce`  
		Last Modified: Tue, 31 Aug 2021 02:52:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785f6e4808b7908f861bce0cbf08dedf895e579a5474fd9fab133bcc56f92549`  
		Last Modified: Tue, 31 Aug 2021 02:53:29 GMT  
		Size: 41.5 MB (41520808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b50ac425df80624b0f3931e6c262c69b4b1e63d9bb4966fdb4b22e4ceb822e2`  
		Last Modified: Tue, 31 Aug 2021 02:53:21 GMT  
		Size: 317.8 KB (317842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dccd1599a0df6b5e1eca72b82a800e27f6062c6d12cbaab8fdcf7bb3117962`  
		Last Modified: Tue, 31 Aug 2021 02:53:34 GMT  
		Size: 72.0 MB (71972726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3ef8c38235c8c6ae3688876b8bcc0e9d6553d110e1210573b9b1216603b0f8`  
		Last Modified: Tue, 31 Aug 2021 02:55:21 GMT  
		Size: 472.1 MB (472100065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
