## `ros:dashing-ros1-bridge-bionic`

```console
$ docker pull ros@sha256:662ded050e6b59779e97de4349b7302ccea11847b93a32f19663423fc291709b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros1-bridge-bionic` - linux; amd64

```console
$ docker pull ros@sha256:c85631eee05dc86a5d2e19d5f39f5126ce76b84a9ba93707d710b88e9d931e55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **418.5 MB (418505476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21486cf0dd60e44c537a6bcea2fa66aabd787aabd3981cd757f0aaaf6921a28`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:03:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:36:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:36:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 01:56:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 26 Sep 2020 01:56:55 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 01:56:55 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 01:56:55 GMT
ENV ROS_DISTRO=dashing
# Sat, 26 Sep 2020 01:58:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:58:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 01:58:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 01:58:44 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 01:59:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:59:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 01:59:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 01:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:00:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 02:00:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 02:00:02 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 02:00:02 GMT
ENV ROS2_DISTRO=dashing
# Sat, 26 Sep 2020 02:01:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:02:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:02:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:02:08 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e9ed312e3419a4c4db0767b3098eb605e89291c6ec52e2a1f9267e0d4e036`  
		Last Modified: Sat, 26 Sep 2020 00:26:41 GMT  
		Size: 838.7 KB (838713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d81648d8ff08a7289511d85e20283d98b1cd6482eb1f7c88c91c5f80800da7b`  
		Last Modified: Sat, 26 Sep 2020 02:14:26 GMT  
		Size: 4.9 MB (4870910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1b1f09e5649b589ba73073a9fc1b0c2d2ec436cbd20d5a9e3844701142bf4b`  
		Last Modified: Sat, 26 Sep 2020 02:14:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf91780e2a3fdf08fe9f79bb72ac102cddc77502f5077400437c81041f94e7`  
		Last Modified: Sat, 26 Sep 2020 02:20:07 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30fee8dcdc4199aac03ca4d0ea655776d032903e4099c4c1b702efcd760b19`  
		Last Modified: Sat, 26 Sep 2020 02:20:44 GMT  
		Size: 179.4 MB (179394094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ba58eae24bd8d8af9d250ce8e1281c2a39cf547cdb22e9aca149a719f058d3`  
		Last Modified: Sat, 26 Sep 2020 02:20:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271a63dc9f9cf95aa1a9791151351656dfcd600714004ddf7b846050d1a10ab8`  
		Last Modified: Sat, 26 Sep 2020 02:21:00 GMT  
		Size: 64.1 MB (64125999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ea0f6c1d03c5dcb63602e4bdcc5209a6a5ea1db02f4fe5f02a41ee58280e57`  
		Last Modified: Sat, 26 Sep 2020 02:20:48 GMT  
		Size: 189.9 KB (189873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309ef61e26bf94afef7889897008abe4d54e33c564eeb8465d2251ba33fca77`  
		Last Modified: Sat, 26 Sep 2020 02:20:48 GMT  
		Size: 2.0 KB (2025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f3bd42b0d6d349e2e318513d6e8cc5cf79c9d5576e4bea02507f1452dcd6f1`  
		Last Modified: Sat, 26 Sep 2020 02:20:50 GMT  
		Size: 4.3 MB (4313013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c294af85e4a31787403c64953f04a8c394f6233aea3314eaa9491341f944f4b`  
		Last Modified: Sat, 26 Sep 2020 02:21:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9573113d2726345b354d71efed3d8963d5466fccef3685570d6fc3f48054578`  
		Last Modified: Sat, 26 Sep 2020 02:21:06 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f589551b770c09a00258bee13b8da064df9a0cf4e6309b07f8592ee036f88fde`  
		Last Modified: Sat, 26 Sep 2020 02:21:35 GMT  
		Size: 117.6 MB (117639492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70dfaf5de29933ddce5f1ca46c14e3a882f91dfc18e1b3add48878a87e8891d6`  
		Last Modified: Sat, 26 Sep 2020 02:21:13 GMT  
		Size: 19.8 MB (19787441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b124b9e4a6b2abee1dd884828c760eb2e53a6a374a56bc0576d4839db813d7`  
		Last Modified: Sat, 26 Sep 2020 02:21:07 GMT  
		Size: 638.8 KB (638830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271bb643001f4769ad63460df5b034004207bbfb444c12eb620f9cd0718886d8`  
		Last Modified: Sat, 26 Sep 2020 02:21:06 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:2d41316bdddf47bf0db3be9a11aa3c2ee4ecb458775d8bcaf3029a4c901032bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.7 MB (354660910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4b7e2ae37b64ecc25116c54fed282306d54cab4b731e1d6792a92338d59f8e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:04:32 GMT
ADD file:0ddc5fefae097a5be4c925fdfc09e4a637b74627a8981f0e6fb9890580adc875 in / 
# Fri, 25 Sep 2020 23:04:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:04:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:04:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:04:40 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:52:17 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:52:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:52:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:15:04 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 26 Sep 2020 00:15:05 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 00:15:06 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 00:15:07 GMT
ENV ROS_DISTRO=dashing
# Sat, 26 Sep 2020 00:17:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:17:43 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 00:17:44 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:17:47 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:20:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:20:28 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:20:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 00:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:23:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:23:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:23:39 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 00:23:41 GMT
ENV ROS2_DISTRO=dashing
# Sat, 26 Sep 2020 00:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:27:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:27:23 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:20e126218ac644f56ef7147c3363108a0814d921e6016af54a1b4c964159f1a9`  
		Last Modified: Fri, 25 Sep 2020 23:06:39 GMT  
		Size: 22.3 MB (22279517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d156c2b31482935ec0363b6e3f1cb6fc56da57e61fc80078914918fe53f8fa5`  
		Last Modified: Fri, 25 Sep 2020 23:06:34 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1a0dbe2162972438aa89d4f90dca5db0e4cee58819ba354ea1c0031101b7a`  
		Last Modified: Fri, 25 Sep 2020 23:06:34 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb78937af11e41b8b67fc193c013f76d8597e2901f9207cb60bcc96c6494422`  
		Last Modified: Sat, 26 Sep 2020 00:43:43 GMT  
		Size: 838.9 KB (838879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bcc9cef45fa068e47d37c7bc183a512bea02bfcff3e7e007e458352c5a37ca`  
		Last Modified: Sat, 26 Sep 2020 00:43:42 GMT  
		Size: 4.1 MB (4085050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd428060fb74592076e296fd161a779da260ddd29b8f39ec36bfe7e0e4ef7ef`  
		Last Modified: Sat, 26 Sep 2020 00:43:41 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7422b314a6e26cdf55febdd3ab72288b5ddec15c283f99baee45ab2faa20a3`  
		Last Modified: Sat, 26 Sep 2020 00:52:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063bc9560c2a7e478463e6f04405ee2ea5cc2639905a834cbebe104ef5f7a136`  
		Last Modified: Sat, 26 Sep 2020 00:53:00 GMT  
		Size: 153.5 MB (153527444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217869449fd4c684ceebc3248fc61506c4a10fb6529c672e82b07bd4f6b0791`  
		Last Modified: Sat, 26 Sep 2020 00:52:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc122089dd4749fa715c03527f166d340d1a9ba4500ef3ea8de8e3e50fd6f08`  
		Last Modified: Sat, 26 Sep 2020 00:53:21 GMT  
		Size: 48.5 MB (48528951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6247062a443176534f8de64a793d1c1d3e046ad24b5f54de243c4bfe3e8c8391`  
		Last Modified: Sat, 26 Sep 2020 00:53:08 GMT  
		Size: 189.9 KB (189936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7ed62f2b9cd3fcba149fbf92d0298723e11f21b2832ad4f49a2acaad4d7685`  
		Last Modified: Sat, 26 Sep 2020 00:53:08 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0a429e950da7a97f648a14b13db508ae0f5368e92da3390e64e598cf9be9c2`  
		Last Modified: Sat, 26 Sep 2020 00:53:11 GMT  
		Size: 3.2 MB (3248999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d28121b612100bbaf523da64df086e60cfebf0716a4a097c1a42a68beb7421`  
		Last Modified: Sat, 26 Sep 2020 00:53:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16de8ecdcdcbc7ccbf797ab5e104d20db99674a742fcd592a1022cb0a7e84053`  
		Last Modified: Sat, 26 Sep 2020 00:53:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e6ee48f566e1cfdd41ebe185e75262d0240f3490192e36e272b1659d9c3e9a`  
		Last Modified: Sat, 26 Sep 2020 00:54:10 GMT  
		Size: 110.5 MB (110520500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17fc034d3a616963087ee899161ae82c11b881839e1ae9a04ac0c5397df99e0`  
		Last Modified: Sat, 26 Sep 2020 00:53:35 GMT  
		Size: 10.8 MB (10801241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b39abb668b335f745dd21aecf22924ae981e8c405504dec0c4e189616775b77`  
		Last Modified: Sat, 26 Sep 2020 00:53:29 GMT  
		Size: 634.8 KB (634830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3d1243c1d8651b3536017ec7fc0d9985f11e0d265a93266fefcf8925302b8c`  
		Last Modified: Sat, 26 Sep 2020 00:53:29 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros1-bridge-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c3cc5e72072b367a817549f0832f4efd4b9dce64323c1be3778c78b330caeaa7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.0 MB (386984124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e6710d8dc5c73537b1b0af0431aa3fac77f1ea58cb0a64eb291802cffe0029f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:15:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:15:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:15:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:46:11 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 26 Sep 2020 00:46:12 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 00:46:13 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 00:46:13 GMT
ENV ROS_DISTRO=dashing
# Sat, 26 Sep 2020 00:48:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-core=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:48:05 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 00:48:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:48:06 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:49:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:49:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:49:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 00:49:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros-base=0.7.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:50:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:50:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:50:38 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 00:50:39 GMT
ENV ROS2_DISTRO=dashing
# Sat, 26 Sep 2020 00:52:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:52:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-dashing-ros1-bridge=0.7.6-1*     ros-dashing-demo-nodes-cpp=0.7.9-1*     ros-dashing-demo-nodes-py=0.7.9-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:52:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:52:59 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439dc9be551df0db43e033037c5edecb4f62c1cf032cd594c89b97fd64a4d80`  
		Last Modified: Sat, 26 Sep 2020 01:20:50 GMT  
		Size: 838.6 KB (838621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb52ce07f5181ce3dadb81cde965981cf2a21bb0b2b54e7b90093cf47d209fa`  
		Last Modified: Sat, 26 Sep 2020 01:20:48 GMT  
		Size: 4.5 MB (4452875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27879dbd83ca4a72a76730e433a5be8582971dd48fa1b6ef75b4b500c0f81e51`  
		Last Modified: Sat, 26 Sep 2020 01:20:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9c7aae51fb63cd27c56ff14ce5374474258619eaf124ec4d53b6f06ff60a46`  
		Last Modified: Sat, 26 Sep 2020 01:32:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a9d4705a9cfe694453c68d07b2811c1ff2fc0556ee05a73e82e862e2f45fac`  
		Last Modified: Sat, 26 Sep 2020 01:33:25 GMT  
		Size: 165.1 MB (165083799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8982857d7f4e3987e074142b6408c426a92eb9f5e305435e0cfd11c9d53559`  
		Last Modified: Sat, 26 Sep 2020 01:32:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68b23c4d3cdecd8e9b6672a5b0ce4b7a9a02f6e90ef88f1ca6f20ff782c7c6d`  
		Last Modified: Sat, 26 Sep 2020 01:33:54 GMT  
		Size: 56.8 MB (56838351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c73fa6080b2487ed8f24f989f7481a67e4b15cb6407737cd15f4731b3e1b4a3`  
		Last Modified: Sat, 26 Sep 2020 01:33:35 GMT  
		Size: 189.9 KB (189931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b1b7fd639b5ad4ccf92b5fc75391abd4d98d7f76bff1c7ab4e2a0007a6f08f`  
		Last Modified: Sat, 26 Sep 2020 01:33:34 GMT  
		Size: 2.1 KB (2067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3db54c562b40c80ca4ce51e187f6590664e013be1d7e4d2c3314d266c7239d`  
		Last Modified: Sat, 26 Sep 2020 01:33:40 GMT  
		Size: 3.7 MB (3664593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7368c0dc01ed925ebb3a8480d6b2263aa60004bb94c7d730f917b3c68c944333`  
		Last Modified: Sat, 26 Sep 2020 01:34:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea78c6fe759173b94237062cc2d429d5032024001f666cb56bd56a0281f0483`  
		Last Modified: Sat, 26 Sep 2020 01:34:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd9d30d9801a7d5bed6cf6f38cd71921a64012c5117b596fe8543ac3c35b153`  
		Last Modified: Sat, 26 Sep 2020 01:35:14 GMT  
		Size: 116.6 MB (116610059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11b7c374ae54bb6fbc3994bc583d8cd36f8a3e7dcbdef7c6582b234ba33ed4`  
		Last Modified: Sat, 26 Sep 2020 01:34:18 GMT  
		Size: 14.9 MB (14942038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d491cb1d835cfd1850d8fcc6fadf6aeb4dc17bec5d4f5c94c48b2921784c79`  
		Last Modified: Sat, 26 Sep 2020 01:34:04 GMT  
		Size: 635.4 KB (635430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d404c3966567bbdff8eab726d35336b0a032457a3a084ce1d892a12f4bbd08`  
		Last Modified: Sat, 26 Sep 2020 01:34:03 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
