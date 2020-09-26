## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:ccad7b7e34cce6d66bd3097d074a154e38486c29bfa570e9e1d3a3ab9024153c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:d971c1deb7908c2e2fcd89563e2dfd3cbf71d7ce1fa623473a9ed276438a5732
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **805.9 MB (805926496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d03514d136ddcf804900f2f09b7da8b0acebc78dcdf4ba9bd3ccf2842342e44`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:13:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:46:37 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:46:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 01:46:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 01:46:39 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 01:46:39 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 01:46:39 GMT
ENV ROS_DISTRO=noetic
# Sat, 26 Sep 2020 01:48:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:48:41 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 26 Sep 2020 01:48:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 01:48:42 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 01:49:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:49:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 01:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:56:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac7e7e50c4ec78d366977925188b5bcceefc778ad809bbacacfddc2494cf44d`  
		Last Modified: Sat, 26 Sep 2020 00:33:06 GMT  
		Size: 1.2 MB (1176627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fee3294cf809591a86eaf42ab53997f7449cba60d6811bbd5d634d5bb436241`  
		Last Modified: Sat, 26 Sep 2020 02:17:06 GMT  
		Size: 5.5 MB (5547147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86eb1d49055c694a2de0fb058693277298e8663cce6066ecbf8caddc195623d`  
		Last Modified: Sat, 26 Sep 2020 02:17:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec3e7a48c90b648f321856ec9dcb74fe2fd4df42af73c2ccc147fcf167408d0`  
		Last Modified: Sat, 26 Sep 2020 02:17:05 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d54d9cb0354c59bf2deeb13a4962c4ea2866f115912193d10e5455ff90c2a92`  
		Last Modified: Sat, 26 Sep 2020 02:17:50 GMT  
		Size: 173.1 MB (173095331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b85c5812dfbf95f0d8953f73c266aa97ed0260112b57661bc77f9909ef16a01`  
		Last Modified: Sat, 26 Sep 2020 02:17:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af34eb18aefe49b2a0c7f05667591a0578807c4f5c2849f5163c624e3ba245f2`  
		Last Modified: Sat, 26 Sep 2020 02:18:06 GMT  
		Size: 46.4 MB (46377224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c876f634a64a593d88036af336eec2abff4a6793f9a64740a5da133523891162`  
		Last Modified: Sat, 26 Sep 2020 02:17:55 GMT  
		Size: 232.7 KB (232739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81915fb3ed87472d71d1e55c0c79ef93aa877a201ff4f65eb9ba6a3235237d`  
		Last Modified: Sat, 26 Sep 2020 02:18:12 GMT  
		Size: 79.6 MB (79590005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656c312722ee72e0430a94982845ad3c0e5bea81817f15db68a1a16d6d5f08ae`  
		Last Modified: Sat, 26 Sep 2020 02:20:00 GMT  
		Size: 471.3 MB (471346527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:1aa516ed0b6c516370f536136aa633e39f3bf98bcabd2e0473c91a524cd94a19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **701.9 MB (701899899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b06f4164332716e224accc7ab9c1889bde3820f98afe0675eaa86b2459002bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:05:07 GMT
ADD file:545bf1be9048265e6c534b9b28f9f47c4a67fe2fe7331c7652187f3b43999005 in / 
# Fri, 25 Sep 2020 23:05:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:05:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:05:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:05:14 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:03:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:03:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:04:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:04:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:04:15 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 00:04:16 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 00:04:18 GMT
ENV ROS_DISTRO=noetic
# Sat, 26 Sep 2020 00:06:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:06:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 26 Sep 2020 00:06:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:06:55 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:07:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:07:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:08:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:39f6a73f1e6a145d93dd5878cc833f3930759e9c59f35905b5ebbcfba8669f0d`  
		Last Modified: Fri, 25 Sep 2020 23:06:54 GMT  
		Size: 24.0 MB (24038486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde417f16107c5260abc78817e22ed7d1fa0eab20e58929e4265b9b782fbc020`  
		Last Modified: Fri, 25 Sep 2020 23:06:47 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b336701abcacc2258baaa4f6e1714b011d5ca0ddbc5231e18f2b7b050b9bfb3`  
		Last Modified: Fri, 25 Sep 2020 23:06:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1365c477ebb042985a05bdae57de2b67b864fe7131f13f5318d0c57cb19327`  
		Last Modified: Sat, 26 Sep 2020 00:47:24 GMT  
		Size: 1.2 MB (1177969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc4d3c40b4137bf9ba4ddae9ace53bac9f385ca5df38b8d5f9d82ae11403a05`  
		Last Modified: Sat, 26 Sep 2020 00:47:22 GMT  
		Size: 4.7 MB (4676373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225de48c4fdf5e54861f963be8a02ef0268b5a129c77554a6db6c17a6ae9735`  
		Last Modified: Sat, 26 Sep 2020 00:47:21 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cad782b0d7b1df7e6473d2bdb593c99de90dffcb1100a59b55d2e36bd0ff2c`  
		Last Modified: Sat, 26 Sep 2020 00:47:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2347f7891e6e7300eb8f46b9c8343cb6249b75b27afa77f71bea88c2c6cb1f2`  
		Last Modified: Sat, 26 Sep 2020 00:49:16 GMT  
		Size: 157.0 MB (156979809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28701a4beb918795eba0f50ecea8573aa7b7ca59120e2e84f6f1d84a58bab8d`  
		Last Modified: Sat, 26 Sep 2020 00:47:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241300aa269922053e62935f01f2786cb91b09628e898ace847fa35cfc477acf`  
		Last Modified: Sat, 26 Sep 2020 00:49:36 GMT  
		Size: 35.8 MB (35827377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c7fe0ebc3c16b6d3be0872e2d096c4ef400e528beffc9589d7197cec7cb37e`  
		Last Modified: Sat, 26 Sep 2020 00:49:26 GMT  
		Size: 232.8 KB (232807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad39776f83d9b04f408774314a8192f809f79d9c07efabe82b7d736e4d36c180`  
		Last Modified: Sat, 26 Sep 2020 00:49:46 GMT  
		Size: 60.5 MB (60480670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193ce23161920d2f9ae023c93be457040b98c5a2a5e4842a97f51436253523bc`  
		Last Modified: Sat, 26 Sep 2020 00:52:09 GMT  
		Size: 418.5 MB (418483528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3707ca722cadbac4cf547c68155476e91c323ae72b5495a34e2a5088e3640400
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **758.3 MB (758275818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cab0180ff841cf6b4424914314424167ebafdfcdf13fe45cb4c0cc54f67997e8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:29:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:30:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:30:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 26 Sep 2020 00:30:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 26 Sep 2020 00:30:20 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 00:30:21 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 00:30:21 GMT
ENV ROS_DISTRO=noetic
# Sat, 26 Sep 2020 00:32:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:33:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 26 Sep 2020 00:33:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 00:33:03 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 00:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:34:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 00:35:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:42:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db17de9ee086c8cf49c0e639054452f6def306454fe50eda3538a35c79eed983`  
		Last Modified: Sat, 26 Sep 2020 01:25:43 GMT  
		Size: 1.2 MB (1177850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35334acab583a62d3a1c5dab26403057290155b7316de791ed4676213dbc439`  
		Last Modified: Sat, 26 Sep 2020 01:25:40 GMT  
		Size: 5.5 MB (5513770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668066e878dafb1b5c1b2edf67108e6433da5f4e07accd083d5063d1c44181de`  
		Last Modified: Sat, 26 Sep 2020 01:25:39 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f78561d780428ca5c9bef896c1c6412a49f68cc26162d21032141ed0da0a0d`  
		Last Modified: Sat, 26 Sep 2020 01:25:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba6ae69e78f00876df695738ab7f9e90825c92f6e1d3d7640c121b7f7525e73`  
		Last Modified: Sat, 26 Sep 2020 01:27:57 GMT  
		Size: 167.6 MB (167568440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512017c2299e1da98d85c174b25d3e53badf8f2ba5b3e3e7a86b5a06ed79eef9`  
		Last Modified: Sat, 26 Sep 2020 01:25:39 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12072f41d71c912aeca09d8aabee465dab9ef8d5fcd89bfa8c2b6622d6ef9d9b`  
		Last Modified: Sat, 26 Sep 2020 01:28:25 GMT  
		Size: 40.6 MB (40629845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8eea5868d3229cad8484cf190df3230591e4511f00fdc59114ce964f4f5e36`  
		Last Modified: Sat, 26 Sep 2020 01:28:10 GMT  
		Size: 232.8 KB (232790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaa53405816c9919f6e3c5724fb7703c45b5a24d2a76112757bae209f07786c`  
		Last Modified: Sat, 26 Sep 2020 01:28:50 GMT  
		Size: 72.0 MB (71973707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0af97a837edbc7dca83503e0a749097e50e4a8ed54ea1753bca381e7412f190`  
		Last Modified: Sat, 26 Sep 2020 01:32:08 GMT  
		Size: 444.0 MB (444016420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
