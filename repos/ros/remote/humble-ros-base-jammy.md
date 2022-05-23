## `ros:humble-ros-base-jammy`

```console
$ docker pull ros@sha256:9f6e02c28c62b0f7370dd6952b1519094bb0151f6d6b04a132cdd8e063385712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:humble-ros-base-jammy` - linux; amd64

```console
$ docker pull ros@sha256:a170eaed292d7817363063540d4b955c98c284a8e3e6e3a32ce95ada819f1367
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.4 MB (265383023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:437432e56e5a1f38296d855045e1c3521f0b5a0b9939b243e8e7a13a34f3e41b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:16:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:52 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 02:16:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:16:53 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:16:53 GMT
ENV LC_ALL=C.UTF-8
# Mon, 23 May 2022 22:21:56 GMT
ENV ROS_DISTRO=humble
# Mon, 23 May 2022 22:23:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 22:23:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 23 May 2022 22:23:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 23 May 2022 22:23:31 GMT
CMD ["bash"]
# Mon, 23 May 2022 22:24:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 22:24:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 23 May 2022 22:24:27 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 23 May 2022 22:25:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5d137ac3f4107166acc832d7edffb774a28a3a16ca4f1fbe1b4f3653c8824d`  
		Last Modified: Sat, 30 Apr 2022 02:29:07 GMT  
		Size: 1.2 MB (1191214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f742e0a4361e52c84f1a27d4d57685a19b201687e97de11e8308e3919dc6`  
		Last Modified: Sat, 30 Apr 2022 02:29:05 GMT  
		Size: 3.8 MB (3826919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de85e82a503b9baeed214acd1421f6eac09e02419926d5eb1ae3fd6863bb7a5c`  
		Last Modified: Sat, 30 Apr 2022 02:29:04 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d5c725f3312c7dd56c39d5af65304e67e94a82e1af69a06d8394c0d4f16be1`  
		Last Modified: Sat, 30 Apr 2022 02:29:04 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ef630c76ed5b8da3cb01430dba5969680629b1f593df525e86e145b06b0946`  
		Last Modified: Mon, 23 May 2022 22:26:46 GMT  
		Size: 108.8 MB (108822234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315c38decded689481324fcd62f00041ed92bceb828298069fb5e395f4ef213a`  
		Last Modified: Mon, 23 May 2022 22:26:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8717e17d205c049a63ced147317faf44ef639cb2658ce555c7ff11614fc28689`  
		Last Modified: Mon, 23 May 2022 22:27:10 GMT  
		Size: 97.8 MB (97838323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdb2f666c5cc91dfdfac9d571b2045ceaad03ab34dd0bb61e9ebd05ff633640`  
		Last Modified: Mon, 23 May 2022 22:26:57 GMT  
		Size: 271.1 KB (271124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeae00ba938a2d6851f34058218cf5771e7b95870475644054fe489a07e6b66`  
		Last Modified: Mon, 23 May 2022 22:26:56 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67361ce25c8eb2f1f6f12b32e28d5a9fa2225dc416199bd6b030ef88be30ec3c`  
		Last Modified: Mon, 23 May 2022 22:27:00 GMT  
		Size: 23.0 MB (23007504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:humble-ros-base-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:dd53e9e2406ccf7d756ffb8cf2ceeaa6dcf07913d02998b8cb7403253db4f282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257481706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5870b8c68ed6ef3977a99e806781cd2794f727b434122942bcf81257410cf214`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:32:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:32:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:32:29 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:32:30 GMT
ENV LC_ALL=C.UTF-8
# Mon, 23 May 2022 22:43:54 GMT
ENV ROS_DISTRO=humble
# Mon, 23 May 2022 22:44:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 22:44:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 23 May 2022 22:44:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 23 May 2022 22:44:59 GMT
CMD ["bash"]
# Mon, 23 May 2022 22:45:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 22:45:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 23 May 2022 22:45:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 23 May 2022 22:46:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-humble-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4339dcf07e4fd919aa10dc0e01fb8f44184f74bf6baf5aef6e8fdd30f5e603`  
		Last Modified: Sat, 30 Apr 2022 00:43:58 GMT  
		Size: 1.2 MB (1192681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0db3fdf5b04e561797500fc1d19d79a37ca0586b71bee71ce2acaee153d4dee`  
		Last Modified: Sat, 30 Apr 2022 00:43:56 GMT  
		Size: 3.6 MB (3594435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af71d8cd404a31e077722270696cf33d59cff54d35c9dad864264138bc3ac`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e01b1250d40bc108a995e5fc6c1630b0abdbfff31529a87a4096271f2a6115`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5686ce861dda605e75ee4a6bab3e53f097e4010fef23f34179217491d430d824`  
		Last Modified: Mon, 23 May 2022 22:48:33 GMT  
		Size: 106.4 MB (106393737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8fffc177af7b7119460aff11709207884cdfd1b72a774646124001a5718646`  
		Last Modified: Mon, 23 May 2022 22:48:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936b0dfdb1762464e987b98fc9d974453ac3415bbfa8d9496752d012dba3294f`  
		Last Modified: Mon, 23 May 2022 22:48:59 GMT  
		Size: 95.2 MB (95223771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a449faeb594cb721b14a7fdb85cbeb8785586887a31b23fa6789b7606800ca7f`  
		Last Modified: Mon, 23 May 2022 22:48:45 GMT  
		Size: 271.1 KB (271074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2665d21fe01d8b1054c89ad2166988f46fadfa08fff394859103f47f7d2687`  
		Last Modified: Mon, 23 May 2022 22:48:45 GMT  
		Size: 2.2 KB (2178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73198756089c073e8dc6861da51d15bf7a80f3ef1ec0d9ea5bded64f40c08154`  
		Last Modified: Mon, 23 May 2022 22:48:49 GMT  
		Size: 22.4 MB (22425004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
