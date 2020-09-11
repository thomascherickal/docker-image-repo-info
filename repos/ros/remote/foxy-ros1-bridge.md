## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:2ca8db64c21108679c72b1922ab8783ab14eec9a1a75f455d0880bf0fd9ad91b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:2c8d7d955404a70aabfcf460eef0130642b2f38b0b539f45440284d37472ce8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.2 MB (340219634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90cee1c8e26173f90e964d6076f4099193051e2a0f93d55f32ca9a1ed58beb67`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:34 GMT
ADD file:9f937f4889e7bf6467d34e7ac4f093054993a93399443dc7469d53750a62234f in / 
# Wed, 19 Aug 2020 21:14:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:39 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:56:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:10:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:10:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 20 Aug 2020 00:30:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 20 Aug 2020 00:30:24 GMT
ENV LANG=C.UTF-8
# Thu, 20 Aug 2020 00:30:24 GMT
ENV LC_ALL=C.UTF-8
# Thu, 20 Aug 2020 00:30:24 GMT
ENV ROS_DISTRO=foxy
# Thu, 20 Aug 2020 00:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:31:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 20 Aug 2020 00:31:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 20 Aug 2020 00:31:20 GMT
CMD ["bash"]
# Thu, 20 Aug 2020 00:31:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:31:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 20 Aug 2020 00:32:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 20 Aug 2020 00:32:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:32:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 20 Aug 2020 00:32:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 20 Aug 2020 00:32:16 GMT
ENV ROS1_DISTRO=noetic
# Thu, 20 Aug 2020 00:32:16 GMT
ENV ROS2_DISTRO=foxy
# Tue, 01 Sep 2020 23:56:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.8-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 23:05:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.3-7*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 23:05:45 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:54ee1f796a1e650627269605cb8e6a596b77b324e6f0a1e4443dc41def0e58a6`  
		Last Modified: Wed, 29 Jul 2020 15:19:55 GMT  
		Size: 28.6 MB (28558017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bfea53ad120b47cea5488f0b8331e737a97b33003517b0bd05e83925b578f0`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d371e02073acecf750a166495a63358517af793de739a51b680c973fae8fb9`  
		Last Modified: Wed, 19 Aug 2020 21:16:55 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66c17bbf772fa072c280b10fe87bc999420042b5fce5b111db38b4fe7c40b49`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa557cc6371ecdf29da34fb9617bb250fff91a99f8d09bd3b5f4ba454d5c4d8b`  
		Last Modified: Wed, 19 Aug 2020 23:11:16 GMT  
		Size: 1.2 MB (1175798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d14d67fb1371eab29e8b3ebd3cc38806d01da3fe7d7dacf2ee8fe215c2f74b`  
		Last Modified: Thu, 20 Aug 2020 00:42:13 GMT  
		Size: 5.5 MB (5546328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f0cb43f8f135cf525d89b3ea013f7c5b7c19e56d68b80ca9c9473ad7f98f2`  
		Last Modified: Thu, 20 Aug 2020 00:42:11 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bef4bdda2da36783e1bf00a1c99b386fc7130a92dff0242646a81c8879e60f3`  
		Last Modified: Thu, 20 Aug 2020 00:48:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a194702420ea560879a75664cf83b50f5e1a80c30255f164e3c4d42f6c0bd5b4`  
		Last Modified: Thu, 20 Aug 2020 00:48:50 GMT  
		Size: 119.3 MB (119325706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd87ad3bb30fdce533ab5c821d5b574e321a8badc8f3ba557547c4b4ac80c1d`  
		Last Modified: Thu, 20 Aug 2020 00:48:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf01c9494f348cdc30a318c91f4af127ecf106148f44c7e53dc6c903d43fcf5`  
		Last Modified: Thu, 20 Aug 2020 00:49:08 GMT  
		Size: 66.6 MB (66578193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564e0662a79ca83816c38b8eed1750a75349c62328faab5b3b7cdc67ab1efccd`  
		Last Modified: Thu, 20 Aug 2020 00:48:55 GMT  
		Size: 191.2 KB (191189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d21aeee94d4d2159f98a39d6ef4104c2c0e96f7f37234e4824319a59a32c58b`  
		Last Modified: Thu, 20 Aug 2020 00:48:54 GMT  
		Size: 2.0 KB (2008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b3328bf471d3974e574e59d0bd60cf133a94644471ffb2ef88c5d0af31205`  
		Last Modified: Thu, 20 Aug 2020 00:48:58 GMT  
		Size: 10.3 MB (10278123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3dc358cbd8b97ceabbeaa8d72660dbcc25374a2174d7b4e81190c9eea48f6`  
		Last Modified: Thu, 20 Aug 2020 00:49:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951d604a7521e8261e253308d15f92147aacbef32ff17722d578158e276de950`  
		Last Modified: Thu, 20 Aug 2020 00:49:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d4c3ca3f37769f4de65a7bf043acfbec125fefbb2073909c8c7ae84d93e3c`  
		Last Modified: Tue, 01 Sep 2020 23:59:45 GMT  
		Size: 76.1 MB (76091425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01955843cfe58a7ff1c2919c7d9289a004b6c8ec0f5a656bcda55a46cfea2aaa`  
		Last Modified: Fri, 11 Sep 2020 23:07:09 GMT  
		Size: 32.4 MB (32437043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07deba9e1b5006a6ceb3f6d220c4f12e41c6a2446675c0815de52a1044b5eee7`  
		Last Modified: Fri, 11 Sep 2020 23:07:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f49712537a352fd2341162b5184a25e0447ce8de3f2c3157d912adf13af16c55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308884612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec6e07752247901e933a95235ca49839fded25da84acfca9b2fe710470cb3cb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:30:23 GMT
ADD file:a332d170aaa2d4c28c85289b62d33de68027ce4d6b0616292ee2252dfdf2628b in / 
# Wed, 19 Aug 2020 21:30:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:30:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:30:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:30:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:24:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:47:03 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 19 Aug 2020 23:47:04 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 23:47:05 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 23:47:10 GMT
ENV ROS_DISTRO=foxy
# Wed, 19 Aug 2020 23:49:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:49:14 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 19 Aug 2020 23:49:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:49:19 GMT
CMD ["bash"]
# Wed, 19 Aug 2020 23:50:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:50:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 19 Aug 2020 23:51:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 19 Aug 2020 23:51:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:52:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 23:52:20 GMT
ENV ROS1_DISTRO=noetic
# Wed, 19 Aug 2020 23:52:21 GMT
ENV ROS2_DISTRO=foxy
# Tue, 01 Sep 2020 23:04:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.8-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 23:15:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.3-7*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 23:15:07 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:61ca5746b6ffb91caaaa0eb4b9678ae147ad24bd40ac203758a90af376976f98`  
		Last Modified: Wed, 29 Jul 2020 08:25:33 GMT  
		Size: 27.2 MB (27162745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d07cd4558d7ea5ba152468ba362cbf62a56cfab14976467187d3943013a932`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 32.3 KB (32335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ef536d7ca531a0dce4a70ac7ad7d9b7ed27c56c7f0953bbec370e4299b951`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d5c7c4a6e93095601576a7663dde336974f6a96329ae2a613511662ed8744`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4083e46f11503c80095b52102ecdb34f1f88359ab6776daee0f399dd71c60372`  
		Last Modified: Thu, 20 Aug 2020 00:11:52 GMT  
		Size: 1.2 MB (1176161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7764603dd05c49038a524211ad7ceb67d2670cab2505beea1af401cca1e779`  
		Last Modified: Thu, 20 Aug 2020 00:11:48 GMT  
		Size: 5.5 MB (5511900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036f7ca74d2d186cd0993ac4fc4b9cef66c4777f93b40d28474a8e487429514f`  
		Last Modified: Thu, 20 Aug 2020 00:11:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570794c6903fc984991682fb63b7f759d52aa83c56c5a79a9d052dc142414524`  
		Last Modified: Thu, 20 Aug 2020 00:20:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfe2c97a91ece4c8c65879e94f05bb84074d61dc62373e8b0d236186be5ff4e`  
		Last Modified: Thu, 20 Aug 2020 00:20:35 GMT  
		Size: 103.5 MB (103548323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b4d5cd498be33da61888884aea8cc59b55d642839c5eba1747d3a8c6786f8`  
		Last Modified: Thu, 20 Aug 2020 00:20:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4c3d8d25318eb83758d2d30ed2f1d9fd5e6b1f3dfccdeccfdf454a0143d1bd`  
		Last Modified: Thu, 20 Aug 2020 00:21:20 GMT  
		Size: 60.9 MB (60932505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2965af5207117f40fe6f9d41af3649d263a565580ad7e4907a045951a9170d7`  
		Last Modified: Thu, 20 Aug 2020 00:20:45 GMT  
		Size: 191.2 KB (191246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8013e5d039e1fc0dc8abedd1d18ff0699a56be442911b93da40c9ad8c498cf06`  
		Last Modified: Thu, 20 Aug 2020 00:20:45 GMT  
		Size: 2.1 KB (2071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50e78bc3e96c1568399cf4ef0d0715cbb0e1eb5c810899b33aa7500a7b960b`  
		Last Modified: Thu, 20 Aug 2020 00:20:49 GMT  
		Size: 9.3 MB (9296651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b63c645fe7df2c3603f3e0a88ad087e075da93cbc5d54cc210d1d8f8343788`  
		Last Modified: Thu, 20 Aug 2020 00:21:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfc536064d2292929e76f128ae30f1d34333a0cd7b3f6c6be7cf008f0fc46dd`  
		Last Modified: Thu, 20 Aug 2020 00:21:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9b2e92a4f24b92e8985bdf9d5aecf60132e8a2d41f4a14d3605fa33a77e7d6`  
		Last Modified: Tue, 01 Sep 2020 23:17:14 GMT  
		Size: 76.1 MB (76130988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf09136d7a07047994dbbe9f2a67cc407776803e061b68d2ef3f94f203a1cd`  
		Last Modified: Fri, 11 Sep 2020 23:16:23 GMT  
		Size: 24.9 MB (24896190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d594e53c499300c55afed539e750fb85230243647bea0b6ace6a7d89a0f4106f`  
		Last Modified: Fri, 11 Sep 2020 23:16:14 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
