## `ros:dashing-ros1-bridge`

```console
$ docker pull ros@sha256:891ef7abf16972d3ab29ef07d2c32f8e371e5b6cab52f6605fb01121ac5454f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:2383f3e0db2c01fb4eda47814ab5e5fc2c7aea9091800c89280ecb6e0682cee1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423871720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7503e4c89684b4266a15725e6b6f55796ba072043b10b2afabfed5a09e6e800c`
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
# Tue, 07 Jul 2020 00:59:40 GMT
ENV ROS_DISTRO=dashing
# Tue, 07 Jul 2020 01:01:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:01:42 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Tue, 07 Jul 2020 01:01:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 07 Jul 2020 01:01:42 GMT
CMD ["bash"]
# Tue, 07 Jul 2020 01:02:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:02:36 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 07 Jul 2020 01:02:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 07 Jul 2020 01:02:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:03:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jul 2020 01:03:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jul 2020 01:03:01 GMT
ENV ROS1_DISTRO=melodic
# Tue, 07 Jul 2020 01:03:01 GMT
ENV ROS2_DISTRO=dashing
# Tue, 07 Jul 2020 01:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:05:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.5-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:05:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:05:08 GMT
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
	-	`sha256:e64ec253cf63014d094d19567a8da6a7e725d8f384748380b7b5742d041d8676`  
		Last Modified: Tue, 07 Jul 2020 01:24:45 GMT  
		Size: 184.7 MB (184738881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163e825dce7ff7b71340f5cb8800f5b845075f6559aa0e30a0315d110832360d`  
		Last Modified: Tue, 07 Jul 2020 01:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aad74b8bc11161a5c855d1f017cfb4ccb3e88a25721bd7fb0ab689d6c335db3`  
		Last Modified: Tue, 07 Jul 2020 01:25:06 GMT  
		Size: 64.1 MB (64121069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97e93a13099ab4b8e82ea0f2a28f5ebafd89f3d129651565c0a4eafcfcf3657`  
		Last Modified: Tue, 07 Jul 2020 01:24:55 GMT  
		Size: 184.3 KB (184269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ea715600c5baf12f1ee00844da2734d41923315a97b76ed4f94112559eb108`  
		Last Modified: Tue, 07 Jul 2020 01:24:54 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7768073418fa143ae4946d0dcb3c8995cad1d8817fe56f87ef8fe7859690f248`  
		Last Modified: Tue, 07 Jul 2020 01:24:56 GMT  
		Size: 4.3 MB (4311978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff7355d1dfb00f2715ed1f2c9d78fddcecafe099faa3d18bebe29a674f17067`  
		Last Modified: Tue, 07 Jul 2020 01:25:13 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2029f653ebab171789929ff99f4f998c806fa7efba044e5933f3af5044f0c20`  
		Last Modified: Tue, 07 Jul 2020 01:25:14 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3b4b7aefc1e5fd46d37790e3bbacfc1a640f9724f5c369ff714c61cd2287a0`  
		Last Modified: Tue, 07 Jul 2020 01:25:40 GMT  
		Size: 117.7 MB (117662511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbf44fba0d25835f577233d4178800afa1eb6c5713b486354f53006cd6a474c`  
		Last Modified: Tue, 07 Jul 2020 01:25:19 GMT  
		Size: 19.8 MB (19772862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be94da0ad37941b6e2f3679500baf74202369e4d9bfae0155acf3ab7f13505d`  
		Last Modified: Tue, 07 Jul 2020 01:25:13 GMT  
		Size: 637.9 KB (637877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51784d5b9d42900c8409d9f3eed7a6535b9c8f30d20293bdf18032381a30fe52`  
		Last Modified: Tue, 07 Jul 2020 01:25:12 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:4d9eae897488857bc93e88f44fc962709eabdd9539fca52e0aaea588d8e55bc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.6 MB (358632596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce92027daec288387845e3fd0c7eff90663fa828d721a59a07ffa7707d22600`
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
# Mon, 06 Jul 2020 21:14:13 GMT
ENV ROS_DISTRO=dashing
# Mon, 06 Jul 2020 21:16:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:16:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 06 Jul 2020 21:16:38 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 06 Jul 2020 21:16:39 GMT
CMD ["bash"]
# Mon, 06 Jul 2020 21:17:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:17:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 06 Jul 2020 21:17:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 06 Jul 2020 21:18:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:18:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 06 Jul 2020 21:18:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 06 Jul 2020 21:18:23 GMT
ENV ROS1_DISTRO=melodic
# Mon, 06 Jul 2020 21:18:23 GMT
ENV ROS2_DISTRO=dashing
# Mon, 06 Jul 2020 21:20:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.5-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:21:00 GMT
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
	-	`sha256:ed14af26bf696e9b1ebc05e1b83b74dd9f2316d9768460a6b1dea63546589407`  
		Last Modified: Mon, 06 Jul 2020 21:36:47 GMT  
		Size: 157.5 MB (157470852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b664b79b817fad4a7c0401bb77ef803944e18c94e98e741a5ad8486abb2293`  
		Last Modified: Mon, 06 Jul 2020 21:36:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1094f2bf44f399431e1e9ba5113c3c20665aff3740bd63aa602e96adaac2274`  
		Last Modified: Mon, 06 Jul 2020 21:37:06 GMT  
		Size: 48.5 MB (48525301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03512150159215db24d1de2d385eb31ee98253bbc5cf779205f54fdc0e6a1865`  
		Last Modified: Mon, 06 Jul 2020 21:36:52 GMT  
		Size: 184.3 KB (184324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c45c880e63693aba3183f0c1ba1ef8d44b9d04cde7810268eb079d459ce02f6`  
		Last Modified: Mon, 06 Jul 2020 21:36:53 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51b6671edb7366e82eb2ff6bd72592bc7b9f79acc2b6438db924de308a0087f`  
		Last Modified: Mon, 06 Jul 2020 21:36:54 GMT  
		Size: 3.2 MB (3249261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc73040a99459caf5394a68ff9ee2c5e8e3bfc18be06dea46084e9df52aea866`  
		Last Modified: Mon, 06 Jul 2020 21:37:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0654e421bf100b9ee9a5f1ecb1b46051addaea360b99b15cc19680cf62012d4`  
		Last Modified: Mon, 06 Jul 2020 21:37:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf397e4203cd5f77ed4a98446793ff33f2965f02f66523522e438f9c31942d27`  
		Last Modified: Mon, 06 Jul 2020 21:37:52 GMT  
		Size: 110.5 MB (110539999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abbf08b68f858b71ac2103fff84994c7fc1f044dad1694647f6f081e17365f`  
		Last Modified: Mon, 06 Jul 2020 21:37:19 GMT  
		Size: 10.8 MB (10789411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6242e463c55b47023ea8761fde1ba2edc51fa38fdec8bb610ecd647473084b56`  
		Last Modified: Mon, 06 Jul 2020 21:37:14 GMT  
		Size: 634.3 KB (634317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7506ed824f7e75e780929e7f5e4768e8fea996f456a0b651d932f48f9a14e2b`  
		Last Modified: Mon, 06 Jul 2020 21:37:14 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ed2672593a72d057fc706e148c0a013edc6ea41c71af74e69ca0e0bfb605447a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.1 MB (391116130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249f77d53e1b604350524ea24a928181c3208e46ae34aafe4e1c51cf0f25cdf8`
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
# Mon, 06 Jul 2020 23:53:20 GMT
ENV ROS_DISTRO=dashing
# Mon, 06 Jul 2020 23:55:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:55:17 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Mon, 06 Jul 2020 23:55:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 06 Jul 2020 23:55:19 GMT
CMD ["bash"]
# Mon, 06 Jul 2020 23:56:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:56:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 06 Jul 2020 23:56:38 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Mon, 06 Jul 2020 23:56:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:57:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 06 Jul 2020 23:57:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 06 Jul 2020 23:57:13 GMT
ENV ROS1_DISTRO=melodic
# Mon, 06 Jul 2020 23:57:14 GMT
ENV ROS2_DISTRO=dashing
# Mon, 06 Jul 2020 23:58:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:59:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.5-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:59:32 GMT
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
	-	`sha256:849d3cc65af8fdbd7bc2a4b0b8e15d62edfaafc829324834dcdb21a9c5242487`  
		Last Modified: Tue, 07 Jul 2020 00:32:01 GMT  
		Size: 169.2 MB (169209770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf524f2e0455d81baee2dd1ea3ac4d295a2fe9858422717528e338c3efe89e`  
		Last Modified: Tue, 07 Jul 2020 00:31:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651dee978f9f5b0f8a3e817bbcd7c785408c3ece5595762ac51f5ffe55d9052b`  
		Last Modified: Tue, 07 Jul 2020 00:32:27 GMT  
		Size: 56.8 MB (56833774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0948d88dc94912e1bc6528ae4cd0f8b3b9eb200bbf8b2bc9cb2670b02db4b32`  
		Last Modified: Tue, 07 Jul 2020 00:32:12 GMT  
		Size: 184.3 KB (184324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3da4d089f31e1194a14e9c2ce5981285bec09a97998711e4c56f6a10256ce`  
		Last Modified: Tue, 07 Jul 2020 00:32:12 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847fd1b53f958d2a107eeac5b9a300cb5d83a85d348c15608e5b3d13f3a46403`  
		Last Modified: Tue, 07 Jul 2020 00:32:13 GMT  
		Size: 3.7 MB (3664483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e903e99f185a84c56a26bec119555c017384ccff35e3551d24a6b3b3274868`  
		Last Modified: Tue, 07 Jul 2020 00:32:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d1c60df9e6c591f01a7920a262fbc973574dae4cbbf6f436e1bb246d1749cc`  
		Last Modified: Tue, 07 Jul 2020 00:32:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c7a6c644508dfbe7c0fb42a6ed16618d7eaae02aece795c6f3d856dba98c1`  
		Last Modified: Tue, 07 Jul 2020 00:33:14 GMT  
		Size: 116.6 MB (116607560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca06b5ffc881d9bdd22a36cc655da363eb840e109b14cd71492f14dd1bf958`  
		Last Modified: Tue, 07 Jul 2020 00:32:40 GMT  
		Size: 14.9 MB (14931216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1983a70221e2903c85b4dc0ab979c34cd008fdb99628253ecac43e385b2f9820`  
		Last Modified: Tue, 07 Jul 2020 00:32:33 GMT  
		Size: 635.8 KB (635762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9af7540090812daaf1f91564aef8b5b4d2315f3b513c162b2fbec542f5e70`  
		Last Modified: Tue, 07 Jul 2020 00:32:33 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
