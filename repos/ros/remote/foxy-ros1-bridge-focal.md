## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:594f093740d228679bdbda1703273e6559c863a5e425e00db1ffd192d1da5036
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:7e5e975651a4c118a37aa779b40d0651597693d799d06c6f2d306b84a4f4b234
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.1 MB (411085948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a5634791a65867fee34df16a3ae4053052841a557d9d11d122d3aa2b1e1c81`
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
# Fri, 24 Jul 2020 18:42:18 GMT
ENV ROS_DISTRO=foxy
# Fri, 24 Jul 2020 18:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:43:15 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Jul 2020 18:43:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 18:43:15 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 18:43:49 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:43:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 18:43:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Jul 2020 18:44:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:44:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 18:44:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 18:44:18 GMT
ENV ROS1_DISTRO=noetic
# Fri, 24 Jul 2020 18:44:18 GMT
ENV ROS2_DISTRO=foxy
# Wed, 05 Aug 2020 06:58:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.8-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:00:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.3-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:00:18 GMT
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
	-	`sha256:dd57d7c9c134f1e633dbd1add0dda0ebb88b8daee088de9bc00326817b608f95`  
		Last Modified: Fri, 24 Jul 2020 19:00:51 GMT  
		Size: 119.3 MB (119279401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49d5e8315945b8e6e91bb2c89142020aca31d0abc13bfd415bedf35251a5453`  
		Last Modified: Fri, 24 Jul 2020 19:00:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12770edac5393e8ccfeaf57c22845b92f6d71a55244096a8f995bc43890846ea`  
		Last Modified: Fri, 24 Jul 2020 19:01:08 GMT  
		Size: 66.6 MB (66578298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9dc4de2ce0d29fc2308a99a4dd09a0f2ef9a414ab71c422b8658c197fa59d3`  
		Last Modified: Fri, 24 Jul 2020 19:00:56 GMT  
		Size: 187.6 KB (187623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac65a3414f8c6e44991fa66227a41022bb18a8432c1e56ac0dfc0e188a6be71c`  
		Last Modified: Fri, 24 Jul 2020 19:00:56 GMT  
		Size: 2.0 KB (2007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01186fe33283abd18dac56249fe2c93b35d6fe6b6e54320dda280c40954d0eb9`  
		Last Modified: Fri, 24 Jul 2020 19:00:59 GMT  
		Size: 10.3 MB (10278082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792d3c839a5d59e2486df450e1301c20a772b2dcfcf942456e579c7b72b5a9e0`  
		Last Modified: Fri, 24 Jul 2020 19:01:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bccdaff07366fb2ad7fb5a66d095bf368ad1c8aed32d43d8930e8a1c30b53d4`  
		Last Modified: Fri, 24 Jul 2020 19:01:14 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac68d51ffbaf566c5853759a62704a092ce7c937104684944c08c7f1521a70`  
		Last Modified: Wed, 05 Aug 2020 07:08:51 GMT  
		Size: 76.1 MB (76093149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd69210de618adae04945bc940eb5286df76ac322b1171fa0ce520b3ff06065a`  
		Last Modified: Wed, 05 Aug 2020 07:08:49 GMT  
		Size: 103.4 MB (103350950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533bea788db6e6c7b28fde97d4372de2198ae5c5d45c9553287d7b9645d837bd`  
		Last Modified: Wed, 05 Aug 2020 07:08:26 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cd33ddd55422a07964bb5bbd4b2307a59608797b162f73747fe732f9257947a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.6 MB (376616744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6af79a9879a9e8abe89fe303cdefc3d7f8dbc836b140f865667f2c950269e1da`
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
# Fri, 24 Jul 2020 17:24:09 GMT
ENV ROS_DISTRO=foxy
# Fri, 24 Jul 2020 17:26:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:26:07 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 24 Jul 2020 17:26:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 24 Jul 2020 17:26:09 GMT
CMD ["bash"]
# Fri, 24 Jul 2020 17:27:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:27:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 24 Jul 2020 17:27:18 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 24 Jul 2020 17:27:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:28:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 24 Jul 2020 17:28:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 24 Jul 2020 17:28:25 GMT
ENV ROS1_DISTRO=noetic
# Fri, 24 Jul 2020 17:28:26 GMT
ENV ROS2_DISTRO=foxy
# Fri, 24 Jul 2020 17:29:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.7-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:30:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.3-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:30:39 GMT
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
	-	`sha256:40e3496507d9f029e3aa2e3ffcc03d7cc1600cd97f7957aa13f2b5946ad7842b`  
		Last Modified: Fri, 24 Jul 2020 18:03:00 GMT  
		Size: 103.5 MB (103504523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5ca3a4b786f532b74525b2d8c1ed6fefa062346c063b7df076868cde415e45`  
		Last Modified: Fri, 24 Jul 2020 18:02:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c331fec9802b161fcd9c49ae5cafa6395667fed0f7ef6d08cae943caae4db4a`  
		Last Modified: Fri, 24 Jul 2020 18:03:28 GMT  
		Size: 60.9 MB (60931348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b4f04532eb4b9f90f1d465f2e0de9f4fc3c740171ceccd83b14d913a4e82e`  
		Last Modified: Fri, 24 Jul 2020 18:03:14 GMT  
		Size: 187.7 KB (187676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b0c67b65b84e3f8e7c6b0a151b9dc040afcbd3dde27af9b5f6307578beb352`  
		Last Modified: Fri, 24 Jul 2020 18:03:14 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd729f7f3676f667baf4d1b1d1d0df93a001657217e65107e6eb15b789fd6210`  
		Last Modified: Fri, 24 Jul 2020 18:03:19 GMT  
		Size: 9.3 MB (9295710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdac21f07493b8c2f396058fd51c8d0b30b299d5a0728433468372de513f4c9`  
		Last Modified: Fri, 24 Jul 2020 18:03:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3506687c5bf410472b6390eba1ab4e044157df9384b2296c6fab20cb5617d8f9`  
		Last Modified: Fri, 24 Jul 2020 18:03:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cdf4bbf37059d412a3f7af09bbb4380ae7521a433fe8157dee84a3568d4baa`  
		Last Modified: Fri, 24 Jul 2020 18:05:08 GMT  
		Size: 76.1 MB (76111551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47c928684532c35fb1bae88176df46c164bcf3c9e1c8d66db728ab0371f4409`  
		Last Modified: Fri, 24 Jul 2020 18:04:51 GMT  
		Size: 92.7 MB (92700865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdb2248c99c5aaf90af64357b6e5f289d6388cdb806a535a2dd4e6962a4e72f`  
		Last Modified: Fri, 24 Jul 2020 18:03:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
