## `ros:eloquent-ros1-bridge`

```console
$ docker pull ros@sha256:bc81cc5994cc6b7bb597bddcf6f8178968d671db862095d3f3d0e5b8e3ea398c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:5900875c3b5c48ba4fcd0e90038f6c31b9cd22b3c8027d9e1a345e8c95f77b60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423915232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14106a2dc033d421c1bc8e079615897b0ba0deb7b8fec2afb978d4a5cb0a0cbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:14:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:27:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:27:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 05:48:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 05:48:08 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:48:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:53:44 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 05:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:54:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 05:54:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:54:48 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 05:55:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:55:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 05:55:33 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 17 Jun 2020 05:55:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:55:47 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 05:55:48 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 05:55:48 GMT
ENV ROS1_DISTRO=melodic
# Wed, 17 Jun 2020 05:55:48 GMT
ENV ROS2_DISTRO=eloquent
# Wed, 17 Jun 2020 05:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:56:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:57:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:57:05 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64a7083ea96b95855d3cee6bcab14b90b20d9bfd209d123ecb0caa88322c7ae`  
		Last Modified: Wed, 17 Jun 2020 03:31:48 GMT  
		Size: 837.6 KB (837600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc602a4d0af8ead24cc13540f49a0fff8887a95b19f7167d71c673468d08954e`  
		Last Modified: Wed, 17 Jun 2020 06:03:08 GMT  
		Size: 4.9 MB (4867669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13ebfa6253ab146de4b680f495660841c32931dfc6640051a14000c8c18ac49`  
		Last Modified: Wed, 17 Jun 2020 06:03:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22b4d4694e78be7232b3d308841e35b90c3f15975115584463ca3eb734f81b5`  
		Last Modified: Wed, 17 Jun 2020 06:08:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dbba4e323e93c2e7319117cf60d51465bef774f27ea2e8be04a1a4920e5a1b`  
		Last Modified: Wed, 17 Jun 2020 06:11:23 GMT  
		Size: 183.0 MB (182960509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e559b1e43395acc7e375c1e56941c4b220d965384f03fda5576b0aa99734c`  
		Last Modified: Wed, 17 Jun 2020 06:10:44 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057a06318d08a24b3a2a56ce23b1a6132b4fd2744b1ee56b5e6123f96d3d1e58`  
		Last Modified: Wed, 17 Jun 2020 06:11:40 GMT  
		Size: 63.5 MB (63500930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7a82a4f3b76648a7bc08f90588a011e04217e13b29d6819a7944057fdc8d79`  
		Last Modified: Wed, 17 Jun 2020 06:11:28 GMT  
		Size: 180.6 KB (180616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f577d29332cec4345d969c2b29be2af815641bd926b1c3781a92f8707eb782`  
		Last Modified: Wed, 17 Jun 2020 06:11:29 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b1b12f80128d394f83ad318f4a553b3007d191adaa625158b9dc70f944df3f`  
		Last Modified: Wed, 17 Jun 2020 06:11:31 GMT  
		Size: 4.6 MB (4579750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e67876d47898fb3309efbd819870e3c348a7cf41c414bec838202cbe0762eb6`  
		Last Modified: Wed, 17 Jun 2020 06:11:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f699543d3422cd7fec20e17ba2a127e248cf862c05fba7d072d433cbce2885c`  
		Last Modified: Wed, 17 Jun 2020 06:11:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5e90bfa60fb2105253fab0ff95216119e81263304bc2d9dcecaeb60cd49ca8`  
		Last Modified: Wed, 17 Jun 2020 06:12:15 GMT  
		Size: 117.7 MB (117671475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff945bb483e06784611778e978e79a2706bbe27ea10c7058f4325c2b4fbd6430`  
		Last Modified: Wed, 17 Jun 2020 06:11:54 GMT  
		Size: 21.9 MB (21941361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf0f13f43eb4b1dc8a28a7bde75f36ff0af2174f3ec81ed6c4c0dd132e97b5`  
		Last Modified: Wed, 17 Jun 2020 06:11:48 GMT  
		Size: 645.8 KB (645786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819c4dd8d480b20dbd8e3df47bd4f97c64af8e45b05c384176ae8a85ff3d40b7`  
		Last Modified: Wed, 17 Jun 2020 06:11:48 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:d45431ffb82f60623d89d30d87fcfef6ed3a036ef8a571f7ef5596dd42e6f0f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359607318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c25a29223d4bbaf32a92973634bcd1ba92424fc9c27ea97d2f9af7d21e57e9d5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 02:02:00 GMT
ADD file:579f3bbed274bd8ec97aa5bfc4eb09fdcfe3e12e37fb3739f3096138b765581c in / 
# Wed, 17 Jun 2020 02:02:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 02:02:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 02:02:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 02:02:09 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:20:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:20:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:21:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:34:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 03:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:34:17 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:44:25 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 03:47:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 03:47:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:47:14 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 03:48:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:48:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 03:48:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 17 Jun 2020 03:48:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:49:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:49:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:49:08 GMT
ENV ROS1_DISTRO=melodic
# Wed, 17 Jun 2020 03:49:09 GMT
ENV ROS2_DISTRO=eloquent
# Wed, 17 Jun 2020 03:51:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:51:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:52:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:52:12 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:2d63ac53d1bca136340c80fe8b64c0b8e2d9a62eddb6fcb794c489840dc027d6`  
		Last Modified: Sat, 30 May 2020 09:27:47 GMT  
		Size: 22.3 MB (22275987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e03e3a8e7321c64d7a483fc9cc0054ce81e5b230b32300b7c68d21001f661a`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 35.5 KB (35459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0e8090890c513488a0f67683f23dcfcfbf2b67e5be854edf1323ad87a60b26`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b801ccb19e43939aa60383f674f0e1f65ab062890870d42d0fa7a7a62fc5b708`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd193992630ce3c05616b2d6384bc7261c04210de22ad6879778b9aca67aaa81`  
		Last Modified: Wed, 17 Jun 2020 03:55:51 GMT  
		Size: 838.2 KB (838177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a62e43a84ad9c1d846a6d034c6ec80467b2e21c620fd37591f04eba4cdb0c01`  
		Last Modified: Wed, 17 Jun 2020 03:55:49 GMT  
		Size: 4.1 MB (4083577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76400ef72b32df9a8e2460f1a21fdf6afb134ef4aa07c8141f7bb89eb6dcff9c`  
		Last Modified: Wed, 17 Jun 2020 03:55:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918fdc185d3fb3945554b26f476ae406a19ce7616be5e247ed94bf07f74d446e`  
		Last Modified: Wed, 17 Jun 2020 03:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa41bff48ade208264d42231471d8f6e03dcb6d4d122a9a1b5263314090c468`  
		Last Modified: Wed, 17 Jun 2020 04:02:16 GMT  
		Size: 156.6 MB (156578683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e295d701386a1ca525f379d6ffd7cc280ed098c98c41f9f2fc37595942585`  
		Last Modified: Wed, 17 Jun 2020 04:01:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21111d1ea7bd562318b0b14ca2dd21bcbf68d35b4d9b6d626a61ad3749974ce8`  
		Last Modified: Wed, 17 Jun 2020 04:02:36 GMT  
		Size: 47.9 MB (47897606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e1cbc174a620e6fd8d656a94eb92fdd3745c77d971d034adc70722c3f0ecfc`  
		Last Modified: Wed, 17 Jun 2020 04:02:22 GMT  
		Size: 180.7 KB (180666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46baede0a731c6d7d9f48172610933c0b2a93c0191af7a1738548c405b9a0b9`  
		Last Modified: Wed, 17 Jun 2020 04:02:23 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0157c3ce96a87376714d83b56fc59b2a85678bd502a03ea3d4f8f406e4094bae`  
		Last Modified: Wed, 17 Jun 2020 04:02:24 GMT  
		Size: 3.5 MB (3491708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d8dda450503aba3d3bdf1e1027ac3b40b39619caeee16d6b558a322cf175ca`  
		Last Modified: Wed, 17 Jun 2020 04:02:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376bf05470435feff1b70618bcf8284fd620b7e9c04c40d834fe1d59ccd37e0e`  
		Last Modified: Wed, 17 Jun 2020 04:02:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcf65502aad07c2713690068d96de5a9f11759e77c0202f2ac86dc47167d1ac`  
		Last Modified: Wed, 17 Jun 2020 04:03:24 GMT  
		Size: 110.5 MB (110544920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720f24f93886376737bcff04252f3ef9000cee726785daa9d361b76be287fe08`  
		Last Modified: Wed, 17 Jun 2020 04:02:53 GMT  
		Size: 13.0 MB (13032957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2b60f05deef7eb9492aba53a8c57a1467d781ac8650d12208ed1b323c7789`  
		Last Modified: Wed, 17 Jun 2020 04:02:47 GMT  
		Size: 642.0 KB (642029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51632292a6a12785ed206e57e7bf18ceaefb12dfe6d8dc056d183483b653b244`  
		Last Modified: Wed, 17 Jun 2020 04:02:47 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:62eeea52e268be082a9fd74a3c075ded10ab6e27739f64d43a9a78e4ecf883af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.9 MB (391875295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08cea067461abd0a3a30e95454579ac14d078607f6420f4d75f25cccb6771e1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:46:41 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 04:08:37 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 04:08:37 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 04:08:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 04:17:00 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 04:19:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:19:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 04:19:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 04:19:59 GMT
CMD ["bash"]
# Wed, 17 Jun 2020 04:21:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:21:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Jun 2020 04:21:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 17 Jun 2020 04:22:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:22:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 04:22:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 04:22:26 GMT
ENV ROS1_DISTRO=melodic
# Wed, 17 Jun 2020 04:22:27 GMT
ENV ROS2_DISTRO=eloquent
# Wed, 17 Jun 2020 04:24:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.6-1*     ros-melodic-roscpp-tutorials=0.9.2-1*     ros-melodic-rospy-tutorials=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:25:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:25:29 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fa5af0f7212815117da17900293ea522ed8cf971e727597f85ee658d8f8c1a`  
		Last Modified: Wed, 17 Jun 2020 04:36:48 GMT  
		Size: 838.3 KB (838254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bf6eb80e593e6f6e4ece6d710b03a4d7d8f378c1d6f2a1bef7a7b4c68009b3`  
		Last Modified: Wed, 17 Jun 2020 04:36:46 GMT  
		Size: 4.5 MB (4451304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ce79b03ccae069bcf39b72bb491ba542a576507093bcf66aaeaf82c94c1d8`  
		Last Modified: Wed, 17 Jun 2020 04:36:45 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2865f2c14406dc3fd3434efdbcb197cb35e58ae34baddd5311196da42e6b8f`  
		Last Modified: Wed, 17 Jun 2020 04:44:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24244156a34df6d325502e451abab9668b3accc6f7f8270c8d733c9649a58f01`  
		Last Modified: Wed, 17 Jun 2020 04:47:12 GMT  
		Size: 168.4 MB (168351060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed77c1acf2662e22120674aea71547c6c7697480aabe1bf3b2c6d16c7a7c3c0`  
		Last Modified: Wed, 17 Jun 2020 04:46:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffde368c20f2e7d3fc500f398f6444f61e0b218d7fcad27e58837124916b384d`  
		Last Modified: Wed, 17 Jun 2020 04:47:31 GMT  
		Size: 56.2 MB (56210080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41028aff850b808ad9f676461aafc2e53c323bb6d277a670024196215f5b926`  
		Last Modified: Wed, 17 Jun 2020 04:47:18 GMT  
		Size: 180.7 KB (180671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f775b2371ffc5b3bbc35b3fd64a5bf9c045eada0d4fdbaa066d07a676a0ef5f5`  
		Last Modified: Wed, 17 Jun 2020 04:47:18 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aaaa7a36a425f41b553f68073243fc23ffe4a3d894f1376e79c3b18ff401b18`  
		Last Modified: Wed, 17 Jun 2020 04:47:20 GMT  
		Size: 3.9 MB (3931665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4030265c2e7e3d09d74460d89996e535720adec503ac80f3eec35ab62aaf13`  
		Last Modified: Wed, 17 Jun 2020 04:47:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da973ab6bab4e47d032fbd0459fe258f5da5c46cf7e659fc323978bd010f9237`  
		Last Modified: Wed, 17 Jun 2020 04:47:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a985af1e877cef109b584d31cba78752b7319f76523254e54d65b06c4de72024`  
		Last Modified: Wed, 17 Jun 2020 04:48:14 GMT  
		Size: 116.6 MB (116615478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781e600701109b460ad34d2e836ae14cb19377104dfae183cee7c25e9fb7f1a`  
		Last Modified: Wed, 17 Jun 2020 04:47:45 GMT  
		Size: 16.9 MB (16889876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894660f2dd8918a934ee20d61b0b4de40bce25b230229dae90851bd1de066d7b`  
		Last Modified: Wed, 17 Jun 2020 04:47:38 GMT  
		Size: 644.5 KB (644453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aae129e9f9260431c58e0ea6b36aca20008c47d5f61f6bc9219cfe4152fd26c`  
		Last Modified: Wed, 17 Jun 2020 04:47:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
