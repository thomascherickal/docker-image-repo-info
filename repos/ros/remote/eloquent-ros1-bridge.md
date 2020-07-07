## `ros:eloquent-ros1-bridge`

```console
$ docker pull ros@sha256:9a7db828f1708dde51fd00bcf8153b385f6713549c352f117b3469ee1dc2e6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:268b2f765a91aaba02ace6bbd0c253ce2be9bad9a0ebf885405a489e67deb2a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.3 MB (429289556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8300485aae7cc3e609d050dc1814f85da8bd627fe66e3e9a36484a5249d70ed9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:42:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:38:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:38:27 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jul 2020 00:59:39 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 07 Jul 2020 00:59:40 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jul 2020 00:59:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jul 2020 01:05:15 GMT
ENV ROS_DISTRO=eloquent
# Tue, 07 Jul 2020 01:06:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:06:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jul 2020 01:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jul 2020 01:06:24 GMT
CMD ["bash"]
# Tue, 07 Jul 2020 01:06:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:07:01 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jul 2020 01:07:03 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jul 2020 01:07:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:07:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jul 2020 01:07:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jul 2020 01:07:20 GMT
ENV ROS1_DISTRO=melodic
# Tue, 07 Jul 2020 01:07:20 GMT
ENV ROS2_DISTRO=eloquent
# Tue, 07 Jul 2020 01:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:08:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:08:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:08:34 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5a9a0d3edafb836db5fec8836034836fd3958d7f30865871a5e6bd21ea4f82`  
		Last Modified: Mon, 06 Jul 2020 23:59:55 GMT  
		Size: 837.6 KB (837576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ed212db9ead4a977f8bd6d2d39e7cd9419e44b909a063b5b687984ab277ff1`  
		Last Modified: Tue, 07 Jul 2020 01:18:26 GMT  
		Size: 4.9 MB (4867686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce51d2b74c6394890393140880b5297053345b1aa65996976782844361e29440`  
		Last Modified: Tue, 07 Jul 2020 01:18:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0339248bdb6a34fc05061e67c76e3eb5fed59a1df09268e704e59bdfb57208`  
		Last Modified: Tue, 07 Jul 2020 01:24:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb59529b620d343ab4db4c2b9ea14982a44f252752cac557eff8cac50b2ed6eb`  
		Last Modified: Tue, 07 Jul 2020 01:26:23 GMT  
		Size: 188.3 MB (188322042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc1fd2ceee6ee1a93471417f23c3cb9048a6cb882f5ef37a6ac067b062b21c4`  
		Last Modified: Tue, 07 Jul 2020 01:25:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645d143de9a1361505c35456bcc98ce5e4dc0dc879806d8f77c142580ef80c77`  
		Last Modified: Tue, 07 Jul 2020 01:26:40 GMT  
		Size: 63.5 MB (63504848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e3a131385ebc66b1c4c96875188f16d6959a214f42e0b0e8b7f497942dd33`  
		Last Modified: Tue, 07 Jul 2020 01:26:29 GMT  
		Size: 182.9 KB (182853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a93dc6167c1a3a5304f68b12c971a6d825fc1360a07d68527e3a3be5642135`  
		Last Modified: Tue, 07 Jul 2020 01:26:29 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea18c4eeaf55e5574b7e247051497858df1c14aa49ebf13e505665f8d6a3c137`  
		Last Modified: Tue, 07 Jul 2020 01:26:30 GMT  
		Size: 4.6 MB (4580153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6432e9f57431ab905f0442fbab18a7311530321fc1132fc5e44dd98c9a93f5d`  
		Last Modified: Tue, 07 Jul 2020 01:26:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9e251e4c9c1df3df77f5398235f5fb4ec8661a16990982a368d37ce5c90aeb`  
		Last Modified: Tue, 07 Jul 2020 01:26:45 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbe2f9bd5afdfbc4f1c682b6283312f19a4ee08568bd5b4cf724d65ef6bf759`  
		Last Modified: Tue, 07 Jul 2020 01:27:13 GMT  
		Size: 117.7 MB (117669862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59f5c1609a1e1a2426456e4be8df5c2c0d4d59be6cb3332c1af6f33c247fe3`  
		Last Modified: Tue, 07 Jul 2020 01:26:52 GMT  
		Size: 21.9 MB (21941584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d64103e170dcd15e3c9f7b77d02c9ced5aefc1acfc41d25053906d7e940bc67`  
		Last Modified: Tue, 07 Jul 2020 01:26:45 GMT  
		Size: 646.0 KB (645957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7f7a1b4aa7699f9ae8d964bf4bdd2e4c022dc3e505e8a6bc1fe85ee7efa889`  
		Last Modified: Tue, 07 Jul 2020 01:26:45 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:cc77629c0b805b53e7b587c8c0916c1e5802e4e21b83d30e2a65d532d1e2a73e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.6 MB (363564422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6badbae51d10995974d80a965171add285ac495fe7a4c5ff49ed5df12d3a9d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:07:11 GMT
ADD file:6797f65071d6d263c6466e89bb2db63753b08510aef54a1dc28891fbf2e58799 in / 
# Mon, 06 Jul 2020 20:07:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:07:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:07:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:07:19 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 21:02:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:03:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:03:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 06 Jul 2020 21:14:10 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 06 Jul 2020 21:14:11 GMT
ENV LANG=C.UTF-8
# Mon, 06 Jul 2020 21:14:12 GMT
ENV LC_ALL=C.UTF-8
# Mon, 06 Jul 2020 21:21:09 GMT
ENV ROS_DISTRO=eloquent
# Mon, 06 Jul 2020 21:23:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:23:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 06 Jul 2020 21:23:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 06 Jul 2020 21:23:39 GMT
CMD ["bash"]
# Mon, 06 Jul 2020 21:24:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:24:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 06 Jul 2020 21:24:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 06 Jul 2020 21:25:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:25:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 06 Jul 2020 21:25:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 06 Jul 2020 21:25:37 GMT
ENV ROS1_DISTRO=melodic
# Mon, 06 Jul 2020 21:25:40 GMT
ENV ROS2_DISTRO=eloquent
# Mon, 06 Jul 2020 21:28:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:28:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:28:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:28:42 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:db182fa07ba527098363444f993730c582b86e361f0ac7ae981ba0e9ca768c84`  
		Last Modified: Mon, 06 Jul 2020 15:46:25 GMT  
		Size: 22.3 MB (22276511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e85650936bd5be5a40db91349e387ede7738f5f7938d6421cb9d64eb021a5a3`  
		Last Modified: Mon, 06 Jul 2020 20:10:21 GMT  
		Size: 35.5 KB (35457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258b890879c48b8d0f50ea632de0a703079d7f5d973ec47338cbe791bb8e30d5`  
		Last Modified: Mon, 06 Jul 2020 20:10:21 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f858a12ecedcf911e3fea9bb17332b53a888444834a3e3d12cd25be830898d`  
		Last Modified: Mon, 06 Jul 2020 20:10:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806d1a89313fbfafec371f2eb4ebfba3b3c83a5cc1ef0d02074f1b8c135030f`  
		Last Modified: Mon, 06 Jul 2020 21:32:39 GMT  
		Size: 838.2 KB (838170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cab5be046cf106505e6b283c44a303a38601c983c4098533cd616fa158cd229`  
		Last Modified: Mon, 06 Jul 2020 21:32:38 GMT  
		Size: 4.1 MB (4083445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d99c7934ee17c416ba33d8c0cd54fbc6b1f40e502b067899bc7875e684b7aa`  
		Last Modified: Mon, 06 Jul 2020 21:32:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbd95ab6f6469fe934cb703f95387119fcd6ddb2ac3e730acbb20ab735c22c8`  
		Last Modified: Mon, 06 Jul 2020 21:36:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3f52c4d3199c18900f031876c87b8687f3986274884ee72e15e23b57cf6de2`  
		Last Modified: Mon, 06 Jul 2020 21:38:55 GMT  
		Size: 160.5 MB (160524352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220c09bcfd36563328dcee914d907b2ac560b60dd0781fe19ace76711fb53b64`  
		Last Modified: Mon, 06 Jul 2020 21:38:05 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13d79c2d205cdf794973fea0f1aa9c087c9a85901c3f373cd5c77e5ac32d2ec`  
		Last Modified: Mon, 06 Jul 2020 21:39:24 GMT  
		Size: 47.9 MB (47903960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61851923be19902942e52b0785058080d78ecf21e8d823c271884523f1faaf01`  
		Last Modified: Mon, 06 Jul 2020 21:39:01 GMT  
		Size: 182.9 KB (182901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a516dc792b7d327c63282ad3fd0f6709115c1c6c3acb156368c73d1a29d944b`  
		Last Modified: Mon, 06 Jul 2020 21:39:01 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccbf3fc9692bbb7ab7bae50edef2aa33a1bc43311d22b3cc59a322f218663ff`  
		Last Modified: Mon, 06 Jul 2020 21:39:02 GMT  
		Size: 3.5 MB (3491844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940f03fdc72a2c2c79b26bbe99f8aba936d9c36d5088b7290ad4e3a2a831a546`  
		Last Modified: Mon, 06 Jul 2020 21:39:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62aadec43ce4df450dba6ea86bdfa51bc1a3076cee4b6a2d8c9707302a2fe488`  
		Last Modified: Mon, 06 Jul 2020 21:39:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fbd49e142bf0f05a16e6764f3691ae6e24e530ef7c902a79644292c4781627`  
		Last Modified: Mon, 06 Jul 2020 21:40:08 GMT  
		Size: 110.5 MB (110546752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812f080fb3f5e11cd719fc20011d70992c9da1044996b4dc0a77da6d234400d5`  
		Last Modified: Mon, 06 Jul 2020 21:39:36 GMT  
		Size: 13.0 MB (13033225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a678585590959d17014a0ff3708de1375e1138c55814ccab45ebffbbb0207f76`  
		Last Modified: Mon, 06 Jul 2020 21:39:31 GMT  
		Size: 642.3 KB (642259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd71cc9108976f622f55c4e48883c08537ae0d21d9e878f4f8095ec2c7d803ab`  
		Last Modified: Mon, 06 Jul 2020 21:39:32 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ba0794227fdb0e7eec754570a24e6c10f8430cc3959c116b1752936686165a8d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396068981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e333a3d7c1468f53f9432aea899f285736c04ce012acf02c9385998f1cb22f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:04:54 GMT
ADD file:090a5d48524c4b10f867bf6bb80c106a69bf839c876de86912ed0c633349a1ab in / 
# Mon, 06 Jul 2020 22:04:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:04:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:05:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:05:01 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:27:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:27:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:27:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 06 Jul 2020 23:53:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Mon, 06 Jul 2020 23:53:18 GMT
ENV LANG=C.UTF-8
# Mon, 06 Jul 2020 23:53:18 GMT
ENV LC_ALL=C.UTF-8
# Mon, 06 Jul 2020 23:59:43 GMT
ENV ROS_DISTRO=eloquent
# Tue, 07 Jul 2020 00:02:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:02:37 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jul 2020 00:02:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jul 2020 00:02:39 GMT
CMD ["bash"]
# Tue, 07 Jul 2020 00:03:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:03:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jul 2020 00:04:06 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jul 2020 00:04:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:04:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jul 2020 00:04:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jul 2020 00:04:43 GMT
ENV ROS1_DISTRO=melodic
# Tue, 07 Jul 2020 00:04:44 GMT
ENV ROS2_DISTRO=eloquent
# Tue, 07 Jul 2020 00:06:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:07:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:07:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 00:07:14 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:68fe03cb170d6a5101858131ae1eac5393a4f018d70abfcd1348fd240ee0ccc5`  
		Last Modified: Tue, 30 Jun 2020 16:25:30 GMT  
		Size: 23.7 MB (23719365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18959295effbb87ec216a036a1821f8b7e183072faaa80a6d7f97aa14b51b2af`  
		Last Modified: Mon, 06 Jul 2020 22:06:58 GMT  
		Size: 35.2 KB (35189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51118fb70ce38c0c2e667ecd5fc941590875e2fd9e55dd17c90073f085ba5970`  
		Last Modified: Mon, 06 Jul 2020 22:06:58 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a5d9eae931d5a3b5a3bcb840e11167c2d3d03ec22258cde67197babf908ed`  
		Last Modified: Mon, 06 Jul 2020 22:06:58 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d832c02196e6213b1651ccaa0dabb3dedd688a3b944828d5a8537aae66e232a`  
		Last Modified: Tue, 07 Jul 2020 00:23:34 GMT  
		Size: 838.0 KB (838034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18f0c890bda61fd31b0a228ebb697678ff4e414e11aa836080255171c9ada0c`  
		Last Modified: Tue, 07 Jul 2020 00:23:34 GMT  
		Size: 4.5 MB (4451086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81284b34b727283f9902f672b693ab335abbea095ae97288197de593fc1efeb`  
		Last Modified: Tue, 07 Jul 2020 00:23:33 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e16952fda1a36cc173ffb18645d840db8413723c7cdd36232cbf70d5985af`  
		Last Modified: Tue, 07 Jul 2020 00:31:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b53975bfde69cb453080cced07ce5207af4d8dca90399e6a8a2eff2bf2adb5`  
		Last Modified: Tue, 07 Jul 2020 00:34:06 GMT  
		Size: 172.5 MB (172542172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94fc169c9bad1c23213bfa43e7fd73b703130a21870046ba11a4ec51b832a69`  
		Last Modified: Tue, 07 Jul 2020 00:33:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b7667b7f222eb0bf0a1e5e08433e8a4479edd10c76f8e88918004883fa53e`  
		Last Modified: Tue, 07 Jul 2020 00:34:26 GMT  
		Size: 56.2 MB (56213333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537af487893d08127ffbfc44c93e57f2af02817eb66f92b6347b71e118f7b620`  
		Last Modified: Tue, 07 Jul 2020 00:34:13 GMT  
		Size: 182.9 KB (182906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7217b423ebafca1a4d0d9fcbdb4665bc140133f4660fa7b120f9577443744dcd`  
		Last Modified: Tue, 07 Jul 2020 00:34:13 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe726d62e5e0d09c69752cd0114135a38c4ae569ef87cd5251245bfae3a2646`  
		Last Modified: Tue, 07 Jul 2020 00:34:15 GMT  
		Size: 3.9 MB (3931480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c78f3ca9bf6a2062ce5a3f3f8d5818592da45b6208809f8255c44c2f24e2f6`  
		Last Modified: Tue, 07 Jul 2020 00:34:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120a11c10a18c5db6c2de8c3e2f94c20fd23076119defeeb39b9726afa7100bf`  
		Last Modified: Tue, 07 Jul 2020 00:34:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b6bc39c388d68aec9b486aa30672463c9069364c96de44ecb9c36c2862a930`  
		Last Modified: Tue, 07 Jul 2020 00:35:11 GMT  
		Size: 116.6 MB (116615915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03050a1b06f46ded48a68ef7e56329f0c5c862be6d85ca9655111546f595abd`  
		Last Modified: Tue, 07 Jul 2020 00:34:41 GMT  
		Size: 16.9 MB (16889670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854f6a65baadcf51c815c8e6652c1e6bb42a5f888e397a3da68a115e4d4b0d08`  
		Last Modified: Tue, 07 Jul 2020 00:34:34 GMT  
		Size: 644.3 KB (644273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ad1c65a845f5511956437d0a32a29c5ec94cd414a3ab0784a3bac90689726d`  
		Last Modified: Tue, 07 Jul 2020 00:34:33 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
