## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:71c16199c51734a2b7842be35e9ddd59e7d09bfdae92195ddf938cae35bcac44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:5130a1dba08e18d87eaa1ed26348581a84c4746636264da4418dcb88733bfedf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.1 MB (411112875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1ade2b17d6835cdb19eff9bc8cdd2fdccbddc7f622af04c6ab130308425864`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:22:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:22:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 18:42:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Jul 2020 18:42:17 GMT
ENV LANG=C.UTF-8
# Fri, 24 Jul 2020 18:42:17 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Jul 2020 18:45:33 GMT
ENV ROS_DISTRO=rolling
# Fri, 24 Jul 2020 18:46:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:46:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Jul 2020 18:46:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 18:46:27 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 18:47:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:47:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 18:47:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Jul 2020 18:47:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:47:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 18:47:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 18:47:26 GMT
ENV ROS1_DISTRO=noetic
# Fri, 24 Jul 2020 18:47:26 GMT
ENV ROS2_DISTRO=rolling
# Wed, 05 Aug 2020 07:01:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.8-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:01:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.9.2-2*     ros-rolling-demo-nodes-cpp=0.10.0-1*     ros-rolling-demo-nodes-py=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:01:42 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e64ae169025b3bf66b3257b0c3ce2879f1ffa845758c933f8dcca5f89cc19b`  
		Last Modified: Fri, 24 Jul 2020 18:54:30 GMT  
		Size: 5.5 MB (5546860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da420c8f951b321ba6103a944759f9556f244c2594e836b48f09847ba7b5cfe8`  
		Last Modified: Fri, 24 Jul 2020 18:54:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a60927d7c8eae45da5d75487f74ef9ff49f8b21bf6b860f56ddb16fe7f04b20`  
		Last Modified: Fri, 24 Jul 2020 19:00:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5560b73fea02644b4372410ed591eeb71aaf62449915e2b76f78f1635482ce`  
		Last Modified: Fri, 24 Jul 2020 19:02:13 GMT  
		Size: 119.3 MB (119269067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d8321b1b106afb233300e31ee9ef6a751d2ca63296004ac31c7f7a46afe523`  
		Last Modified: Fri, 24 Jul 2020 19:01:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f60995f19cb540187bf823c0a371c77bf56e7c54b859ecf8fe8a268141e286e`  
		Last Modified: Fri, 24 Jul 2020 19:02:31 GMT  
		Size: 66.6 MB (66579215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bfa5861c763b46263a7824ddabe6a79dc7365128ae0b11bcf05226154b8339`  
		Last Modified: Fri, 24 Jul 2020 19:02:18 GMT  
		Size: 183.7 KB (183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acf79d5d6c96eb35b36284eafef986ae57ffcca441d9ac867469289dcc712ef`  
		Last Modified: Fri, 24 Jul 2020 19:02:18 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06df6ba0a242fe5b5d6cbcb60b0494be8e5dbe9868b4d112cb6957b91bf0488`  
		Last Modified: Fri, 24 Jul 2020 19:02:21 GMT  
		Size: 10.3 MB (10283022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e70e7ace398c1e899a864874cfa31a7cbd05c45bddc599be1c2408e46ec47`  
		Last Modified: Fri, 24 Jul 2020 19:02:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb647ed890b7247e98037ede088e2f91b21b734a7e192a54389f92925bb168b`  
		Last Modified: Fri, 24 Jul 2020 19:02:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ff320285de65dd22f74a4745262be9f7bd1f2b5dfe786448e3a8da4f27459c`  
		Last Modified: Wed, 05 Aug 2020 07:09:22 GMT  
		Size: 76.1 MB (76095325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faddecc27bcf5f73e829fd2427011d61ba851a4d80929f5b091dbc0ba0ab6bac`  
		Last Modified: Wed, 05 Aug 2020 07:09:20 GMT  
		Size: 103.4 MB (103384070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0524080bc79a8346eaf47cc9995da79081e85202b881951ee7117ecf12b1782`  
		Last Modified: Wed, 05 Aug 2020 07:08:57 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1cf5e7cddc77a8e53d6eb3d77c8b4f892817dba8057495d2140eeab4d87b6cc1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.7 MB (376650010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21991753e1e53d9792bb891bbe3ed7b3386987045815cf7ca3f6281a603ef628`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:24:06 GMT
ADD file:26bd57f1dbcfd1a91715cc84cf0f221783655f16bbb7a912aaf20507cc252535 in / 
# Fri, 24 Jul 2020 16:24:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:24:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:24:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:24:44 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:57:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:57:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:57:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 17:24:07 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 24 Jul 2020 17:24:08 GMT
ENV LANG=C.UTF-8
# Fri, 24 Jul 2020 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Fri, 24 Jul 2020 17:30:58 GMT
ENV ROS_DISTRO=rolling
# Fri, 24 Jul 2020 17:32:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:32:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Jul 2020 17:32:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 17:32:57 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 17:33:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:34:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 17:34:13 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Jul 2020 17:34:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.1-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:34:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 17:34:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 17:34:55 GMT
ENV ROS1_DISTRO=noetic
# Fri, 24 Jul 2020 17:34:56 GMT
ENV ROS2_DISTRO=rolling
# Fri, 24 Jul 2020 17:35:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.7-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:37:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.9.2-2*     ros-rolling-demo-nodes-cpp=0.10.0-1*     ros-rolling-demo-nodes-py=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:37:20 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:3583fd5e2faf2976fb6333a3a15414f2708dc284c018a672e37112326bc7b7a1`  
		Last Modified: Mon, 20 Jul 2020 15:50:10 GMT  
		Size: 27.2 MB (27159444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d9e0aed378588f59f8f4276e70ea379b773d7d6507046cd7a044601499785`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 32.3 KB (32333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a6dca9e536449681a937b8f49022cb56b230e352da8aed9b616fadb14dc30`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d9e98650a6106452fc9e640abe8929399fa4f7a0d3ef58a593e8d68cdf3a6`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b877914f23fdc8a3fd15f9b3daa4a5a017f378e476b524967a0ab3874b518fe5`  
		Last Modified: Fri, 24 Jul 2020 17:48:49 GMT  
		Size: 1.2 MB (1175990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd422d18fc87ff73ecb113f2cf765e9b4e16079bb0f4c697b78fc61dfbbbb2f`  
		Last Modified: Fri, 24 Jul 2020 17:48:49 GMT  
		Size: 5.5 MB (5511790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281dec9f244ed77fbf977c9357ced59b8843bba14d99bbbaf00a19cb797f655a`  
		Last Modified: Fri, 24 Jul 2020 17:48:43 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8222dc272a4ea67fceee9f2cd1d6fa321f28a2ca48e4187dbef9fc609c03fde7`  
		Last Modified: Fri, 24 Jul 2020 18:02:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e42434d879d59a987c2c6aae212c34d2c3581854d0bcf3dcd95bb5c77ccc38a`  
		Last Modified: Fri, 24 Jul 2020 18:06:37 GMT  
		Size: 103.5 MB (103496824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d66d3005f38065aca76a79dd178e370c20bb4c958bc23a5085471b0a7d8fc13`  
		Last Modified: Fri, 24 Jul 2020 18:05:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbe4ce6b34429b9cf3c595068b425eb279fa003b6ffcd755af09b4de39a38f6`  
		Last Modified: Fri, 24 Jul 2020 18:07:28 GMT  
		Size: 60.9 MB (60932117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ff26300fad41529f36f1b1bdb0e6bce4af3b005161d294e875982b855466c7`  
		Last Modified: Fri, 24 Jul 2020 18:06:48 GMT  
		Size: 183.8 KB (183788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4497e482a6bcda17c5af840af74f4f4439f74d4eefb6dd7a378ef2313c0e3b82`  
		Last Modified: Fri, 24 Jul 2020 18:06:48 GMT  
		Size: 2.0 KB (2025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9831e9e3f59f3ec1ff626d44ed6a5f7463529aa8839125c2c10190441ea9d347`  
		Last Modified: Fri, 24 Jul 2020 18:06:55 GMT  
		Size: 9.3 MB (9302620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4dbcd98641e93dc690dc032eb1f907ed22c3f81e13b27dd50443cc37b977a8`  
		Last Modified: Fri, 24 Jul 2020 18:07:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adce0bb834206f67e28ffdbb6d2b18cc261d86186910184bb295f0190ea2ca8c`  
		Last Modified: Fri, 24 Jul 2020 18:07:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959f552e40d9ec5f430a3dc25c09cbfb98835f8ac2b08bb409542c0f8e17a75a`  
		Last Modified: Fri, 24 Jul 2020 18:08:53 GMT  
		Size: 76.1 MB (76107416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2fa40db443c5f00a90c62635ed4493ce82b3fbe3da915e27ca3ab9a6008533`  
		Last Modified: Fri, 24 Jul 2020 18:08:44 GMT  
		Size: 92.7 MB (92742164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16284451912c59e9269b67e40952c8f05fb08f3a37990a3b59dfd2b5655d1514`  
		Last Modified: Fri, 24 Jul 2020 18:07:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
