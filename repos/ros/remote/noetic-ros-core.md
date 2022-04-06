## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:38c74fe965f0b107dc189a35137f8aa2a2a8c62cbc81653fc61326d085fdb2bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:da7ec50a3e68b60e33b15fef09e0f92a3a83018ce2553189783281803911e9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212177406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64673c72ed30579022e8e79e5eeb91ba1007ab1273a2964148042de96998d817`
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

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:ada7d17bfb1f6ee1ac243fdd0d26aafa15caf90b0bb406199537417e265f857b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187363008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ed9e1075cc4eea11b0715f2b9c038e134229cbb848608f38f8fc3a1d94ba19`
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

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1913eaa0a667b95bee6071f9e40e86f334cc1b79f8f84339e4bd4e42e8b60b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (204980833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7b6e15a51366f44582049f2c49a89cd65ab15e4f252c9c01d8f418a5b9abe1`
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
