## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:f7b5843a230a2227f5e136838550fe272fa2ef262f19bfda8387748d0431471c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:3842d83316cef50508d18f237113ebacb4b5a797a3231c5fa7a2d1c283e4c21a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.0 MB (340970821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c471d974d4f6486b3fa9835db6eec9e97cd716d0e8821b85a2de361b45c24875`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:08:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:20:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:20:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 02:33:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 03 Apr 2021 02:33:42 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 02:33:42 GMT
ENV LC_ALL=C.UTF-8
# Sat, 03 Apr 2021 02:33:42 GMT
ENV ROS_DISTRO=foxy
# Sat, 03 Apr 2021 02:34:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:34:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 03 Apr 2021 02:34:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 03 Apr 2021 02:34:40 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 02:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:35:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 03 Apr 2021 02:35:29 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 03 Apr 2021 02:35:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 02:35:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 03 Apr 2021 02:35:46 GMT
ENV ROS1_DISTRO=noetic
# Sat, 03 Apr 2021 02:35:46 GMT
ENV ROS2_DISTRO=foxy
# Sat, 03 Apr 2021 02:36:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:36:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:36:28 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c5d2d7a6606006c3c9ad68491e77516419c59fceb2f4c04ca5580c96d8501`  
		Last Modified: Sat, 03 Apr 2021 02:40:16 GMT  
		Size: 1.2 MB (1182070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccd2266e6deaba5ba5682d19318df74543102cf36e0b3e2be8240cbd58404eb`  
		Last Modified: Sat, 03 Apr 2021 02:40:15 GMT  
		Size: 5.5 MB (5547325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2974076651535b81ed47daec0c9ac8a8a614de3b86c54d48a04c89ad19e07559`  
		Last Modified: Sat, 03 Apr 2021 02:40:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcd05d1e076faa0694af18a98a932e308a61016ec9d22d17a4a5d09ee624c5b`  
		Last Modified: Sat, 03 Apr 2021 02:43:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ccc6319ab7559a5964a05ea51d8169ed0bba9278525aceba25c3cd5c94a23`  
		Last Modified: Sat, 03 Apr 2021 02:43:53 GMT  
		Size: 119.9 MB (119907745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64b3515b1ac8e33202ea4cbb40699a3bca4bae71b70e6cc00f6b6bed6335464`  
		Last Modified: Sat, 03 Apr 2021 02:43:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82508de426fea3fba48e287cbd15132c6f4dd8d0d066829804c0da2137c65db1`  
		Last Modified: Sat, 03 Apr 2021 02:44:16 GMT  
		Size: 66.6 MB (66601760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21ba7e4fdc51c146abed1a8ca7036dbe6e8852f3d9a9e48f20f6af8866271e1`  
		Last Modified: Sat, 03 Apr 2021 02:44:05 GMT  
		Size: 216.2 KB (216218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844c2c9e77b1334d84a4e304b931290793b1a3d570f1aefdc0da55f5950ef7f`  
		Last Modified: Sat, 03 Apr 2021 02:44:04 GMT  
		Size: 2.0 KB (2031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6685ec9eb88c4700d1e65a3088d81a231e4c1f985214267f0225499199f1c7`  
		Last Modified: Sat, 03 Apr 2021 02:44:07 GMT  
		Size: 10.3 MB (10282338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908e013ca84daff1ada0db4edcbfdd2c105a11a62519a58d8a4f14062bf8f7f7`  
		Last Modified: Sat, 03 Apr 2021 02:44:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647dc7a48bf1062b8678b8fccc846cccd2ce1efbd57b2f1c1c6e51637157ed5`  
		Last Modified: Sat, 03 Apr 2021 02:44:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72e32303cf66eb7f9604da8a8b48976df43f5cc28a9e57cb95d9b5794e8ad98`  
		Last Modified: Sat, 03 Apr 2021 02:44:48 GMT  
		Size: 76.1 MB (76114120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a750323ba26ba66bd42a491af2cd27268d46910e37f7c7859d753ca4b7a50813`  
		Last Modified: Sat, 03 Apr 2021 02:44:39 GMT  
		Size: 32.5 MB (32544699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07186863895d1097a6a19f3e3d711a8812cf288b363da5341740dfc8b8601dc6`  
		Last Modified: Sat, 03 Apr 2021 02:44:33 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bcce10b3624ae2a389c3a01f1caace11d0aa74a58799009f58636182d5a8cb7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.6 MB (309613871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f1fba3e4b2a279d78ef5528ed7abb724b39c9d87b9207bda3cf5c886e686ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:25:49 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:26:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:26:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 06:35:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 03 Apr 2021 06:35:56 GMT
ENV LANG=C.UTF-8
# Sat, 03 Apr 2021 06:35:57 GMT
ENV LC_ALL=C.UTF-8
# Sat, 03 Apr 2021 06:35:58 GMT
ENV ROS_DISTRO=foxy
# Sat, 03 Apr 2021 06:37:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:37:42 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 03 Apr 2021 06:37:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 03 Apr 2021 06:37:43 GMT
CMD ["bash"]
# Sat, 03 Apr 2021 06:38:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:38:44 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 03 Apr 2021 06:38:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 03 Apr 2021 06:39:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:39:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 03 Apr 2021 06:39:21 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 03 Apr 2021 06:39:22 GMT
ENV ROS1_DISTRO=noetic
# Sat, 03 Apr 2021 06:39:23 GMT
ENV ROS2_DISTRO=foxy
# Sat, 03 Apr 2021 06:40:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:41:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:41:04 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b425e160ecdc1ce2e8f2c9394df0bf787e591ab7983fa386fa029ed26a92c1`  
		Last Modified: Sat, 03 Apr 2021 06:48:05 GMT  
		Size: 1.2 MB (1183308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19dbee98155e4cab1ca612d6d81cf3e8713fb2f87fc42d92530e2635fd1ba8f`  
		Last Modified: Sat, 03 Apr 2021 06:48:04 GMT  
		Size: 5.5 MB (5513345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874fc4821a261dd3d76266f77f06518b341b2bea50a79bd0dbc4fd367823c520`  
		Last Modified: Sat, 03 Apr 2021 06:48:03 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c452bc5faf1f1e451a20172334f340dd4489b450beb68b361113cbb662c759`  
		Last Modified: Sat, 03 Apr 2021 06:52:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a200d719b0970b08fb93f5a3c7cbd8b77b81a57f87c6f1ca19bc9edb64cd02`  
		Last Modified: Sat, 03 Apr 2021 06:52:40 GMT  
		Size: 104.1 MB (104086167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7619377c52dac48950e5f2593b3aa5b46543c19c5c0aa10e78d44ebf0da00e`  
		Last Modified: Sat, 03 Apr 2021 06:52:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c074bdbb1d113ccb6da4253451d71489c701b12fab9785e11f9a8c378e743`  
		Last Modified: Sat, 03 Apr 2021 06:53:03 GMT  
		Size: 61.0 MB (60970939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f198947f3ca651a40a6543e2a85d7ee5958d650e28dc8ee96a93f60d4e1a82`  
		Last Modified: Sat, 03 Apr 2021 06:52:47 GMT  
		Size: 216.2 KB (216225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fa149f281abf26c53845bf1255246678bde978647d64c6ff0ebd45f9d07a6f`  
		Last Modified: Sat, 03 Apr 2021 06:52:47 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d36dba38b21a843a911702cf0b5d4180818b22cf223b8082fafe132c8ae1bd6`  
		Last Modified: Sat, 03 Apr 2021 06:52:50 GMT  
		Size: 9.3 MB (9298794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc0772617f6fee76b5b284eec4e12ebe6a478fab4df504638a6358ff56fd45e`  
		Last Modified: Sat, 03 Apr 2021 06:53:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5738f00685c52e2da9c4974356f82e0718a9cb6b00476596c1af19c1958977eb`  
		Last Modified: Sat, 03 Apr 2021 06:53:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff0616f0cd59f3d3c33ea60e6eaa826eacff5ffd92c1d6e0a25d62f345de0f7`  
		Last Modified: Sat, 03 Apr 2021 06:53:39 GMT  
		Size: 76.2 MB (76157755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58b00a554c01604b8ffe1f0e5ffa64977756968823036c1a7593d2ce6298a30`  
		Last Modified: Sat, 03 Apr 2021 06:53:20 GMT  
		Size: 25.0 MB (25005003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665db0d8b910bb46618b7228dcb869fe4ffee24427d775d7b189be6cbf9c5c54`  
		Last Modified: Sat, 03 Apr 2021 06:53:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
