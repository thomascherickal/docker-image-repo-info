## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:f589c10912e3d8f9c0c4e60307cc6a9402f2d340bf4fcb416601796c0ce19d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:084558d8fbcaafdc9edbfbeaa341c6082303d35e47ca82c54d926399125ac810
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **410.9 MB (410941003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cc01a530a45b7183d69bac50c7ae61c4174fe0467255bcaf6f0eddf707b4310`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:46 GMT
ADD file:a58c8b447951f9e30c92e7262a2effbb8b403c2e795ebaf58456f096b5b2a720 in / 
# Fri, 24 Apr 2020 01:07:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:51 GMT
CMD ["/bin/bash"]
# Tue, 19 May 2020 18:42:20 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:21:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:21:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 06 Jun 2020 01:28:17 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 06 Jun 2020 01:28:17 GMT
ENV LANG=C.UTF-8
# Sat, 06 Jun 2020 01:28:17 GMT
ENV LC_ALL=C.UTF-8
# Sat, 06 Jun 2020 01:28:18 GMT
ENV ROS_DISTRO=foxy
# Sat, 06 Jun 2020 01:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 01:29:41 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 06 Jun 2020 01:29:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 06 Jun 2020 01:29:42 GMT
CMD ["bash"]
# Sat, 06 Jun 2020 01:30:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 01:30:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 06 Jun 2020 01:30:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 06 Jun 2020 01:30:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:25:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 08 Jun 2020 22:25:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 08 Jun 2020 22:25:37 GMT
ENV ROS1_DISTRO=noetic
# Mon, 08 Jun 2020 22:25:38 GMT
ENV ROS2_DISTRO=foxy
# Mon, 08 Jun 2020 22:26:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.7-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.2-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:28:10 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d51af753c3d3a984351448ec0f85ddafc580680fd6dfce9f4b09fdb367ee1e3e`  
		Last Modified: Fri, 24 Apr 2020 01:09:34 GMT  
		Size: 28.6 MB (28556247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc878cd0a91c7bece56f668b2c79a19d94dd5471dae41fe5a7e14b4ae65251f6`  
		Last Modified: Fri, 24 Apr 2020 01:09:27 GMT  
		Size: 32.3 KB (32304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154df8ff9882934dc5bf265b8b85a3aeadba06387447ffa440f7af7f32b0e1d`  
		Last Modified: Fri, 24 Apr 2020 01:09:26 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee5db0ff82f7aa5ace63497df4802bbadf8f2779ed3e1858605b791dc449425`  
		Last Modified: Fri, 24 Apr 2020 01:09:27 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3e5de01a1b5595882fcb3da54a47556f3d36ac6a4a952bc4d2432a0715a4ad`  
		Last Modified: Tue, 19 May 2020 19:01:20 GMT  
		Size: 1.2 MB (1174766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e1d894b26307c3fd316e1b286e7ea5840bca5139148f674e741f4762eae1bb`  
		Last Modified: Wed, 27 May 2020 01:38:49 GMT  
		Size: 5.5 MB (5548577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b657ccfc9d28c3e22960d6d4680437be8bf7b2192cc35c630e1ebc462215d97`  
		Last Modified: Wed, 27 May 2020 01:38:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd2b2f951ec4c3cd203999728a6abaa97c4229dd4351c68ce8f52e573f97a2`  
		Last Modified: Sat, 06 Jun 2020 01:31:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd4e0f31b5c2ff58f693ce74853e840a69654ad358b2bdba26c9dc107e0dd52`  
		Last Modified: Sat, 06 Jun 2020 01:31:34 GMT  
		Size: 119.2 MB (119246098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280d71259757324bfa655fbc0b7f11b53a1e08a6b5306e15d250654cea592aba`  
		Last Modified: Sat, 06 Jun 2020 01:31:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b6a4d0c3917449be085ee40df95f1fdefa0aa2c47349aef5d8f16340d21b27`  
		Last Modified: Sat, 06 Jun 2020 01:32:17 GMT  
		Size: 66.6 MB (66567760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35b9aaaf404b1eb523d17887cea49c316b5fd4850f4502e215649e1f3fe44f4`  
		Last Modified: Sat, 06 Jun 2020 01:32:04 GMT  
		Size: 178.0 KB (178003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a5ee4d3bde1a6ec8bc4589897257594fe73e39c4229fce737e1966e20fb77c`  
		Last Modified: Sat, 06 Jun 2020 01:32:04 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5055412660d31f01eb69b8d54c63eee71b021138835d3a97d711ec626ac49701`  
		Last Modified: Sat, 06 Jun 2020 01:32:08 GMT  
		Size: 10.3 MB (10269093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103d4a2706bcaf30b759291a5416799e68694a7314ec55e87fa35537bab076a9`  
		Last Modified: Mon, 08 Jun 2020 22:29:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae6d246f736490d1025870ad309c2780b9a4da05eccd5f265c0be6ded3daa9c`  
		Last Modified: Mon, 08 Jun 2020 22:29:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b0c84ccd6b3cd03bce135a3a5225431568e1ffade6a71f56ac560c173690ab`  
		Last Modified: Mon, 08 Jun 2020 22:30:00 GMT  
		Size: 76.1 MB (76066390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb884dda790838d297faeed387c855f7943bbaa6bb591c31d9cb1cadc33e6cb`  
		Last Modified: Mon, 08 Jun 2020 22:30:00 GMT  
		Size: 103.3 MB (103296301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519dc623a93bcdb0a69e2451d0d5a6176654d5aff823cd839f9f9ced5c1a8df5`  
		Last Modified: Mon, 08 Jun 2020 22:29:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4687496eea48a7f0cda895782dd986b11ecd41d8a6f4623299db1826bde6d9ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.5 MB (376526752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caf3d03b87b573391233ef1ce321ceb1b99c8d3b0b97be179fc7a7f38e417bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:18:16 GMT
ADD file:e9947aff2dfa8f220d4b25dc0770aff8d9ffc08482e52f54833f39e1c3ec08bf in / 
# Fri, 24 Apr 2020 00:18:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:18:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:18:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:18:29 GMT
CMD ["/bin/bash"]
# Wed, 27 May 2020 01:42:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 06 Jun 2020 00:42:37 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 06 Jun 2020 00:42:38 GMT
ENV LANG=C.UTF-8
# Sat, 06 Jun 2020 00:42:39 GMT
ENV LC_ALL=C.UTF-8
# Sat, 06 Jun 2020 00:42:40 GMT
ENV ROS_DISTRO=foxy
# Sat, 06 Jun 2020 00:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 00:44:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 06 Jun 2020 00:44:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 06 Jun 2020 00:44:38 GMT
CMD ["bash"]
# Sat, 06 Jun 2020 00:45:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 00:45:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 06 Jun 2020 00:45:50 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 06 Jun 2020 00:46:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:50:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 08 Jun 2020 22:50:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 08 Jun 2020 22:50:49 GMT
ENV ROS1_DISTRO=noetic
# Mon, 08 Jun 2020 22:50:50 GMT
ENV ROS2_DISTRO=foxy
# Mon, 08 Jun 2020 22:52:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.7-1*     ros-noetic-roscpp-tutorials=0.10.1-1*     ros-noetic-rospy-tutorials=0.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:54:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.2-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 08 Jun 2020 22:54:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:6c2d76ba33f8d52087147ce28d8f03c08f69677591e3e10db810bf76a6e09427`  
		Last Modified: Fri, 24 Apr 2020 00:22:00 GMT  
		Size: 27.2 MB (27158644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d4cfc71d3821474946021fdbf241a74992a84c6269c3e9a052ce7fc56cece`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 32.3 KB (32326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63063bfe137200b3c8d1ee8d819124352c20ee8c189a0388f461ec66bb759310`  
		Last Modified: Fri, 24 Apr 2020 00:21:53 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38385900086ffa7d7cb9c3bbeabaf2176d7d7958ebf0736d2a01773a830201ee`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee47658e5a2b6951b5c8f1df079e5f94fa5babfcb132843f7e89a21a531555f5`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 1.2 MB (1175483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b7e5841799d26c7c96bfbade1ef6d8be3e67adbbc8402a26e6a6cf491a849`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 5.5 MB (5515489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079fbc9cd40b2782019694e3fdfea45d641b7cd63c3e41e193edc9581c050ee`  
		Last Modified: Wed, 27 May 2020 02:09:33 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3ec18d9d03c6ef880ba9e4caecbbfd50402843b4d260e38bf7d308700a606`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526f25ed5278e2e7a7fde79b21330117bd4b9e32b6b5232ae881703bdcd287aa`  
		Last Modified: Sat, 06 Jun 2020 00:47:30 GMT  
		Size: 103.5 MB (103476592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc209a31a5ea7c241b1c1de254415f9a26b41a629573e40f2deb838c76a0571`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc422b8040cae43e2cffe00a313538b1cb4403997bb7d1d04d93dd6428032d37`  
		Last Modified: Sat, 06 Jun 2020 00:47:54 GMT  
		Size: 60.9 MB (60920850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c19a97d639dd8b2ffa7aab57eb52443168bccc100f9d52ca0fec80a6bdcab3`  
		Last Modified: Sat, 06 Jun 2020 00:47:38 GMT  
		Size: 178.1 KB (178053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ec65a6dc3c1e370aff3a74854a2b8125875dfeca9bb569a2b4fb6e068fde1`  
		Last Modified: Sat, 06 Jun 2020 00:47:38 GMT  
		Size: 2.0 KB (2016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa53f0e6cd1fca763eb9c735bc6aa6e64c8b8688e32422adc1eedc51b6fc8bb`  
		Last Modified: Sat, 06 Jun 2020 00:47:41 GMT  
		Size: 9.3 MB (9288504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dccb52c7cecb474dc64dcd5b7b07f23948c3fb4379b000474612f7b0a3891e9`  
		Last Modified: Mon, 08 Jun 2020 22:56:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73153f4ba0fd700b855eacdfd7ed29fec8e3741513c32b698c742ea206ca693`  
		Last Modified: Mon, 08 Jun 2020 22:56:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74edc31afd167d6344f48a0d7f1a7e129b43a8d79bed3cf8d54b95c9b5fcbd62`  
		Last Modified: Mon, 08 Jun 2020 22:57:11 GMT  
		Size: 76.1 MB (76106158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ed8b7152a0c764b2f331c7a32c3b2c3c983207a624bc4cd782699ea79a61d4`  
		Last Modified: Mon, 08 Jun 2020 22:57:09 GMT  
		Size: 92.7 MB (92669132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc276c9fb3f870a7b08f59c67988cfcaefe2532b856de3b9dec48708e2bf77fb`  
		Last Modified: Mon, 08 Jun 2020 22:56:39 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
