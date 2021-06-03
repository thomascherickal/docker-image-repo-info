## `ros:foxy-ros1-bridge`

```console
$ docker pull ros@sha256:ed645056a7047830b65f418cc15a4546a3d30f2e368b56f6448095cdae44bca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:f725ab64b2cca6f9dac5d3c574dd328b94b43ef94d33d4bd695ba9470475c669
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.5 MB (341488404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f222f34a73dc5b3466aeed0b60fc1b677bf6ea2f4f45d33c09585b9bf768b4e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:05:34 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:28:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:25:24 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Jun 2021 19:25:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:25:25 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:25:26 GMT
ENV LC_ALL=C.UTF-8
# Thu, 03 Jun 2021 18:34:46 GMT
ENV ROS_DISTRO=foxy
# Thu, 03 Jun 2021 18:35:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:35:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 03 Jun 2021 18:35:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 03 Jun 2021 18:35:47 GMT
CMD ["bash"]
# Thu, 03 Jun 2021 18:36:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:36:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 03 Jun 2021 18:36:35 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 03 Jun 2021 18:36:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:36:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 03 Jun 2021 18:36:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 03 Jun 2021 18:36:50 GMT
ENV ROS1_DISTRO=noetic
# Thu, 03 Jun 2021 18:36:51 GMT
ENV ROS2_DISTRO=foxy
# Thu, 03 Jun 2021 18:37:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:37:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:37:36 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f60c1e15de5890db12b66dcdc9fead43b285bea7d10d147a7baddfe0093488`  
		Last Modified: Sat, 24 Apr 2021 00:20:37 GMT  
		Size: 1.2 MB (1183512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fbc9697fb73e1f55467886a56de4ed73ea1fa95a907d4eaa7cc7795c3f4438`  
		Last Modified: Sat, 24 Apr 2021 02:08:15 GMT  
		Size: 5.5 MB (5548747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184aa1c1cb1dc4ac420cdd479bbb970c33487ecba22eeb694365e55c4eb1169b`  
		Last Modified: Wed, 02 Jun 2021 19:48:54 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365d962263e1fa28cab16a988e3c87fe09253c863af7f49af060afd22aeff35e`  
		Last Modified: Wed, 02 Jun 2021 19:48:54 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb44d8dc6f43598db69e1155e5dfe27c214f4ee072bffd78ac435ada5bc356c5`  
		Last Modified: Thu, 03 Jun 2021 18:42:27 GMT  
		Size: 120.0 MB (119968675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70068e78ffe617882cf63f25d4a14ee1c0979e0c99757ddb09935ca400970aec`  
		Last Modified: Thu, 03 Jun 2021 18:42:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41dbf6d400ca15a08ec594522bcf4fa735f8bd21677e242033a4a838652d6db1`  
		Last Modified: Thu, 03 Jun 2021 18:42:55 GMT  
		Size: 66.6 MB (66603463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1007ffc2047664ef77089aa304792a11482b1932c55a62646c1c250e823b021e`  
		Last Modified: Thu, 03 Jun 2021 18:42:44 GMT  
		Size: 234.0 KB (234013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85312e107e4e7dabd08dc9a495920cfed26cb00003371036b0cef23d64ad524e`  
		Last Modified: Thu, 03 Jun 2021 18:42:44 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e27ef43293524cd653ef554630165e28dc1db74457c02fa4b30329fb66c54f`  
		Last Modified: Thu, 03 Jun 2021 18:42:47 GMT  
		Size: 10.3 MB (10284048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96112ae7110b96299f776a500df81bec4322eab50e8c26641ecc9f91a08b60f`  
		Last Modified: Thu, 03 Jun 2021 18:43:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4a7c73224a241718b84692ed06b8c052e27fb5561e78a557410bae5ae0accf`  
		Last Modified: Thu, 03 Jun 2021 18:43:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d87bc3bdf5fe88f846b4af0fc856f0b8ce5ef98b8fba2c5283c40d893f8155`  
		Last Modified: Thu, 03 Jun 2021 18:43:28 GMT  
		Size: 76.4 MB (76383857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96930dae43af22b55cacbd4f8ea98c7a581863eea860d578c6c06a730f513399`  
		Last Modified: Thu, 03 Jun 2021 18:43:19 GMT  
		Size: 32.7 MB (32736340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ecacf2711165f592a78306992ea3a051764a2d0f43eb94dac47fbe818372b4`  
		Last Modified: Thu, 03 Jun 2021 18:43:12 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b4284d42e0de520c86d30534bb226600976be5dd9469987e3027113f2f35d257
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309833464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa03886d878e0b4631657707101a4c6bef290e93e9595519141a75a6c7471e7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 May 2021 12:29:57 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Thu, 27 May 2021 12:29:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 27 May 2021 12:29:59 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 27 May 2021 12:30:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 27 May 2021 12:30:00 GMT
CMD ["/bin/bash"]
# Thu, 27 May 2021 15:09:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 15:10:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:42:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 02 Jun 2021 19:42:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 02 Jun 2021 19:42:43 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:42:44 GMT
ENV LC_ALL=C.UTF-8
# Thu, 03 Jun 2021 18:46:40 GMT
ENV ROS_DISTRO=foxy
# Thu, 03 Jun 2021 18:47:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:47:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 03 Jun 2021 18:47:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 03 Jun 2021 18:47:23 GMT
CMD ["bash"]
# Thu, 03 Jun 2021 18:47:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:47:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 03 Jun 2021 18:47:59 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 03 Jun 2021 18:48:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:48:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 03 Jun 2021 18:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 03 Jun 2021 18:48:17 GMT
ENV ROS1_DISTRO=noetic
# Thu, 03 Jun 2021 18:48:17 GMT
ENV ROS2_DISTRO=foxy
# Thu, 03 Jun 2021 18:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.11-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:48:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.3-1*     ros-foxy-demo-nodes-py=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:48:58 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c937c19c2d76950fb80c27261cfc3ba1515cd1d701bf7c5b570ce4d14a7b9688`  
		Last Modified: Thu, 27 May 2021 12:31:57 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4ad27543765699a5feb74058f25dff93de058fe2ccca9bd8f3f419d4c3d0bd`  
		Last Modified: Thu, 27 May 2021 12:31:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f05beb762e975ed5abeeb6aaf94120f220cc804c8db4d48f779491fc8d0bf`  
		Last Modified: Thu, 27 May 2021 15:42:50 GMT  
		Size: 1.2 MB (1183418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce883da7b9bc53f882d490a42da8b1853046822fc762a916e26981f92886097`  
		Last Modified: Thu, 27 May 2021 15:42:48 GMT  
		Size: 5.5 MB (5512644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203d57e854addea1192a906320cf51f2142a2d524db23871e23a49595bd80e98`  
		Last Modified: Wed, 02 Jun 2021 20:06:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ccf07d9f53e08ed2c3abd466b913f6c0c44bad7aeecf29c2abcc3af8f101fb`  
		Last Modified: Wed, 02 Jun 2021 20:06:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7cc0114ebbf8965f889b3e7d90ffb4bdecc3f4fc68b93470fc7e0055961887`  
		Last Modified: Thu, 03 Jun 2021 18:55:35 GMT  
		Size: 104.1 MB (104142629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af37e4a423aa2aac7b8fc2abd222bc62ff6861ebd2e0d22f6472061aa11d2710`  
		Last Modified: Thu, 03 Jun 2021 18:55:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8c8b382782c4824ab34e043364b5dca7bdf457588603ea252a3635c6f0c437`  
		Last Modified: Thu, 03 Jun 2021 18:55:58 GMT  
		Size: 61.0 MB (60969665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34eeb39752334763d6d232100985903d0f3bc87ed59a1a6795bd0167131b035`  
		Last Modified: Thu, 03 Jun 2021 18:55:48 GMT  
		Size: 234.0 KB (234013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818ac7b5407d044c4d2ad5c3c16a53e4c157ca4528b73e13e831d470e8b11d78`  
		Last Modified: Thu, 03 Jun 2021 18:55:48 GMT  
		Size: 2.0 KB (2020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f45bd82103fc5ea0a25e5a5b2dfc5b479dd937f36d50b4ac3cff66f2682bce1`  
		Last Modified: Thu, 03 Jun 2021 18:55:50 GMT  
		Size: 9.3 MB (9298509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2753b6a1ce1de6b54e37c69cc0e43db73d928a825f6ca4ae62f60d35242410`  
		Last Modified: Thu, 03 Jun 2021 18:56:19 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1278b043a9b45cce02f387a30c8ac6ccda8851522480abc02a59e7bd15eaf1`  
		Last Modified: Thu, 03 Jun 2021 18:56:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b24ce878bd3cb27e3696cee38148161a0a9bd553f2e55e400c4b4553ab30fb`  
		Last Modified: Thu, 03 Jun 2021 18:56:35 GMT  
		Size: 76.2 MB (76232905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abfa04ec9e90a398c513c25589cfe57729d2d6a45848c36e4923ffe03907fed`  
		Last Modified: Thu, 03 Jun 2021 18:56:23 GMT  
		Size: 25.1 MB (25109164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78536a2a54bfa48af6526e3b7ce3fc9ee9657426c39b8276ca539314ce030bac`  
		Last Modified: Thu, 03 Jun 2021 18:56:18 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
