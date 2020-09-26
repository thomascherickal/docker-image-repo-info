## `ros:eloquent-ros1-bridge`

```console
$ docker pull ros@sha256:c5fa03444159d19784cdbc567cb1e8f59ce6ef205bc601d12d65fccd170594c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:78b3d75283631046a3f1a358aa6b84d7fd112241ee3fd46f0a99e4d30cb57edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.9 MB (423913767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca0a1850edfa83433cce42df2ec700f4761cc71320680e01bb9f530c86da1e6`
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
# Sat, 26 Sep 2020 02:02:16 GMT
ENV ROS_DISTRO=eloquent
# Sat, 26 Sep 2020 02:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:03:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 02:03:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 02:03:21 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 02:04:00 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:04:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 02:04:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 02:04:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:04:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 02:04:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 02:04:22 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 02:04:22 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 26 Sep 2020 02:05:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:05:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:05:34 GMT
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
	-	`sha256:6efed6f5d6878c6e07c7b00215f5bb1a8b07c04ca00230ccaa850c0b32bd5d8b`  
		Last Modified: Sat, 26 Sep 2020 02:22:18 GMT  
		Size: 183.0 MB (182970582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb6c1589b3701cd599e1248397085b4b6a2bed8387b1910e6978c1b3314d347`  
		Last Modified: Sat, 26 Sep 2020 02:21:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77a69bb6ed964d144a50c7a8f99975cba2bdaf1a69acc81dfe7f3d55e894ec3`  
		Last Modified: Sat, 26 Sep 2020 02:22:34 GMT  
		Size: 63.5 MB (63506069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d263b9e866ccd9a9b27b5fad2dc931eab58e67cfffe40cd8ee3e7c2255a45f`  
		Last Modified: Sat, 26 Sep 2020 02:22:22 GMT  
		Size: 189.2 KB (189227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7820542f2661176e2d33b74f31e7091069cefcb07cf72fcb2ba8e29d9d089aae`  
		Last Modified: Sat, 26 Sep 2020 02:22:22 GMT  
		Size: 2.0 KB (2028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a82d191da6529fcff2ab647817e7691a3f8f90b49be3326b0c32a3686e108ea`  
		Last Modified: Sat, 26 Sep 2020 02:22:24 GMT  
		Size: 4.6 MB (4581043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383a44cb173c3374589fcd81413a733eefcf995f4f82f85de165468a32dadc98`  
		Last Modified: Sat, 26 Sep 2020 02:22:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6894273d1c3f30afe2f7bf7b2cf7d67c156d50559d3d9745d906845cc6b9485e`  
		Last Modified: Sat, 26 Sep 2020 02:22:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3d3acead4b22fd842ce1cf4927c94ccc4717e7e513ea5794955498d15e6a8`  
		Last Modified: Sat, 26 Sep 2020 02:23:08 GMT  
		Size: 117.6 MB (117647944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c32bd8985dc9d30c11225548787188d14950d764222f4ca130ca83068452f64`  
		Last Modified: Sat, 26 Sep 2020 02:22:46 GMT  
		Size: 22.0 MB (21955189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcc6c837186cf1c3587e358c96e7e6c347ba3ef9ae4c573157571922742b401`  
		Last Modified: Sat, 26 Sep 2020 02:22:39 GMT  
		Size: 647.0 KB (646975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ecb185af5ae7b6a769ce5a6e99ff80074555e32633023f28d328956f351d3`  
		Last Modified: Sat, 26 Sep 2020 02:22:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm variant v7

```console
$ docker pull ros@sha256:8df866b5036f753a1920dd21cbbed43daeb24df8be8a06f0f16e27305c30315d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.6 MB (359584276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5ee2eb0837824a4af927d920608b15e6d189733d7e5a7d27d99cab912859d4`
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
# Sat, 26 Sep 2020 00:27:52 GMT
ENV ROS_DISTRO=eloquent
# Sat, 26 Sep 2020 00:30:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:30:12 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 00:30:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:30:16 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:32:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:32:22 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:32:34 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 00:33:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:34:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:34:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:34:09 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 00:34:11 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 26 Sep 2020 00:36:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:36:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:37:12 GMT
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
	-	`sha256:fb096cb22fd7cc70b176784de7a9e369f827c4df8d41fb01cf767a9391eb6cac`  
		Last Modified: Sat, 26 Sep 2020 00:55:57 GMT  
		Size: 156.6 MB (156570177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12775ecccd94f4e80dcaf1590e07b3c89d44ccaea20d954ca444d0c560d4c7d2`  
		Last Modified: Sat, 26 Sep 2020 00:54:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4094882c81503a3bceb805b289c04795840c7648470596f092dc1e66d64cfdc4`  
		Last Modified: Sat, 26 Sep 2020 00:56:20 GMT  
		Size: 47.9 MB (47906814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec79f8b2972775aeb69517a26c6fbf5619aa9c176c90942e360af12630c0408`  
		Last Modified: Sat, 26 Sep 2020 00:56:08 GMT  
		Size: 189.3 KB (189291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73f4865a2113daff43f028e50ec83fcff802f9a9e8ce59d607839f45f6d3762`  
		Last Modified: Sat, 26 Sep 2020 00:56:08 GMT  
		Size: 2.0 KB (2020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e092c30e21d7bdcb9eea9a6cd5e5f4c8e5b416237ca9bdb83cd7ea88778cedb3`  
		Last Modified: Sat, 26 Sep 2020 00:56:11 GMT  
		Size: 3.5 MB (3492176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecec5e9be520358b081d793c2bc5075ec3ddbdd822ffd1621b088d9013ea3893`  
		Last Modified: Sat, 26 Sep 2020 00:56:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f009ca9f3590d599b15079a74c054ac0b2bf818aa3d372170133308e373220f7`  
		Last Modified: Sat, 26 Sep 2020 00:56:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4d29ccf229ede683afcf7f142cdc24dd9ed20d272b0a7b591043cf89cc9daa`  
		Last Modified: Sat, 26 Sep 2020 00:57:10 GMT  
		Size: 110.5 MB (110528397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63d2cabbc85509ac06b4a4fea047061fae9c3cbf06ebe452ea0237aa7235b0f`  
		Last Modified: Sat, 26 Sep 2020 00:56:35 GMT  
		Size: 13.0 MB (13045966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75481fc6c3ca8cd1de1c0ffd74eab870068a7eed570a81340b408d1448cd27d1`  
		Last Modified: Sat, 26 Sep 2020 00:56:30 GMT  
		Size: 642.5 KB (642483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb7a512e12a3e9ef9d817338f48f8f1ae70bc7aecc2e182cadf461947571a34`  
		Last Modified: Sat, 26 Sep 2020 00:56:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:edd8a9dadecc65f8d4b7639856982c7215675b432ddb0526d1489b04c65adf99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.9 MB (391866938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a226c5440f5abe1478defb8bd7afa6adc23ab3ea8eb79179cea1e3968d357bb`
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
# Sat, 26 Sep 2020 00:53:13 GMT
ENV ROS_DISTRO=eloquent
# Sat, 26 Sep 2020 00:55:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:55:16 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 00:55:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:55:17 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:56:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:57:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:57:11 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 00:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:58:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:58:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:58:14 GMT
ENV ROS1_DISTRO=melodic
# Sat, 26 Sep 2020 00:58:15 GMT
ENV ROS2_DISTRO=eloquent
# Sat, 26 Sep 2020 01:00:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-comm=1.14.9-1*     ros-melodic-roscpp-tutorials=0.9.3-1*     ros-melodic-rospy-tutorials=0.9.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:00:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros1-bridge=0.8.2-1*     ros-eloquent-demo-nodes-cpp=0.8.4-1*     ros-eloquent-demo-nodes-py=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     python-rosdep     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:00:42 GMT
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
	-	`sha256:baf6adca2bc1df9757d832e0d423e3df4ab5ab610d0bfd4cea9bb81f3a309bc4`  
		Last Modified: Sat, 26 Sep 2020 01:36:24 GMT  
		Size: 168.3 MB (168347915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df6193ac7f2730205a43435bc43e222399ba81eca2e16870e93833d36c64d8e`  
		Last Modified: Sat, 26 Sep 2020 01:35:22 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5b68578aaed76bf04d85bde5ca2ad493939e837c71c70e8193092de7935c69`  
		Last Modified: Sat, 26 Sep 2020 01:36:47 GMT  
		Size: 56.2 MB (56215938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc188eeb9b9f33cf751358f0b46c3d50fed283bcea6d46a0375e7e03b410056c`  
		Last Modified: Sat, 26 Sep 2020 01:36:32 GMT  
		Size: 189.3 KB (189289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d321ecd8de8dcdf5f104c78239ec3658ff559c9d57419fd30986a2bf0ac55784`  
		Last Modified: Sat, 26 Sep 2020 01:36:33 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6b01d669e05741b51100b5ad478c41c64fbf3f66ce88eb9db6e24499229223`  
		Last Modified: Sat, 26 Sep 2020 01:36:36 GMT  
		Size: 3.9 MB (3931695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d58e4df357b97373d9f2532a614bc3d6cb5bc1709244b1cb4ec4e0a60712d3`  
		Last Modified: Sat, 26 Sep 2020 01:36:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649641b578ee8e1df126f7fca4220c78fb5e82a085f74ca80eaeb142f1e590a5`  
		Last Modified: Sat, 26 Sep 2020 01:36:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fdab3d91095c9200d14713fdf0826a486cb2a850bbb9849f7d8a0cddda9421`  
		Last Modified: Sat, 26 Sep 2020 01:37:56 GMT  
		Size: 116.6 MB (116619248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95086b86b323995ce5f80a94bd400547edefc946743a1963f79539994a34542`  
		Last Modified: Sat, 26 Sep 2020 01:37:15 GMT  
		Size: 16.9 MB (16898378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc318b05f568a3f3450d4012a167f8284ad2b957d9c8f180d198bc7fe6aa5af`  
		Last Modified: Sat, 26 Sep 2020 01:36:56 GMT  
		Size: 644.6 KB (644573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f212cda67160e28372a11850d2813d59082a6fff42a0dfe87ea19528dee3e9`  
		Last Modified: Sat, 26 Sep 2020 01:36:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
