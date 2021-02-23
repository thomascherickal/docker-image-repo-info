## `ros:rolling-ros1-bridge-focal`

```console
$ docker pull ros@sha256:ecdc13bbdbebf4108ef9bd686a7c38e2b3c103505e4aa65b7100538507b2bdfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:0bbfec39d1c459c6e75667008758a09d9e28e8ee9dd288d6cdcb030db2dd7974
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.6 MB (335582196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fd048cf284f793549589efe02a98b22671bfb31124926382ba63d350b195f9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 08:38:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:13:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:13:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 11:34:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 21 Jan 2021 11:34:23 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 11:34:23 GMT
ENV LC_ALL=C.UTF-8
# Thu, 21 Jan 2021 11:38:04 GMT
ENV ROS_DISTRO=rolling
# Thu, 21 Jan 2021 11:38:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:38:59 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 21 Jan 2021 11:38:59 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 21 Jan 2021 11:39:00 GMT
CMD ["bash"]
# Thu, 21 Jan 2021 11:39:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:39:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 21 Jan 2021 11:39:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 21 Jan 2021 11:39:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:40:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 11:40:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 21 Jan 2021 11:40:07 GMT
ENV ROS1_DISTRO=noetic
# Thu, 21 Jan 2021 11:40:08 GMT
ENV ROS2_DISTRO=rolling
# Thu, 21 Jan 2021 11:40:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 22 Feb 2021 20:55:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.12.0-1*     ros-rolling-demo-nodes-py=0.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 22 Feb 2021 20:55:08 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b329de66e00a76df07e660eb83a5097f2bbaca25d0f8030ae04b2a9045d726e`  
		Last Modified: Thu, 21 Jan 2021 08:55:02 GMT  
		Size: 1.2 MB (1181953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ca6f3074dc19264c495086cc66977079fd2553a4803bff7061524587caeff8`  
		Last Modified: Thu, 21 Jan 2021 11:47:40 GMT  
		Size: 5.5 MB (5547368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b12fc1d4ab992cb14f16c7af9bd19f75b5fd82db79e4e925e38bcb4969667`  
		Last Modified: Thu, 21 Jan 2021 11:47:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4b846f1510e05ec2e9f03bfbb1e0865f69dcb23742f4f04590bed5d988feb`  
		Last Modified: Thu, 21 Jan 2021 11:54:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473d7c7711794b1c585dd584be338c44f3b523d8987710c5cb9e6a9cedf08494`  
		Last Modified: Thu, 21 Jan 2021 11:56:17 GMT  
		Size: 119.9 MB (119894720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adf58a25a3026bb6417f5d53984a109397e3d1a3db800b7fc7060be3bcef9af`  
		Last Modified: Thu, 21 Jan 2021 11:55:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9931a4c4aa1f78db8a58a95ed3986e7074d6397fd6bef4f64fe0ffcb6110f224`  
		Last Modified: Thu, 21 Jan 2021 11:56:38 GMT  
		Size: 66.6 MB (66552280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471df9c82773a57f977e34f0bc724500b950aee774681a3d745f013563ddaf2c`  
		Last Modified: Thu, 21 Jan 2021 11:56:23 GMT  
		Size: 198.9 KB (198861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be3f1637f36fbf3d765d91eeac6c7da21a83c3437c4e93d1373e3932e66cc7e`  
		Last Modified: Thu, 21 Jan 2021 11:56:23 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee9487e697c515124855093ee1b809d6d434447dd94fd02bc8e39f228d6d0dc`  
		Last Modified: Thu, 21 Jan 2021 11:56:30 GMT  
		Size: 22.3 MB (22275392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab42eae2e1741f33d4a6baeb51a4be9124551a0a5704f6e93f86439441f67b27`  
		Last Modified: Thu, 21 Jan 2021 11:56:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e76c34382344dd0602cb504a09c42cc58f51e973ea24bf6cda837c24bb6105`  
		Last Modified: Thu, 21 Jan 2021 11:56:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0278dad1afef84e07b4ad0e00dd5d3d8bbc21b6f2c1d3ec37d989a2b79fb3e41`  
		Last Modified: Thu, 21 Jan 2021 11:57:08 GMT  
		Size: 76.1 MB (76122511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e25ea0222a8f49803184b1635fe6823a495092dd98fee28205c73946908989`  
		Last Modified: Mon, 22 Feb 2021 20:56:38 GMT  
		Size: 15.2 MB (15237754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2d6343033680ed35960bee43efb5b4c2787476ee20c5e8cdebc73621ebf57f`  
		Last Modified: Mon, 22 Feb 2021 20:56:34 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:97aeb3dc20c99a3f49d36503c8433695eeb4be5a6b13441ca2c38e17e12a1fcc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308617816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc7223e7d9561c2642759544063f81c9f14c9b4c56adea376136c907fd0dd22`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:45:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:45:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:45:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 07:09:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 21 Jan 2021 07:09:09 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 07:09:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 21 Jan 2021 07:14:48 GMT
ENV ROS_DISTRO=rolling
# Thu, 21 Jan 2021 07:16:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:16:39 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 21 Jan 2021 07:16:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 21 Jan 2021 07:16:42 GMT
CMD ["bash"]
# Thu, 21 Jan 2021 07:17:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:17:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 21 Jan 2021 07:18:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 21 Jan 2021 07:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:19:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 21 Jan 2021 07:19:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 21 Jan 2021 07:19:17 GMT
ENV ROS1_DISTRO=noetic
# Thu, 21 Jan 2021 07:19:18 GMT
ENV ROS2_DISTRO=rolling
# Thu, 21 Jan 2021 07:20:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.9-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 22 Feb 2021 20:50:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros1-bridge=0.10.1-1*     ros-rolling-demo-nodes-cpp=0.12.0-1*     ros-rolling-demo-nodes-py=0.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 22 Feb 2021 20:50:15 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf194558d7d697893645e2928d8c12f602b77dd0aaf2f5344233277d7b160d1`  
		Last Modified: Thu, 21 Jan 2021 07:29:34 GMT  
		Size: 1.2 MB (1183038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f15cd3db3fa7d5351aa9b332d57ca02a4276fef9f7b3363ef98b2c4f9611d8`  
		Last Modified: Thu, 21 Jan 2021 07:29:31 GMT  
		Size: 5.5 MB (5514280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67e6495e9d3639f76b9c4f19a8a602bcf7fe068fb7b7f08ee8cba855c1f301`  
		Last Modified: Thu, 21 Jan 2021 07:29:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba3fea46fa21f2e435af76ebf72934a3b25fc18e9d03b07f583304b0335d7e`  
		Last Modified: Thu, 21 Jan 2021 07:36:44 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe15401fa20919feee7ef656cc89d14e3fd4588d3acf9afa81ba5d694e418`  
		Last Modified: Thu, 21 Jan 2021 07:38:55 GMT  
		Size: 104.0 MB (103959553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65506f9e42a413dd004c5ca05f35b5c93d44d17eaaaed4ecb4a0ba086f6d5788`  
		Last Modified: Thu, 21 Jan 2021 07:38:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cb10bf9dab8eb9804d307c75f6f9bbd32e7c44b246c486243b21d832e9c76d`  
		Last Modified: Thu, 21 Jan 2021 07:39:29 GMT  
		Size: 60.9 MB (60916470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b67cfd545dfe0a02a40ee2e48799f77df6ad16188aec7af2b8b825e0aee06f`  
		Last Modified: Thu, 21 Jan 2021 07:39:16 GMT  
		Size: 198.9 KB (198915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a946c6ab8cde674a07a2c180f1524bc4fae61a10c18f7db345664a8498e1d9`  
		Last Modified: Thu, 21 Jan 2021 07:39:16 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60d6fed229d22b0a8f7e78d2c929ad203ee660769e5dffbf7865d88ad2fddb2`  
		Last Modified: Thu, 21 Jan 2021 07:39:20 GMT  
		Size: 20.9 MB (20941494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5ed917db6ef6b506817f3237dc6e9a3f959c1f9ae16149e308e3f0e6fa71b`  
		Last Modified: Thu, 21 Jan 2021 07:39:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce8b3b65709e415a646e5f7175809c44f997933362d87f1af96207d5950cfd2`  
		Last Modified: Thu, 21 Jan 2021 07:39:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115d86a384366eda9a5a905f8823eb46d1bfef41f0cce84ce75279415bfed89b`  
		Last Modified: Thu, 21 Jan 2021 07:40:10 GMT  
		Size: 76.2 MB (76170532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76a03f1c70dfe84e67b6fe06cc43d4035fd9c0f4e44bd455abc8f9e297ba35`  
		Last Modified: Mon, 22 Feb 2021 20:51:58 GMT  
		Size: 12.6 MB (12555044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc64ec45774df70b7974f054ace3a94d6ecbf8187e0454e7d445e757c92e112d`  
		Last Modified: Mon, 22 Feb 2021 20:51:55 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
