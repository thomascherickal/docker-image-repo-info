## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:b2eaa30a8e8d9df217217fdb74c5e9796587246239d406fe97c63c414d3603c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:eaff9aab6096206d5602d1a8eae36d1534b53299c172e347c251bf51dba63877
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.2 MB (340187876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf92241175ae4197bb4cbcb99b62d8e89327e97e85e1e85d9b3b12d4e249e9f6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:39 GMT
ADD file:c77338d21e6d1587df92d76a2b0a5c36f0e026ac1640b5cddefb1bf8db8a1204 in / 
# Thu, 04 Mar 2021 02:24:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:42 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 10:03:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:11:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:11:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:48:31 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 12 Mar 2021 14:48:31 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 14:48:31 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 14:55:02 GMT
ENV ROS_DISTRO=rolling
# Fri, 12 Mar 2021 14:55:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:55:49 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 12 Mar 2021 14:55:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 14:55:49 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 14:56:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:56:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 14:56:21 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 12 Mar 2021 14:56:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:56:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:56:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 12 Mar 2021 14:56:46 GMT
ENV ROS1_DISTRO=noetic
# Fri, 12 Mar 2021 14:56:46 GMT
ENV ROS2_DISTRO=rolling
# Fri, 12 Mar 2021 14:57:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:57:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.12.0-1*     ros-rolling-demo-nodes-py=0.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:57:23 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:5d3b2c2d21bba59850dac063bcbb574fddcb6aefb444ffcc63843355d878d54f`  
		Last Modified: Mon, 22 Feb 2021 16:09:51 GMT  
		Size: 28.6 MB (28567785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2062ea6672189447be7510fb7d5bc2ef2fda234a04b457d9dda4bba5cc635`  
		Last Modified: Thu, 04 Mar 2021 02:25:50 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf526d75b82eb4f9981cce0b23608ebe6ab85c3e1ab2441f29b302d2f9aa8`  
		Last Modified: Thu, 04 Mar 2021 02:25:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07cfec6f2da960164171c5970a0a257d0cedb5f791a43019ec06be3f6be3842`  
		Last Modified: Fri, 12 Mar 2021 10:28:38 GMT  
		Size: 1.2 MB (1182808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694590d03abf5d1734a02addbf98c8bae4b3ad1ebdf9523ec5687888462f1360`  
		Last Modified: Fri, 12 Mar 2021 15:09:45 GMT  
		Size: 5.5 MB (5547975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b6051fbcd3c71d56397c8f01cf7b807b358b76dfbd34be6f585e364b69645f`  
		Last Modified: Fri, 12 Mar 2021 15:09:43 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837d766562deb82c9084eba6327232cd4556395a71f01dd9b332f90c6227c866`  
		Last Modified: Fri, 12 Mar 2021 15:21:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a790f8d7684346bc385b9378ce86cb3979c992e8b6a7e7dd6060d3abf98ff1b0`  
		Last Modified: Fri, 12 Mar 2021 15:23:54 GMT  
		Size: 117.2 MB (117234300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f578d362792fdd74863fb2f7be5d58719d53111c45be96d1b2e95901dc202a`  
		Last Modified: Fri, 12 Mar 2021 15:23:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba2ad7f22dcf1e2999ceafc9a6643a08deec89d16f6f22c1224be148b1f5e35`  
		Last Modified: Fri, 12 Mar 2021 15:24:20 GMT  
		Size: 66.6 MB (66560511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5f364acc6bb45b4711743e65e99122a25329cf2139f42366ecf5e8f7bcec2a`  
		Last Modified: Fri, 12 Mar 2021 15:24:08 GMT  
		Size: 209.5 KB (209506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389284900d0e6d55ea35d9961f8da59e9ce25b6efffc4b08e11cf9b2a36efa10`  
		Last Modified: Fri, 12 Mar 2021 15:24:07 GMT  
		Size: 2.0 KB (2021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361586f05dd00241f0e9a6fcd7da37081a85c20914220c173e9651e407810ed2`  
		Last Modified: Fri, 12 Mar 2021 15:24:14 GMT  
		Size: 29.5 MB (29486671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345af4dab3c8fa3d9177371be070a3e9ae66ec0228f881852446d045c601abe3`  
		Last Modified: Fri, 12 Mar 2021 15:24:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1b0d53489ed69e4e1194663a56fc7e7a4cbf77fdfe0933da6577a9544816c3`  
		Last Modified: Fri, 12 Mar 2021 15:24:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993c91df597ef220eaad5deac239aac57916757ab241a6c89e9bc2b6da23da26`  
		Last Modified: Fri, 12 Mar 2021 15:24:56 GMT  
		Size: 76.1 MB (76145811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f7f3a9b3a4ebb47f9460cb449ad4c000b5e0ec76d3fe6829d49511f4d0dc4e`  
		Last Modified: Fri, 12 Mar 2021 15:24:39 GMT  
		Size: 15.2 MB (15247017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69023392d756a84c0c3ffe09f678f9585395dc1704ecfae117e01d8da18570e8`  
		Last Modified: Fri, 12 Mar 2021 15:24:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0e67285c443e71a29a3eafe8473d73bec43e50ba4189e420c79327a19351e73b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.9 MB (312882575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7c699dee829d0028a3e3a74893e2fb6a8f595b1cd939fcb4034a073f8a827d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:52 GMT
ADD file:1dfda258a4ebfa53687877ae153107d2e472e0b039363ec35aafe9f5733cae22 in / 
# Thu, 04 Mar 2021 02:52:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:53:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:53:01 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:22:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:22:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:22:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 03:47:10 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 04 Mar 2021 03:47:12 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 03:47:13 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 03:53:21 GMT
ENV ROS_DISTRO=rolling
# Thu, 04 Mar 2021 03:55:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:55:18 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 04 Mar 2021 03:55:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 03:55:20 GMT
CMD ["bash"]
# Thu, 04 Mar 2021 03:56:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:56:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 04 Mar 2021 03:56:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 04 Mar 2021 03:57:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:57:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 03:57:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 04 Mar 2021 03:57:48 GMT
ENV ROS1_DISTRO=noetic
# Thu, 04 Mar 2021 03:57:49 GMT
ENV ROS2_DISTRO=rolling
# Thu, 04 Mar 2021 03:58:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:59:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.12.0-1*     ros-rolling-demo-nodes-py=0.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:59:12 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:32d7611b468cbc07986302f1a8e74d92e30a1f11cdfa8bc2900aedda2758d050`  
		Last Modified: Wed, 17 Feb 2021 08:25:24 GMT  
		Size: 27.2 MB (27175799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be16fdc30614524222cdec466297e7ed49c7695e868c5dd2700a1778d88b23`  
		Last Modified: Thu, 04 Mar 2021 02:54:33 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a361e87bde5e27ceda037ab2116d88d9570b6d53c34102a2a214ef2944270138`  
		Last Modified: Thu, 04 Mar 2021 02:54:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1317e878738b2e361ab2bc6c5e9dad3effcdd7f83f6a2e3687fc82bc9c1ada3`  
		Last Modified: Thu, 04 Mar 2021 04:04:00 GMT  
		Size: 1.2 MB (1182875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba5f746c529c10d1d08e23f12a45a07e2921c194edd5618c4b72f862233e909`  
		Last Modified: Thu, 04 Mar 2021 04:03:59 GMT  
		Size: 5.5 MB (5512834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea8b4c459768d7eb6fc2a16d12531aface693a3d22b366e35336593ee89d6ad`  
		Last Modified: Thu, 04 Mar 2021 04:03:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d21be1269617b9a86a32152d26029110477c2c276439a32dadbb93c5fa52754`  
		Last Modified: Thu, 04 Mar 2021 04:11:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64c9cc31cd48021d0277aee50bd43d42b6ae4269b7b8048a87b35884d413a7e`  
		Last Modified: Thu, 04 Mar 2021 04:13:52 GMT  
		Size: 101.6 MB (101581989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924120b85fbf4bcc245236b2272b0470c9b3feb1b536914f3f5a0504f80b4a64`  
		Last Modified: Thu, 04 Mar 2021 04:13:22 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91438bf90a4a53a8babb799dd4baaa1d122a5dc011fa7cccf32732e2a1e65d3`  
		Last Modified: Thu, 04 Mar 2021 04:14:15 GMT  
		Size: 60.9 MB (60915958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ceeabd40eddd1d6fee8970b8b0d21fb55481663f4115a40cd62d94aa7dc1334`  
		Last Modified: Thu, 04 Mar 2021 04:14:00 GMT  
		Size: 209.1 KB (209068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432729f3fbb5c2e446142ba81942a0d65045c5cc11ed062a9302a3f283f4b729`  
		Last Modified: Thu, 04 Mar 2021 04:14:00 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67e5e2b03d993a6698a4f5b6025a92b83c3e28a1ebe37c3048580b8617335e5`  
		Last Modified: Thu, 04 Mar 2021 04:14:08 GMT  
		Size: 27.6 MB (27558960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f422b8505527f78616f25c9ad6b4e384a59553cccc7be2219b13b0a538e2fbbc`  
		Last Modified: Thu, 04 Mar 2021 04:14:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97eba661a3cbc95ecfe93d210e7dca12e997792cef688b4ea7e76e5100496a`  
		Last Modified: Thu, 04 Mar 2021 04:14:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba6c4d7c0e0d0c312366590f4fa87ff245b95f42969bd646eb15f54f7280ee`  
		Last Modified: Thu, 04 Mar 2021 04:14:51 GMT  
		Size: 76.2 MB (76184068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b790f10c894dcf2b364700c64c0e13321676235cfc60ad0a988234294bc2d357`  
		Last Modified: Thu, 04 Mar 2021 04:14:28 GMT  
		Size: 12.6 MB (12555458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a905b131bf2a0421172ff500666f9b217a1841d1044e19becae5d132d7fadf42`  
		Last Modified: Thu, 04 Mar 2021 04:14:24 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
