## `ros:noetic-perception`

```console
$ docker pull ros@sha256:efc4c1e40d16fafbdf5ee1a68a468855b602a89148bd8320419a6d4f0850993f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:75b9e694d8bf831ceeeb7f839faef39718b756fe7fd6b147389b423e81e4deff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834975524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6f96daae1d6f221b7a1e3c317e0e1857ae4406c0cd798c7caea98c423afbcf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:11:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 01:11:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 01:11:03 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 01:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 01:13:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:13:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 01:15:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 01:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44b59555aadd115e37e45f079fef0ca694c5888fcd16350e10a693138a6db4`  
		Last Modified: Tue, 07 Jun 2022 01:47:19 GMT  
		Size: 5.5 MB (5547097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cefae97638ee7cb88a42485677466aa5587fca9972953eaaea67058f3e6d72b`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86209410ac0375ac01df476d1f843d17c9837f6c086953deeaf0c7941bb3c47e`  
		Last Modified: Tue, 07 Jun 2022 01:47:17 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf3bc6872ece682381026a6f6f11c4d5545ea0332db254fd844cd04ba7ea30`  
		Last Modified: Tue, 07 Jun 2022 01:47:47 GMT  
		Size: 176.9 MB (176860236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d317e6d1d9fe1bfd2c0445d594e8536c4d7e97846da20d59866f3c735294eb`  
		Last Modified: Tue, 07 Jun 2022 01:47:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617909da5816fdd6725712597eee7c8f07b716d1adbd74100e4c2c6d8695e764`  
		Last Modified: Tue, 07 Jun 2022 01:48:05 GMT  
		Size: 50.9 MB (50934172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d95b4adafcf47d6a3bcba767615da47a945bbee4229e97017601a6aae6487`  
		Last Modified: Tue, 07 Jun 2022 01:47:57 GMT  
		Size: 319.3 KB (319342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65210ff74d033bbbd26bd59530f4a4f3a6ef5932282476aa41b7ec7342ddc592`  
		Last Modified: Tue, 07 Jun 2022 01:48:09 GMT  
		Size: 79.6 MB (79603101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b507c79d7107ec363c6307707669011365415eaf3e2b57e092345795a891073`  
		Last Modified: Tue, 07 Jun 2022 01:49:48 GMT  
		Size: 492.0 MB (491955351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:76c31d214cc137ea927ff2063fb650677b35f9425a2bb33a6403f9ea212cac21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.1 MB (726099628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1981d18f271e92ae9f73bd01a9b570ca52867b8c82762839e22e3941de6b65`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:22:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 10:22:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 10:22:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:23:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:23:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 10:24:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:30:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35ba9bb076ac5c2202b84cf791ad024ed567d567515ea810f06952938c7e7d`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29bf79e77081f6707280737117556ce402c4f3adc2715aebbc655cfc523094`  
		Last Modified: Tue, 07 Jun 2022 10:41:40 GMT  
		Size: 40.5 MB (40500574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da5bd7c69f54a4f26f342e791874bacc258c931f68a08e170de5371450e010c`  
		Last Modified: Tue, 07 Jun 2022 10:41:18 GMT  
		Size: 319.4 KB (319361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c69679c4c18509848bd2b01c85345c5176fe8db6e7214f4c68b1ccfe9ed415`  
		Last Modified: Tue, 07 Jun 2022 10:41:57 GMT  
		Size: 60.5 MB (60481674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af91be591a3f9fbb984d9d660d7663ce56bf63f386cb93d3a117bc2f204becd`  
		Last Modified: Tue, 07 Jun 2022 10:47:07 GMT  
		Size: 436.9 MB (436928957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:abdaf92af631a706682332fa8444b201e5826269a643b8f0c793ae9b3f0271b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.6 MB (784601209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a32e701f93d54e204881bde26d8a04052227b742fa4f4bfcf14734f215f8d81`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:17 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 07 Jun 2022 05:54:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jun 2022 05:54:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:54:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:54:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jun 2022 05:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:57:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a0b8a290ad7faa448334c682b81ada169f7014ab73db216501105537e3f2ae`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fddd19b2dd196832c93dcc720dbc68cbe84ad6617329dbacb64940c6335519f`  
		Last Modified: Tue, 07 Jun 2022 06:18:46 GMT  
		Size: 45.0 MB (44989246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c51c8606ccfddadf8d24ef39d6da319acb3c475c4708ef58fed6312b0020d`  
		Last Modified: Tue, 07 Jun 2022 06:18:39 GMT  
		Size: 319.3 KB (319298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c26f1e72b4890b70a8091ac90548e1010153bfec6b8a6af616fc192d6e0e5`  
		Last Modified: Tue, 07 Jun 2022 06:18:49 GMT  
		Size: 71.8 MB (71754197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0301bf829c4c9a911ce71974625824a518faa4957e75948073a0788f5ce1e`  
		Last Modified: Tue, 07 Jun 2022 06:20:26 GMT  
		Size: 462.5 MB (462490945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
