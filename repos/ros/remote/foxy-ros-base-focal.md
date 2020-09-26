## `ros:foxy-ros-base-focal`

```console
$ docker pull ros@sha256:f469a44e759e2eba13018ca254b96d945abb9acbac8cdd906aee6842014d57d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base-focal` - linux; amd64

```console
$ docker pull ros@sha256:8c17fa41fd07ff6daeb870e83ebeaa1431262668a2a4cc2eac137cd508657036
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231716398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd925712bafa23f104cb578bb912721d13a0c79fa789c22c9aaf534b6652caf8`
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
# Sat, 26 Sep 2020 02:05:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 26 Sep 2020 02:05:51 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 02:05:51 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 02:05:52 GMT
ENV ROS_DISTRO=foxy
# Sat, 26 Sep 2020 02:06:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:06:46 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 02:06:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 02:06:47 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 02:07:22 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 02:07:27 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 02:07:30 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 02:07:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f16a159fff5cd41fcb199ffc6f5d72a234ae211ab84a79244bd1f668555b418a`  
		Last Modified: Sat, 26 Sep 2020 02:23:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01cc0e2d108a2e38e69e0b1f2b821dea42a45867611f5a36e062415bfe23d0`  
		Last Modified: Sat, 26 Sep 2020 02:23:45 GMT  
		Size: 119.4 MB (119373530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007ac1dfc028dcd61e5021e4c2591a8abd3b4401ec92f633937d645a474ed021`  
		Last Modified: Sat, 26 Sep 2020 02:23:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308577e2beb74ee81e3ad50a7945b566ec75f59ea18126ea58139aae3162f94a`  
		Last Modified: Sat, 26 Sep 2020 02:24:02 GMT  
		Size: 66.6 MB (66579361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc69a813ab602cce8a79c7606723b5a69feaf52e5f4191aeab24d307e459d9fa`  
		Last Modified: Sat, 26 Sep 2020 02:23:49 GMT  
		Size: 194.8 KB (194836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734e091dba74e322cb1f725bb1c0f400064b1ab4ace58f879a28df6b1981528`  
		Last Modified: Sat, 26 Sep 2020 02:23:49 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a66276663c17c67beab187982813cc3f77cf12533ca8457ebcc3113aa31205`  
		Last Modified: Sat, 26 Sep 2020 02:23:52 GMT  
		Size: 10.3 MB (10281994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bd4ab7b9fdf2d51f4122a51b9004a1cd6277538698b0dc36c845fcd6fccec226
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.9 MB (207885367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4e0b1ed3bb59f8b232b31e51499733707dbe109f32d6efb1c6b274e194fb02`
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
# Sat, 26 Sep 2020 01:01:23 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 26 Sep 2020 01:01:24 GMT
ENV LANG=C.UTF-8
# Sat, 26 Sep 2020 01:01:25 GMT
ENV LC_ALL=C.UTF-8
# Sat, 26 Sep 2020 01:01:26 GMT
ENV ROS_DISTRO=foxy
# Sat, 26 Sep 2020 01:03:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:03:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 26 Sep 2020 01:03:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 26 Sep 2020 01:03:38 GMT
CMD ["bash"]
# Sat, 26 Sep 2020 01:04:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 01:05:02 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 26 Sep 2020 01:05:08 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 26 Sep 2020 01:05:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e70cd470d5fc14328f40a3142c18edf2f1dff685fc0caaccc3cbf98c679818b8`  
		Last Modified: Sat, 26 Sep 2020 01:38:04 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b4a2fe3e7c5a1e1e58bbb4c26e62535715b3869ce47613970f0718fdc2d93`  
		Last Modified: Sat, 26 Sep 2020 01:38:57 GMT  
		Size: 103.6 MB (103597689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ff5a61264cf7102e198e301a829161e2457a444cb306e9ef76fc38c4a1facc`  
		Last Modified: Sat, 26 Sep 2020 01:38:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde71bedef93f7333fdd4c34eb4bfeaac93e88c53798a71d31698df10fbe841b`  
		Last Modified: Sat, 26 Sep 2020 01:39:20 GMT  
		Size: 60.9 MB (60936045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eb949a74164b19a8edd43fe4a1b1f715a42e7959944c2464d09c03ff117a56`  
		Last Modified: Sat, 26 Sep 2020 01:39:05 GMT  
		Size: 194.9 KB (194899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b402ea3e397855171e26648d2abce2dad8b730e98d23fa67ca40828489827f6`  
		Last Modified: Sat, 26 Sep 2020 01:39:05 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fdf749f4cdd8183d71afa1c9cf04b49ad11db263be9e47d46f0f84ee68b625`  
		Last Modified: Sat, 26 Sep 2020 01:39:10 GMT  
		Size: 9.3 MB (9300101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
