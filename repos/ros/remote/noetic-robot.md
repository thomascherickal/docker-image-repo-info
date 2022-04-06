## `ros:noetic-robot`

```console
$ docker pull ros@sha256:5570a0e6b2e1afba93a776a75e858354abbd351f6f608f89c8cfb98bf4ca723f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:98b3b8474ed7ae0f2570d70027d01387a0000983e4e4292b9d8362dd8bc09dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.9 MB (358883344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7517906c00ef7ed4cfd66db1ae0cc7745a10f8296bbf10501dde42a45dce76c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:50:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:22:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:22:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 02:23:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 02:23:01 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 02:23:01 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 02:23:01 GMT
ENV ROS_DISTRO=noetic
# Wed, 06 Apr 2022 02:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:24:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 02:24:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:24:49 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 02:25:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:25:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 02:26:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:27:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbdf8d1aa53ac931cb020f1ee4ae35afbc9afcf41aa966fed51bc2848d19d4c`  
		Last Modified: Wed, 06 Apr 2022 00:01:59 GMT  
		Size: 1.2 MB (1180816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbffaa3aa803be1d98256e0c9f979dfce3a93c8d4e1e03d457d43d5b26e4c06a`  
		Last Modified: Wed, 06 Apr 2022 02:45:59 GMT  
		Size: 5.5 MB (5546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33339fde28a071d810e1014cd84398bffc468381f3a25dbf123216ae3af1d84`  
		Last Modified: Wed, 06 Apr 2022 02:45:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e2549691486b3db151ecfa73a84d0f2332b6c44e46091a8f971763113c226`  
		Last Modified: Wed, 06 Apr 2022 02:45:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0437ecd137dfa45eb78490e0b6aab0208328dc6ca7caaf0b1fa171ee5da524`  
		Last Modified: Wed, 06 Apr 2022 02:46:27 GMT  
		Size: 176.9 MB (176881303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ebb4de46699fdcb9e790b8f341ba30b43517f9400c0069e5370bef272ed15e`  
		Last Modified: Wed, 06 Apr 2022 02:45:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a483ad94148164aa510d036c77b03a84ba569051d186aa4ba08a96eb87e8bc`  
		Last Modified: Wed, 06 Apr 2022 02:46:46 GMT  
		Size: 50.9 MB (50933048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8167b9400eac12b6d079c9354c2ef03d78971eb3ce906be930155d2ab3df7f`  
		Last Modified: Wed, 06 Apr 2022 02:46:37 GMT  
		Size: 311.8 KB (311818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecd305fde6b65e548c4a324be9acc1d2cd34c65122bc85074064ff9b873ae78`  
		Last Modified: Wed, 06 Apr 2022 02:46:50 GMT  
		Size: 79.6 MB (79602253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849b843e679cb2878ba4ee40c2e0dd8f8ffaa32c59d7599b6d94bb3c2043cecc`  
		Last Modified: Wed, 06 Apr 2022 02:47:06 GMT  
		Size: 15.9 MB (15858819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:3c62929dca7daa8d5518def18b3dd61b62a5c318bb61fcff1d4374f214c5136b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302719411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37d2cd73d041ef1d6576c434d11adcf02424f1e4a5ee8537bdbf65812f68df09`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:26:01 GMT
ADD file:be35fd9a0ef4a49afbe583edf1750187cad18b1bde4e7bf0ab344464740b5749 in / 
# Wed, 06 Apr 2022 03:26:01 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:32:26 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:32:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:32:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 04:32:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 04:32:48 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 04:32:48 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 04:32:49 GMT
ENV ROS_DISTRO=noetic
# Wed, 06 Apr 2022 04:35:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:35:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 04:35:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 04:35:16 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:36:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:36:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 04:37:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:38:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de340d6c69b8bed917b969ad75b8fe4fe951502bc050b013dc9151c3632fb704`  
		Last Modified: Tue, 05 Apr 2022 13:15:39 GMT  
		Size: 24.1 MB (24073792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce0b0d26ad7a918b36da73b2eddac1e8f316863bbccd547c7ccadf4c7b5b8e3`  
		Last Modified: Wed, 06 Apr 2022 04:51:28 GMT  
		Size: 1.2 MB (1181524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a650205a9690aefea5eeec6ae78f99583040431f6fab18289857cc3d63c1ecc`  
		Last Modified: Wed, 06 Apr 2022 04:51:27 GMT  
		Size: 4.7 MB (4676054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af4193a1277485335b3de17430e9866176d6776e23f4a3e0408f9d843c4bbb6`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d32a40c6e63463e77533412a4d8ed9f74793778c730bec91a7f5a9d14688d42`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fdf1f4ad453b3a18dd87e720f5c322b674889bef7f10ea87e6856841a9ba5b`  
		Last Modified: Wed, 06 Apr 2022 04:53:35 GMT  
		Size: 157.4 MB (157429225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfbfdf74b4e2df8963d7509f98192a343047402ec0d91f9d448a656ec970061`  
		Last Modified: Wed, 06 Apr 2022 04:51:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddadecb4a27a3e0d593b52126b531eccca2f87e3620c832031450f532782c34`  
		Last Modified: Wed, 06 Apr 2022 04:54:09 GMT  
		Size: 40.5 MB (40500174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f7f0954acfa0e5e6880e529feb45596adf4c793185871dcbef7efb79fe8aaf`  
		Last Modified: Wed, 06 Apr 2022 04:53:47 GMT  
		Size: 311.8 KB (311831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1792acea348afad56c81f309974ab41d76528931ea68d24a5fde2c9beaee0c45`  
		Last Modified: Wed, 06 Apr 2022 04:54:27 GMT  
		Size: 60.5 MB (60481261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46ef657972035dd5e9deb5842553c1c3ce23fa5bd241836138526e9b6c0b84`  
		Last Modified: Wed, 06 Apr 2022 04:54:52 GMT  
		Size: 14.1 MB (14063137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:34450dc0963ff9e38b6cd9f2898af38c86ae8996f9b75e358914c3aec3964233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337480966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52c708c2aa11585c619f40fec799605a5f3d96810c046c32da285e5f2d8c7b3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:07:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:07:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:07:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 00:07:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 00:07:44 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 00:07:45 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 00:07:46 GMT
ENV ROS_DISTRO=noetic
# Wed, 06 Apr 2022 00:08:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:08:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 00:08:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:08:45 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:09:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:09:10 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 00:09:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:10:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a8b80bc3dfe754b09e8f3623fb3cd9e300bee4e2ee1ff5d754e921ff23e802`  
		Last Modified: Wed, 06 Apr 2022 00:24:48 GMT  
		Size: 1.2 MB (1181994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8cfeabbec8839214562f2254e216ef5cfc5a5809f29bc698db7732e32a1392`  
		Last Modified: Wed, 06 Apr 2022 00:24:46 GMT  
		Size: 5.3 MB (5321759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da8823fdc5cee0d100dd6dde003a5eb0bcddf554b44d339dfaf898b1cce78d`  
		Last Modified: Wed, 06 Apr 2022 00:24:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e6c0035719ce261304cc492c75a959ba0c2adeeda30ca62ce151e812dc240f`  
		Last Modified: Wed, 06 Apr 2022 00:24:45 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d4a7852cc1f492ea8c3f2182441e01972de69e8cb431d5efcf134cd1129b22`  
		Last Modified: Wed, 06 Apr 2022 00:25:14 GMT  
		Size: 171.3 MB (171305318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdd8de1f045e21c6093f43ce6904e2749f5a726e47d5b22f8821bb5f7c3d349`  
		Last Modified: Wed, 06 Apr 2022 00:24:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01813c1914905e5b21831e0911f7d32f9a63232dac855e79fdf58960457a02`  
		Last Modified: Wed, 06 Apr 2022 00:25:33 GMT  
		Size: 45.0 MB (44988186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64b58c4553378a5f9376929fc6946b8958f03bd743251a050e65f486ca9359b`  
		Last Modified: Wed, 06 Apr 2022 00:25:26 GMT  
		Size: 311.8 KB (311760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9beb87651ab3416a3f7b7ae4a8233fafc4b182728420bd3ea4db3addb33300d`  
		Last Modified: Wed, 06 Apr 2022 00:25:37 GMT  
		Size: 71.8 MB (71753434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc52af72271ca59e6415f2d32f5d26f3adba4f956ccaf7c378c3fd171ff327a2`  
		Last Modified: Wed, 06 Apr 2022 00:25:56 GMT  
		Size: 15.4 MB (15446753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
