<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:crystal`](#roscrystal)
-	[`ros:crystal-ros-base`](#roscrystal-ros-base)
-	[`ros:crystal-ros-base-bionic`](#roscrystal-ros-base-bionic)
-	[`ros:crystal-ros-core`](#roscrystal-ros-core)
-	[`ros:crystal-ros-core-bionic`](#roscrystal-ros-core-bionic)
-	[`ros:dashing`](#rosdashing)
-	[`ros:dashing-ros-base`](#rosdashing-ros-base)
-	[`ros:dashing-ros-base-bionic`](#rosdashing-ros-base-bionic)
-	[`ros:dashing-ros-core`](#rosdashing-ros-core)
-	[`ros:dashing-ros-core-bionic`](#rosdashing-ros-core-bionic)
-	[`ros:eloquent`](#roseloquent)
-	[`ros:eloquent-ros-base`](#roseloquent-ros-base)
-	[`ros:eloquent-ros-base-bionic`](#roseloquent-ros-base-bionic)
-	[`ros:eloquent-ros-core`](#roseloquent-ros-core)
-	[`ros:eloquent-ros-core-bionic`](#roseloquent-ros-core-bionic)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
-	[`ros:latest`](#roslatest)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-perception-stretch`](#rosmelodic-perception-stretch)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-robot-stretch`](#rosmelodic-robot-stretch)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-base-stretch`](#rosmelodic-ros-base-stretch)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:melodic-ros-core-stretch`](#rosmelodic-ros-core-stretch)

## `ros:crystal`

```console
$ docker pull ros@sha256:0489756a6abe52e43a55591a0164744c4b283b7cf8a2aa1a54d832541911d77b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal` - linux; amd64

```console
$ docker pull ros@sha256:95908051b3373824751a7572e5bb49aa5fe9a56d0eee5dab8fb57d60b6581dbe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262518950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1582267554cc0490cade13160c3b36762cdfa17e15305200280b150d9a89c9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 04:24:13 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 04:24:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:25:02 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 04:25:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:25:08 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:25:08 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 04:25:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:25:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:25:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:25:45 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:26:01 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9addf1d92b8503f1d25fa9267e42ab7180bb2777caaf9c0012d40c8ee4709b3`  
		Last Modified: Thu, 16 Jan 2020 04:34:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59f02d915cfe1f66ccc84d677760ae5d06b3e7f9b4658c50537734a770c9e1`  
		Last Modified: Thu, 16 Jan 2020 04:34:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94bdb8b5914c7efd28d519e3cc7a89d5aed63aac56042a6ce6a72a249da9932`  
		Last Modified: Thu, 16 Jan 2020 04:35:02 GMT  
		Size: 28.4 MB (28396659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4395f405c8de33864522ded020e7e8c15f2306d61db0518afd9d5a9797dce5`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 980.9 KB (980941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a008b9dc978318a542cc7bb8e4b1ecb1a210a9e4784fba66a596bacd0450abca`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577ccb31d5b0be22594cf02c438d11c0df69c4edf2e5a179de6289144d02831`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 327.0 KB (327016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76368d728bb05f7104060302eb46d3539d8699d85d7756ceb9101d1148d03ada`  
		Last Modified: Thu, 16 Jan 2020 04:35:12 GMT  
		Size: 50.1 MB (50058557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca3672fdd34cc3e06f786a7bf2d1708db4b71cf8be6df442f6a04901c1966f`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5a20f25974b8a29411bed746777f9bfbbde7b7994122e9bc8d52d10487f8d4`  
		Last Modified: Thu, 16 Jan 2020 04:35:29 GMT  
		Size: 3.2 MB (3179953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:03c1ff40d25f80dad1ba57409f2a4758b5be3fd6b1cbb4c4fc39072f89ca393a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238646637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f68bcf593c1288232d8bf8f5209e2e4891ae2c846a278c73e7333547afdd38`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 02:54:07 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 02:55:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:56:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:56:44 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 02:56:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 02:57:01 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 02:57:02 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 02:58:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:58:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 02:58:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:58:33 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:59:10 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262698059de5b26d03f503e4d2c8681bd2ec8a20d2b8e4fcb4ad8ba482e2dd6f`  
		Last Modified: Thu, 16 Jan 2020 03:20:37 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3200eb5fe400ffaaf7abf80518ebab5d81cb95e5796a4623e06c64942fa712`  
		Last Modified: Thu, 16 Jan 2020 03:20:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074c7fafffe2695ed2f6dca9a412161082222db32127f9c3d1abbffa319aaf6`  
		Last Modified: Thu, 16 Jan 2020 03:20:47 GMT  
		Size: 27.1 MB (27082494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee97e4e48108d71e1ff39e03788137536d35184e3f25fe846999e64cda9f`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 981.0 KB (980995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a4ec8ab3b5b5bd81e9c295b60ea6e28be24c0ec0cbcf8d7c0456cc7a66c7d`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 1.9 KB (1932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8e91593059fab4b1fede301b4a0227f94bb9f1ea2255c49b6466551715c1e`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 327.3 KB (327307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07ebfb58a0d1eecc608dd1aeba967ddd4ac282c615010d009555491eb5b3fc`  
		Last Modified: Thu, 16 Jan 2020 03:20:52 GMT  
		Size: 39.5 MB (39536035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f37338b010c9d89b1e2fd356e7b5ce2b5645fe5aa523424db0e7740460270`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed49e742e33a0461f9c79f98c1c0573465b8e35abb09f6a46eb8f198a8bd918`  
		Last Modified: Thu, 16 Jan 2020 03:21:23 GMT  
		Size: 2.9 MB (2942720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-base`

```console
$ docker pull ros@sha256:0489756a6abe52e43a55591a0164744c4b283b7cf8a2aa1a54d832541911d77b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:95908051b3373824751a7572e5bb49aa5fe9a56d0eee5dab8fb57d60b6581dbe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262518950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1582267554cc0490cade13160c3b36762cdfa17e15305200280b150d9a89c9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 04:24:13 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 04:24:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:25:02 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 04:25:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:25:08 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:25:08 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 04:25:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:25:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:25:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:25:45 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:26:01 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9addf1d92b8503f1d25fa9267e42ab7180bb2777caaf9c0012d40c8ee4709b3`  
		Last Modified: Thu, 16 Jan 2020 04:34:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59f02d915cfe1f66ccc84d677760ae5d06b3e7f9b4658c50537734a770c9e1`  
		Last Modified: Thu, 16 Jan 2020 04:34:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94bdb8b5914c7efd28d519e3cc7a89d5aed63aac56042a6ce6a72a249da9932`  
		Last Modified: Thu, 16 Jan 2020 04:35:02 GMT  
		Size: 28.4 MB (28396659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4395f405c8de33864522ded020e7e8c15f2306d61db0518afd9d5a9797dce5`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 980.9 KB (980941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a008b9dc978318a542cc7bb8e4b1ecb1a210a9e4784fba66a596bacd0450abca`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577ccb31d5b0be22594cf02c438d11c0df69c4edf2e5a179de6289144d02831`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 327.0 KB (327016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76368d728bb05f7104060302eb46d3539d8699d85d7756ceb9101d1148d03ada`  
		Last Modified: Thu, 16 Jan 2020 04:35:12 GMT  
		Size: 50.1 MB (50058557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca3672fdd34cc3e06f786a7bf2d1708db4b71cf8be6df442f6a04901c1966f`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5a20f25974b8a29411bed746777f9bfbbde7b7994122e9bc8d52d10487f8d4`  
		Last Modified: Thu, 16 Jan 2020 04:35:29 GMT  
		Size: 3.2 MB (3179953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:03c1ff40d25f80dad1ba57409f2a4758b5be3fd6b1cbb4c4fc39072f89ca393a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238646637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f68bcf593c1288232d8bf8f5209e2e4891ae2c846a278c73e7333547afdd38`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 02:54:07 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 02:55:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:56:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:56:44 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 02:56:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 02:57:01 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 02:57:02 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 02:58:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:58:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 02:58:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:58:33 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:59:10 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262698059de5b26d03f503e4d2c8681bd2ec8a20d2b8e4fcb4ad8ba482e2dd6f`  
		Last Modified: Thu, 16 Jan 2020 03:20:37 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3200eb5fe400ffaaf7abf80518ebab5d81cb95e5796a4623e06c64942fa712`  
		Last Modified: Thu, 16 Jan 2020 03:20:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074c7fafffe2695ed2f6dca9a412161082222db32127f9c3d1abbffa319aaf6`  
		Last Modified: Thu, 16 Jan 2020 03:20:47 GMT  
		Size: 27.1 MB (27082494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee97e4e48108d71e1ff39e03788137536d35184e3f25fe846999e64cda9f`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 981.0 KB (980995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a4ec8ab3b5b5bd81e9c295b60ea6e28be24c0ec0cbcf8d7c0456cc7a66c7d`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 1.9 KB (1932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8e91593059fab4b1fede301b4a0227f94bb9f1ea2255c49b6466551715c1e`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 327.3 KB (327307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07ebfb58a0d1eecc608dd1aeba967ddd4ac282c615010d009555491eb5b3fc`  
		Last Modified: Thu, 16 Jan 2020 03:20:52 GMT  
		Size: 39.5 MB (39536035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f37338b010c9d89b1e2fd356e7b5ce2b5645fe5aa523424db0e7740460270`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed49e742e33a0461f9c79f98c1c0573465b8e35abb09f6a46eb8f198a8bd918`  
		Last Modified: Thu, 16 Jan 2020 03:21:23 GMT  
		Size: 2.9 MB (2942720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-base-bionic`

```console
$ docker pull ros@sha256:0489756a6abe52e43a55591a0164744c4b283b7cf8a2aa1a54d832541911d77b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:95908051b3373824751a7572e5bb49aa5fe9a56d0eee5dab8fb57d60b6581dbe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262518950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1582267554cc0490cade13160c3b36762cdfa17e15305200280b150d9a89c9ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 04:24:13 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 04:24:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:25:02 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 04:25:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:25:08 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:25:08 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 04:25:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:25:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:25:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:25:45 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:26:01 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9addf1d92b8503f1d25fa9267e42ab7180bb2777caaf9c0012d40c8ee4709b3`  
		Last Modified: Thu, 16 Jan 2020 04:34:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59f02d915cfe1f66ccc84d677760ae5d06b3e7f9b4658c50537734a770c9e1`  
		Last Modified: Thu, 16 Jan 2020 04:34:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94bdb8b5914c7efd28d519e3cc7a89d5aed63aac56042a6ce6a72a249da9932`  
		Last Modified: Thu, 16 Jan 2020 04:35:02 GMT  
		Size: 28.4 MB (28396659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4395f405c8de33864522ded020e7e8c15f2306d61db0518afd9d5a9797dce5`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 980.9 KB (980941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a008b9dc978318a542cc7bb8e4b1ecb1a210a9e4784fba66a596bacd0450abca`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577ccb31d5b0be22594cf02c438d11c0df69c4edf2e5a179de6289144d02831`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 327.0 KB (327016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76368d728bb05f7104060302eb46d3539d8699d85d7756ceb9101d1148d03ada`  
		Last Modified: Thu, 16 Jan 2020 04:35:12 GMT  
		Size: 50.1 MB (50058557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca3672fdd34cc3e06f786a7bf2d1708db4b71cf8be6df442f6a04901c1966f`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5a20f25974b8a29411bed746777f9bfbbde7b7994122e9bc8d52d10487f8d4`  
		Last Modified: Thu, 16 Jan 2020 04:35:29 GMT  
		Size: 3.2 MB (3179953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:03c1ff40d25f80dad1ba57409f2a4758b5be3fd6b1cbb4c4fc39072f89ca393a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238646637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f68bcf593c1288232d8bf8f5209e2e4891ae2c846a278c73e7333547afdd38`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 02:54:07 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 02:55:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:56:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:56:44 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 02:56:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 02:57:01 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 02:57:02 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 02:58:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:58:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 02:58:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:58:33 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:59:10 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-base=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262698059de5b26d03f503e4d2c8681bd2ec8a20d2b8e4fcb4ad8ba482e2dd6f`  
		Last Modified: Thu, 16 Jan 2020 03:20:37 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3200eb5fe400ffaaf7abf80518ebab5d81cb95e5796a4623e06c64942fa712`  
		Last Modified: Thu, 16 Jan 2020 03:20:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074c7fafffe2695ed2f6dca9a412161082222db32127f9c3d1abbffa319aaf6`  
		Last Modified: Thu, 16 Jan 2020 03:20:47 GMT  
		Size: 27.1 MB (27082494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee97e4e48108d71e1ff39e03788137536d35184e3f25fe846999e64cda9f`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 981.0 KB (980995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a4ec8ab3b5b5bd81e9c295b60ea6e28be24c0ec0cbcf8d7c0456cc7a66c7d`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 1.9 KB (1932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8e91593059fab4b1fede301b4a0227f94bb9f1ea2255c49b6466551715c1e`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 327.3 KB (327307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07ebfb58a0d1eecc608dd1aeba967ddd4ac282c615010d009555491eb5b3fc`  
		Last Modified: Thu, 16 Jan 2020 03:20:52 GMT  
		Size: 39.5 MB (39536035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f37338b010c9d89b1e2fd356e7b5ce2b5645fe5aa523424db0e7740460270`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed49e742e33a0461f9c79f98c1c0573465b8e35abb09f6a46eb8f198a8bd918`  
		Last Modified: Thu, 16 Jan 2020 03:21:23 GMT  
		Size: 2.9 MB (2942720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-core`

```console
$ docker pull ros@sha256:a97e975aae886b4702f66763a7184370b1e792b29276797e0ceca9e3f3dcfb9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:38a528ddc76db36fed8a26d67267496bdeb9425eb7b0c239c39a4a286dedc2c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259338997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c020342ceadf023eb13e8b5a25c4b37ca7a87b9a8f27f693275870c6da5472ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 04:24:13 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 04:24:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:25:02 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 04:25:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:25:08 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:25:08 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 04:25:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:25:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:25:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:25:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9addf1d92b8503f1d25fa9267e42ab7180bb2777caaf9c0012d40c8ee4709b3`  
		Last Modified: Thu, 16 Jan 2020 04:34:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59f02d915cfe1f66ccc84d677760ae5d06b3e7f9b4658c50537734a770c9e1`  
		Last Modified: Thu, 16 Jan 2020 04:34:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94bdb8b5914c7efd28d519e3cc7a89d5aed63aac56042a6ce6a72a249da9932`  
		Last Modified: Thu, 16 Jan 2020 04:35:02 GMT  
		Size: 28.4 MB (28396659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4395f405c8de33864522ded020e7e8c15f2306d61db0518afd9d5a9797dce5`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 980.9 KB (980941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a008b9dc978318a542cc7bb8e4b1ecb1a210a9e4784fba66a596bacd0450abca`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577ccb31d5b0be22594cf02c438d11c0df69c4edf2e5a179de6289144d02831`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 327.0 KB (327016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76368d728bb05f7104060302eb46d3539d8699d85d7756ceb9101d1148d03ada`  
		Last Modified: Thu, 16 Jan 2020 04:35:12 GMT  
		Size: 50.1 MB (50058557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca3672fdd34cc3e06f786a7bf2d1708db4b71cf8be6df442f6a04901c1966f`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0916e4d5929c6a85f99fa5f061cba92f14c27d8edb717cd3dbbb767486f4d577
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235703917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cdf8f73e27ffe05ff4f515f08db0bce4c02f9050b2f845056a63e94cea8e314`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 02:54:07 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 02:55:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:56:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:56:44 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 02:56:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 02:57:01 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 02:57:02 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 02:58:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:58:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 02:58:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:58:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262698059de5b26d03f503e4d2c8681bd2ec8a20d2b8e4fcb4ad8ba482e2dd6f`  
		Last Modified: Thu, 16 Jan 2020 03:20:37 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3200eb5fe400ffaaf7abf80518ebab5d81cb95e5796a4623e06c64942fa712`  
		Last Modified: Thu, 16 Jan 2020 03:20:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074c7fafffe2695ed2f6dca9a412161082222db32127f9c3d1abbffa319aaf6`  
		Last Modified: Thu, 16 Jan 2020 03:20:47 GMT  
		Size: 27.1 MB (27082494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee97e4e48108d71e1ff39e03788137536d35184e3f25fe846999e64cda9f`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 981.0 KB (980995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a4ec8ab3b5b5bd81e9c295b60ea6e28be24c0ec0cbcf8d7c0456cc7a66c7d`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 1.9 KB (1932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8e91593059fab4b1fede301b4a0227f94bb9f1ea2255c49b6466551715c1e`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 327.3 KB (327307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07ebfb58a0d1eecc608dd1aeba967ddd4ac282c615010d009555491eb5b3fc`  
		Last Modified: Thu, 16 Jan 2020 03:20:52 GMT  
		Size: 39.5 MB (39536035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f37338b010c9d89b1e2fd356e7b5ce2b5645fe5aa523424db0e7740460270`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:crystal-ros-core-bionic`

```console
$ docker pull ros@sha256:a97e975aae886b4702f66763a7184370b1e792b29276797e0ceca9e3f3dcfb9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:crystal-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:38a528ddc76db36fed8a26d67267496bdeb9425eb7b0c239c39a4a286dedc2c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259338997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c020342ceadf023eb13e8b5a25c4b37ca7a87b9a8f27f693275870c6da5472ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 04:24:13 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 04:24:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:24:47 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:25:02 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 04:25:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:25:08 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:25:08 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 04:25:44 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:25:45 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:25:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:25:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9addf1d92b8503f1d25fa9267e42ab7180bb2777caaf9c0012d40c8ee4709b3`  
		Last Modified: Thu, 16 Jan 2020 04:34:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb59f02d915cfe1f66ccc84d677760ae5d06b3e7f9b4658c50537734a770c9e1`  
		Last Modified: Thu, 16 Jan 2020 04:34:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94bdb8b5914c7efd28d519e3cc7a89d5aed63aac56042a6ce6a72a249da9932`  
		Last Modified: Thu, 16 Jan 2020 04:35:02 GMT  
		Size: 28.4 MB (28396659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4395f405c8de33864522ded020e7e8c15f2306d61db0518afd9d5a9797dce5`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 980.9 KB (980941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a008b9dc978318a542cc7bb8e4b1ecb1a210a9e4784fba66a596bacd0450abca`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577ccb31d5b0be22594cf02c438d11c0df69c4edf2e5a179de6289144d02831`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 327.0 KB (327016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76368d728bb05f7104060302eb46d3539d8699d85d7756ceb9101d1148d03ada`  
		Last Modified: Thu, 16 Jan 2020 04:35:12 GMT  
		Size: 50.1 MB (50058557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca3672fdd34cc3e06f786a7bf2d1708db4b71cf8be6df442f6a04901c1966f`  
		Last Modified: Thu, 16 Jan 2020 04:34:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:crystal-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0916e4d5929c6a85f99fa5f061cba92f14c27d8edb717cd3dbbb767486f4d577
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235703917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cdf8f73e27ffe05ff4f515f08db0bce4c02f9050b2f845056a63e94cea8e314`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 16 Jan 2020 02:54:07 GMT
RUN echo "deb http://snapshots.ros.org/crystal/final/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 16 Jan 2020 02:55:51 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:55:57 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:56:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:56:44 GMT
RUN rosdep init     && rosdep update --include-eol-distros
# Thu, 16 Jan 2020 02:56:55 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 02:57:01 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 02:57:02 GMT
ENV ROS_DISTRO=crystal
# Thu, 16 Jan 2020 02:58:26 GMT
RUN apt-get update && apt-get install -y     ros-crystal-ros-core=0.6.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:58:31 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 02:58:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:58:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262698059de5b26d03f503e4d2c8681bd2ec8a20d2b8e4fcb4ad8ba482e2dd6f`  
		Last Modified: Thu, 16 Jan 2020 03:20:37 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3200eb5fe400ffaaf7abf80518ebab5d81cb95e5796a4623e06c64942fa712`  
		Last Modified: Thu, 16 Jan 2020 03:20:36 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9074c7fafffe2695ed2f6dca9a412161082222db32127f9c3d1abbffa319aaf6`  
		Last Modified: Thu, 16 Jan 2020 03:20:47 GMT  
		Size: 27.1 MB (27082494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3aee97e4e48108d71e1ff39e03788137536d35184e3f25fe846999e64cda9f`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 981.0 KB (980995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a4ec8ab3b5b5bd81e9c295b60ea6e28be24c0ec0cbcf8d7c0456cc7a66c7d`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 1.9 KB (1932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8e91593059fab4b1fede301b4a0227f94bb9f1ea2255c49b6466551715c1e`  
		Last Modified: Thu, 16 Jan 2020 03:20:34 GMT  
		Size: 327.3 KB (327307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d07ebfb58a0d1eecc608dd1aeba967ddd4ac282c615010d009555491eb5b3fc`  
		Last Modified: Thu, 16 Jan 2020 03:20:52 GMT  
		Size: 39.5 MB (39536035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f37338b010c9d89b1e2fd356e7b5ce2b5645fe5aa523424db0e7740460270`  
		Last Modified: Thu, 16 Jan 2020 03:20:33 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing`

```console
$ docker pull ros@sha256:b357186970fc13864c4892b451734aa9acfc890e66d9e817f6441b85f1cd1d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing` - linux; amd64

```console
$ docker pull ros@sha256:0bd7b270fe8e014d811b929887e892418a2575f0f3a929b27651db09aefeb111
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281147821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7211a06555f6a509e52c0425c2393cbfce5e2d3c6982aab446d0cfa0d7a55b94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:26:45 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 04:27:23 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:27:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:27:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:27:24 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:27:42 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b06fc78bb1a7619588ec20b904f6bcb7cde5310456fe3ccf489ed7c18fbc40`  
		Last Modified: Thu, 16 Jan 2020 04:35:58 GMT  
		Size: 68.1 MB (68085760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b974d53d11b0a5797da673f187a1c4a901cc1864e4d30d20338a34d99ef0c`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b06270edcbf4e3149ed9d24834cc5750f2031734e449f95dbd8883c8d6dbd6e`  
		Last Modified: Thu, 16 Jan 2020 04:36:09 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm variant v7

```console
$ docker pull ros@sha256:b36dc6fe429ecbea8d4671d9b7de218520a9076955d312d4c9b597f0cf0cf01a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.4 MB (235374158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cfbadddff55f84b45c41bee21e4b8bd2581ecbf080ac6758c05312213f7a40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:12:48 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:14:44 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:14:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:14:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:14:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:15:27 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e955036ba0d39235062d7a8018f72c1ea0ba80897662b0e923abcdd472b620f5`  
		Last Modified: Thu, 16 Jan 2020 03:26:58 GMT  
		Size: 49.3 MB (49262089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe2e51c51328a1ef21dbba0a5ac08c333556f85c79646c6d349cc71da603cb`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528e777c5b38ff5e7b5a4b9e22f924c069b952a9631e4a4f06fd6e5a2b11f6d`  
		Last Modified: Thu, 16 Jan 2020 03:27:20 GMT  
		Size: 3.3 MB (3278403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:da4d6e5a2d0db784606e58a213d2041f5c0cf0449ad0a1670bb200170bee83c8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.9 MB (254863737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5776112d86aff0c727d5c27508835578a21f3a9403d0c9e87e8d2dec400e41d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:02:36 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:06:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:07:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:07:06 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:07:54 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a14961574783cff8a9199cba06c4a4138c094ba97299bc01407a7435d936626`  
		Last Modified: Thu, 16 Jan 2020 03:21:53 GMT  
		Size: 55.6 MB (55560242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b3b97300169f54c95c1c0abe10c6978b18c174ee2a9afe2fd13859901f0907`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af62bc0678a5d480aaf07725232b9be410672eb01032c5da63b1d2365957cd3`  
		Last Modified: Thu, 16 Jan 2020 03:22:03 GMT  
		Size: 3.7 MB (3693098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base`

```console
$ docker pull ros@sha256:b357186970fc13864c4892b451734aa9acfc890e66d9e817f6441b85f1cd1d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:0bd7b270fe8e014d811b929887e892418a2575f0f3a929b27651db09aefeb111
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281147821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7211a06555f6a509e52c0425c2393cbfce5e2d3c6982aab446d0cfa0d7a55b94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:26:45 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 04:27:23 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:27:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:27:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:27:24 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:27:42 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b06fc78bb1a7619588ec20b904f6bcb7cde5310456fe3ccf489ed7c18fbc40`  
		Last Modified: Thu, 16 Jan 2020 04:35:58 GMT  
		Size: 68.1 MB (68085760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b974d53d11b0a5797da673f187a1c4a901cc1864e4d30d20338a34d99ef0c`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b06270edcbf4e3149ed9d24834cc5750f2031734e449f95dbd8883c8d6dbd6e`  
		Last Modified: Thu, 16 Jan 2020 04:36:09 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:b36dc6fe429ecbea8d4671d9b7de218520a9076955d312d4c9b597f0cf0cf01a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.4 MB (235374158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cfbadddff55f84b45c41bee21e4b8bd2581ecbf080ac6758c05312213f7a40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:12:48 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:14:44 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:14:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:14:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:14:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:15:27 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e955036ba0d39235062d7a8018f72c1ea0ba80897662b0e923abcdd472b620f5`  
		Last Modified: Thu, 16 Jan 2020 03:26:58 GMT  
		Size: 49.3 MB (49262089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe2e51c51328a1ef21dbba0a5ac08c333556f85c79646c6d349cc71da603cb`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528e777c5b38ff5e7b5a4b9e22f924c069b952a9631e4a4f06fd6e5a2b11f6d`  
		Last Modified: Thu, 16 Jan 2020 03:27:20 GMT  
		Size: 3.3 MB (3278403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:da4d6e5a2d0db784606e58a213d2041f5c0cf0449ad0a1670bb200170bee83c8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.9 MB (254863737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5776112d86aff0c727d5c27508835578a21f3a9403d0c9e87e8d2dec400e41d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:02:36 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:06:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:07:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:07:06 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:07:54 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a14961574783cff8a9199cba06c4a4138c094ba97299bc01407a7435d936626`  
		Last Modified: Thu, 16 Jan 2020 03:21:53 GMT  
		Size: 55.6 MB (55560242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b3b97300169f54c95c1c0abe10c6978b18c174ee2a9afe2fd13859901f0907`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af62bc0678a5d480aaf07725232b9be410672eb01032c5da63b1d2365957cd3`  
		Last Modified: Thu, 16 Jan 2020 03:22:03 GMT  
		Size: 3.7 MB (3693098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-base-bionic`

```console
$ docker pull ros@sha256:b357186970fc13864c4892b451734aa9acfc890e66d9e817f6441b85f1cd1d77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:0bd7b270fe8e014d811b929887e892418a2575f0f3a929b27651db09aefeb111
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281147821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7211a06555f6a509e52c0425c2393cbfce5e2d3c6982aab446d0cfa0d7a55b94`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:26:45 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 04:27:23 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:27:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:27:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:27:24 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:27:42 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b06fc78bb1a7619588ec20b904f6bcb7cde5310456fe3ccf489ed7c18fbc40`  
		Last Modified: Thu, 16 Jan 2020 04:35:58 GMT  
		Size: 68.1 MB (68085760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b974d53d11b0a5797da673f187a1c4a901cc1864e4d30d20338a34d99ef0c`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b06270edcbf4e3149ed9d24834cc5750f2031734e449f95dbd8883c8d6dbd6e`  
		Last Modified: Thu, 16 Jan 2020 04:36:09 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:b36dc6fe429ecbea8d4671d9b7de218520a9076955d312d4c9b597f0cf0cf01a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.4 MB (235374158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77cfbadddff55f84b45c41bee21e4b8bd2581ecbf080ac6758c05312213f7a40`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:12:48 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:14:44 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:14:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:14:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:14:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:15:27 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e955036ba0d39235062d7a8018f72c1ea0ba80897662b0e923abcdd472b620f5`  
		Last Modified: Thu, 16 Jan 2020 03:26:58 GMT  
		Size: 49.3 MB (49262089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe2e51c51328a1ef21dbba0a5ac08c333556f85c79646c6d349cc71da603cb`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7528e777c5b38ff5e7b5a4b9e22f924c069b952a9631e4a4f06fd6e5a2b11f6d`  
		Last Modified: Thu, 16 Jan 2020 03:27:20 GMT  
		Size: 3.3 MB (3278403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:da4d6e5a2d0db784606e58a213d2041f5c0cf0449ad0a1670bb200170bee83c8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.9 MB (254863737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5776112d86aff0c727d5c27508835578a21f3a9403d0c9e87e8d2dec400e41d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:02:36 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:06:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:07:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:07:06 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:07:54 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-base=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a14961574783cff8a9199cba06c4a4138c094ba97299bc01407a7435d936626`  
		Last Modified: Thu, 16 Jan 2020 03:21:53 GMT  
		Size: 55.6 MB (55560242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b3b97300169f54c95c1c0abe10c6978b18c174ee2a9afe2fd13859901f0907`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af62bc0678a5d480aaf07725232b9be410672eb01032c5da63b1d2365957cd3`  
		Last Modified: Thu, 16 Jan 2020 03:22:03 GMT  
		Size: 3.7 MB (3693098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core`

```console
$ docker pull ros@sha256:f2ef14e81bf41c9339a95ca4557ec445c530c14b8ea9ed668613c5857a2c3af0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:6c274db76976e2163022cc68ec9f10a9dd3a55cfef69b30a7d01fe2f53ab9836
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.8 MB (276807605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2b386bf9ae4d439a4de9f78e0e236a31b6190f5ca566e55430cec0b35ead432`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:26:45 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 04:27:23 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:27:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:27:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:27:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b06fc78bb1a7619588ec20b904f6bcb7cde5310456fe3ccf489ed7c18fbc40`  
		Last Modified: Thu, 16 Jan 2020 04:35:58 GMT  
		Size: 68.1 MB (68085760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b974d53d11b0a5797da673f187a1c4a901cc1864e4d30d20338a34d99ef0c`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5ecd10e82e1fdb22479ca774d76740f58a23a10555e38efc179e474279a39718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232095755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d10b59ab958f2aa84a84cb181e23fbeffc861d6e64703870acc5388ff5a4a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:12:48 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:14:44 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:14:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:14:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e955036ba0d39235062d7a8018f72c1ea0ba80897662b0e923abcdd472b620f5`  
		Last Modified: Thu, 16 Jan 2020 03:26:58 GMT  
		Size: 49.3 MB (49262089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe2e51c51328a1ef21dbba0a5ac08c333556f85c79646c6d349cc71da603cb`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:132c8befbe3833135711af4619d2497cef3e2fbf20f3acebd608a56a89debe75
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251170639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08dd27e2e378c30e42792fd7bdbd981ef258670affa1c907faa1e29f57bab91d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:02:36 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:06:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:07:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:07:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a14961574783cff8a9199cba06c4a4138c094ba97299bc01407a7435d936626`  
		Last Modified: Thu, 16 Jan 2020 03:21:53 GMT  
		Size: 55.6 MB (55560242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b3b97300169f54c95c1c0abe10c6978b18c174ee2a9afe2fd13859901f0907`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:dashing-ros-core-bionic`

```console
$ docker pull ros@sha256:f2ef14e81bf41c9339a95ca4557ec445c530c14b8ea9ed668613c5857a2c3af0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:dashing-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6c274db76976e2163022cc68ec9f10a9dd3a55cfef69b30a7d01fe2f53ab9836
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.8 MB (276807605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2b386bf9ae4d439a4de9f78e0e236a31b6190f5ca566e55430cec0b35ead432`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:26:45 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 04:27:23 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:27:23 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:27:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:27:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b06fc78bb1a7619588ec20b904f6bcb7cde5310456fe3ccf489ed7c18fbc40`  
		Last Modified: Thu, 16 Jan 2020 04:35:58 GMT  
		Size: 68.1 MB (68085760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b974d53d11b0a5797da673f187a1c4a901cc1864e4d30d20338a34d99ef0c`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:5ecd10e82e1fdb22479ca774d76740f58a23a10555e38efc179e474279a39718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232095755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d10b59ab958f2aa84a84cb181e23fbeffc861d6e64703870acc5388ff5a4a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:12:48 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:14:44 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:14:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:14:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e955036ba0d39235062d7a8018f72c1ea0ba80897662b0e923abcdd472b620f5`  
		Last Modified: Thu, 16 Jan 2020 03:26:58 GMT  
		Size: 49.3 MB (49262089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe2e51c51328a1ef21dbba0a5ac08c333556f85c79646c6d349cc71da603cb`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:dashing-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:132c8befbe3833135711af4619d2497cef3e2fbf20f3acebd608a56a89debe75
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251170639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08dd27e2e378c30e42792fd7bdbd981ef258670affa1c907faa1e29f57bab91d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:02:36 GMT
ENV ROS_DISTRO=dashing
# Thu, 16 Jan 2020 03:06:46 GMT
RUN apt-get update && apt-get install -y     ros-dashing-ros-core=0.7.3-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:07:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:07:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a14961574783cff8a9199cba06c4a4138c094ba97299bc01407a7435d936626`  
		Last Modified: Thu, 16 Jan 2020 03:21:53 GMT  
		Size: 55.6 MB (55560242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b3b97300169f54c95c1c0abe10c6978b18c174ee2a9afe2fd13859901f0907`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent`

```console
$ docker pull ros@sha256:38e31f05534bba79981d6f3c737c14a4d4609849236efc1a046e866f9e046b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:4d1c8c6e43052d8b5b2a19edc2b529d8516751aa207b27e6aaac045ff6d9bec7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.6 MB (283618004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ecd87ff213b37e8573826b7b3240a0902a6b57ff36675317f1fda6426dc8e57`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:28:40 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f54fa04cfa49ffe305cc98e22817e1d7e10c1d05de2bad7b30572b4c15fb559`  
		Last Modified: Thu, 16 Jan 2020 04:36:42 GMT  
		Size: 4.6 MB (4602192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm variant v7

```console
$ docker pull ros@sha256:af5c6862560a6933f018782114cb4ee51e36aec944444a7a89a5ec1966e26401
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237374716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62fe72b79d428c35d38291ea5ae7e7e3b0948f2530d6dac327d350b25c96788b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:18:06 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055227d75c97e401b955db9ea1a4d784bf04b1926af6a84f351586a9b3a935f5`  
		Last Modified: Thu, 16 Jan 2020 03:27:59 GMT  
		Size: 3.5 MB (3516872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:94237ca5406272645d192a40267979829d49b6460a9ebf9ae72ad6fbdf55ac83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257155305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0887f74845992d30957ff8706f1f8def1a9003e796f444350c68bf45a36c76`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:11:37 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620498a630739d39314cb08eae34f29a33dd1e0b06483582035c8072e3fec4c9`  
		Last Modified: Thu, 16 Jan 2020 03:22:42 GMT  
		Size: 4.0 MB (3954504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base`

```console
$ docker pull ros@sha256:38e31f05534bba79981d6f3c737c14a4d4609849236efc1a046e866f9e046b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:4d1c8c6e43052d8b5b2a19edc2b529d8516751aa207b27e6aaac045ff6d9bec7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.6 MB (283618004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ecd87ff213b37e8573826b7b3240a0902a6b57ff36675317f1fda6426dc8e57`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:28:40 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f54fa04cfa49ffe305cc98e22817e1d7e10c1d05de2bad7b30572b4c15fb559`  
		Last Modified: Thu, 16 Jan 2020 04:36:42 GMT  
		Size: 4.6 MB (4602192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:af5c6862560a6933f018782114cb4ee51e36aec944444a7a89a5ec1966e26401
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237374716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62fe72b79d428c35d38291ea5ae7e7e3b0948f2530d6dac327d350b25c96788b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:18:06 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055227d75c97e401b955db9ea1a4d784bf04b1926af6a84f351586a9b3a935f5`  
		Last Modified: Thu, 16 Jan 2020 03:27:59 GMT  
		Size: 3.5 MB (3516872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:94237ca5406272645d192a40267979829d49b6460a9ebf9ae72ad6fbdf55ac83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257155305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0887f74845992d30957ff8706f1f8def1a9003e796f444350c68bf45a36c76`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:11:37 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620498a630739d39314cb08eae34f29a33dd1e0b06483582035c8072e3fec4c9`  
		Last Modified: Thu, 16 Jan 2020 03:22:42 GMT  
		Size: 4.0 MB (3954504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-base-bionic`

```console
$ docker pull ros@sha256:38e31f05534bba79981d6f3c737c14a4d4609849236efc1a046e866f9e046b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:4d1c8c6e43052d8b5b2a19edc2b529d8516751aa207b27e6aaac045ff6d9bec7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.6 MB (283618004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ecd87ff213b37e8573826b7b3240a0902a6b57ff36675317f1fda6426dc8e57`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:28:40 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f54fa04cfa49ffe305cc98e22817e1d7e10c1d05de2bad7b30572b4c15fb559`  
		Last Modified: Thu, 16 Jan 2020 04:36:42 GMT  
		Size: 4.6 MB (4602192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:af5c6862560a6933f018782114cb4ee51e36aec944444a7a89a5ec1966e26401
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.4 MB (237374716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62fe72b79d428c35d38291ea5ae7e7e3b0948f2530d6dac327d350b25c96788b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:18:06 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055227d75c97e401b955db9ea1a4d784bf04b1926af6a84f351586a9b3a935f5`  
		Last Modified: Thu, 16 Jan 2020 03:27:59 GMT  
		Size: 3.5 MB (3516872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:94237ca5406272645d192a40267979829d49b6460a9ebf9ae72ad6fbdf55ac83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257155305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0887f74845992d30957ff8706f1f8def1a9003e796f444350c68bf45a36c76`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 03:11:37 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-base=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620498a630739d39314cb08eae34f29a33dd1e0b06483582035c8072e3fec4c9`  
		Last Modified: Thu, 16 Jan 2020 03:22:42 GMT  
		Size: 4.0 MB (3954504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core`

```console
$ docker pull ros@sha256:064b06183635793dd274a48b10830c3868b3c803d2175c3b50f286f035d0a156
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:95136060df4720bde9423146376e7178323678c48249b7f776ba02c54a56d86a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.0 MB (279015812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af943ae3ff67f7f15b0b2a00e2c38f013bcdd7819ef2569d4b6dedfa0155fa96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:f363ac5e07864d2718f3c3593457c86057dc911abbf5344e2285a7d62a9d8e82
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233857844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46f5fe0f5937732e1b27683b59bd8000a47a40f9a2725af8e46c87664c48c04`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4cb892e9fe42a19bf7f57a67a07bbb7e80ffc2bef01224bd82fa8b8b3aa1504
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253200801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c17a04bbe3cfb3be9723d42d21c794694e498516b89ab047242ff0666c00006`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:eloquent-ros-core-bionic`

```console
$ docker pull ros@sha256:064b06183635793dd274a48b10830c3868b3c803d2175c3b50f286f035d0a156
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:95136060df4720bde9423146376e7178323678c48249b7f776ba02c54a56d86a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.0 MB (279015812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af943ae3ff67f7f15b0b2a00e2c38f013bcdd7819ef2569d4b6dedfa0155fa96`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:24:10 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:26:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 04:26:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:26:32 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:26:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:26:40 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:26:43 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 04:26:45 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 04:27:47 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 04:28:26 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:28:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 04:28:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:28:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47860fbfee20faf985017137b1a207d6305a6f0e383f6e3eee136cf1213111ef`  
		Last Modified: Thu, 16 Jan 2020 04:35:21 GMT  
		Size: 152.0 MB (152007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739500682cbb0ffc4115ca90da07f225f6b5872465712241672f2a7f2ad1b6e1`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6510e8c430177f44918b440434795fd37f83cbb08eb16f3ac32f90338e3ccb34`  
		Last Modified: Thu, 16 Jan 2020 04:35:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a73d1eda1d5a5e90ccfe716e85be3f88210d3b6926cb9ddb76dfbef8a5410f`  
		Last Modified: Thu, 16 Jan 2020 04:35:43 GMT  
		Size: 28.4 MB (28400883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154aadde3bc6886f4ae1cd0478e12f15430ece84dd0be057a356250c83ec9bd`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 418.7 KB (418733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a98a41ae0e9c930de9e11baf6e18df13233215d9c2d8b3d26140f4c3298502b`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9998fabedb931db5162a69b65d36c0214dcc243d770e7dbc69a845786aad3c8`  
		Last Modified: Thu, 16 Jan 2020 04:35:34 GMT  
		Size: 327.0 KB (327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42965efca798c9c9e706ab5922070f5654bcf4608d5190162edaac6d567628`  
		Last Modified: Thu, 16 Jan 2020 04:36:36 GMT  
		Size: 70.3 MB (70293967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea24eb1ad310cafced566a0eccc94ad52e979fa2bb226cc7897080d02ce0da2`  
		Last Modified: Thu, 16 Jan 2020 04:36:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f363ac5e07864d2718f3c3593457c86057dc911abbf5344e2285a7d62a9d8e82
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233857844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46f5fe0f5937732e1b27683b59bd8000a47a40f9a2725af8e46c87664c48c04`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:39 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:09:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 03:09:53 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:12:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:12:14 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:12:15 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:12:30 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:12:36 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:12:42 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:15:34 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:17:25 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:17:29 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:17:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:17:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0f5560e852f7f56a00d07625adee98a2f42e1ab2b799e2ba9076be6f89444`  
		Last Modified: Thu, 16 Jan 2020 03:27:11 GMT  
		Size: 133.6 MB (133562427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78305fe242b5e016bcbdfaab268baaae05af6aefe35cda26d70b3fbf9e01082`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642a504f83ae9eff77dd98951ec05c3bf83c39734b13307680dd477e4495aa1`  
		Last Modified: Thu, 16 Jan 2020 03:26:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab34c54fcf37b9c6c928147391084e06be9c50c98364c2d18627ebcdeb628a82`  
		Last Modified: Thu, 16 Jan 2020 03:26:45 GMT  
		Size: 25.4 MB (25371604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260d22681f1fd118397473071bc4ce97fcabccc30f0c832c1e53bd16cf3b2ac6`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 418.8 KB (418810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a6eb7a2755d8f67f86b2526d328c0cd9096589052358e3e614bde9b3d1c78e`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 1.9 KB (1907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9b65605aa5f53341ef81cf09ef3191ff6f7b3bd1d1e228fdf138c437f62e8`  
		Last Modified: Thu, 16 Jan 2020 03:26:33 GMT  
		Size: 327.3 KB (327329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb05985b74964e9342cf7fea3660f7e829e196207602285054d94dbd52551db`  
		Last Modified: Thu, 16 Jan 2020 03:27:50 GMT  
		Size: 51.0 MB (51024178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfd7e9391f9003e2d47d56afbb32806f06263d0d3957ccfeefb70ca2644d0c3`  
		Last Modified: Thu, 16 Jan 2020 03:27:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e4cb892e9fe42a19bf7f57a67a07bbb7e80ffc2bef01224bd82fa8b8b3aa1504
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253200801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c17a04bbe3cfb3be9723d42d21c794694e498516b89ab047242ff0666c00006`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:54:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     python3-pip     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:59:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:59:22 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 16 Jan 2020 03:01:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:01:33 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 03:01:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 03:02:06 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 03:02:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 16 Jan 2020 03:02:31 GMT
RUN pip3 install -U     argcomplete
# Thu, 16 Jan 2020 03:08:05 GMT
ENV ROS_DISTRO=eloquent
# Thu, 16 Jan 2020 03:10:24 GMT
RUN apt-get update && apt-get install -y     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:10:38 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 16 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 03:10:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586861d850e94d19a4f09524ad8b6debd8243983f5d306baf682760570722b`  
		Last Modified: Thu, 16 Jan 2020 03:21:15 GMT  
		Size: 143.2 MB (143179290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552c6d8052085ae3899ec9adbacfff2bfcaac77e95ccfc4b4dc7425cf290b20e`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ad6f0b852d14b50179905ec18a230c20f95bc90533daccde3e86ea5a37fda`  
		Last Modified: Thu, 16 Jan 2020 03:21:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fdd3813347eba37cfccbffb4655a0cf0baee8b7733dce725b3c843beaec6ce`  
		Last Modified: Thu, 16 Jan 2020 03:21:41 GMT  
		Size: 27.1 MB (27087735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92288e9e0112e1d58483bbe59270b3d072c83ec5ba073ee1cc8c313f27eac85f`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 418.8 KB (418813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991ae3725db52c36fedba586155a2df9d44ca823d46cdf7fe023b50432a0025`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 1.9 KB (1931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64069bbf592deb57b4720e5f3eb1574afda76d5f9a8b6556faeaa68e78944e7`  
		Last Modified: Thu, 16 Jan 2020 03:21:30 GMT  
		Size: 327.3 KB (327347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191819737b8386a2ca9385a20290b92b7398c773d5b1a91f628aec3b30d3dad`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 57.6 MB (57590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218ac6d7be7b32161e12523997260627c3539594bf84bbd785783e640c63aac6`  
		Last Modified: Thu, 16 Jan 2020 03:22:10 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:0430be68be9b61d1c2e03e28bf05fa1dd3694c7af1280f770270a6998ee20715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:786f0dc7c99e43715d26bc25e5dab52bd531eba68d5967649e59046a495e4194
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385371235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2ec0c3ff726c74aab3ce1f145b2b0f62fe9e875067d01bf8bb2ae860be75537`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3cccddc753c46115fdfa6cbe096c6007359ae0294378c900ee842b7e8d76ee4a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336609302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513334779facbcff9db0b4a3aed5fcd78395e92bb17ec906f339f21bcd898eed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:61adb8691477fa8b98139d0377cc569bd2ed042514de666a4b183afb2ff2b409
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350419138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77107989faa08df0c4a6f0882b85d6ee3689c92364bb55a6d008612739e2c16f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:8230f241170322bf548761417eb700524b1facd4f0e9848dd2c6af3c4cc34b4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:bcf983a0a0a934b67b14d7a9ca586d31f2a070059e0c3241233c48a05cf6e728
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725780011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b48aecb4dc5eed4d9dff47229949a91b7f444b5b0ac85814e77e30e16314914`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:28 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580331cb7fff8bf72f628ba76e17656f071ecbe6d26254aed9f052931e2aec4c`  
		Last Modified: Thu, 16 Jan 2020 04:31:53 GMT  
		Size: 340.4 MB (340408776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:1b9658312983761fbf685ee9ee5cd0777d3453027dcdb45bc2932e729a16c851
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.1 MB (617119300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83936009b0b20af566033a891d7f527c3bd6d22a966ea43d645f94072bd814a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:45:33 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb435f169eacecc640515489d5893ff82333b27c13460d216602cb61fc265785`  
		Last Modified: Thu, 16 Jan 2020 03:22:23 GMT  
		Size: 280.5 MB (280509998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:efa6a0ae13cb69d75e81ad726a9f70bb0afc8135f509ddce0748580b2bcc660b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641377198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6c240e950e47d709da18d91504b85fd12e980afd3c7c5b3616db0473102330`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe216118715188ef41dd0042da40ce57ed6dbd6c59af91372d10a0b93c7fa5e0`  
		Last Modified: Thu, 16 Jan 2020 03:16:20 GMT  
		Size: 291.0 MB (290958060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:8230f241170322bf548761417eb700524b1facd4f0e9848dd2c6af3c4cc34b4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:bcf983a0a0a934b67b14d7a9ca586d31f2a070059e0c3241233c48a05cf6e728
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.8 MB (725780011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b48aecb4dc5eed4d9dff47229949a91b7f444b5b0ac85814e77e30e16314914`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:28 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580331cb7fff8bf72f628ba76e17656f071ecbe6d26254aed9f052931e2aec4c`  
		Last Modified: Thu, 16 Jan 2020 04:31:53 GMT  
		Size: 340.4 MB (340408776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:1b9658312983761fbf685ee9ee5cd0777d3453027dcdb45bc2932e729a16c851
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **617.1 MB (617119300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83936009b0b20af566033a891d7f527c3bd6d22a966ea43d645f94072bd814a4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:45:33 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb435f169eacecc640515489d5893ff82333b27c13460d216602cb61fc265785`  
		Last Modified: Thu, 16 Jan 2020 03:22:23 GMT  
		Size: 280.5 MB (280509998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:efa6a0ae13cb69d75e81ad726a9f70bb0afc8135f509ddce0748580b2bcc660b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.4 MB (641377198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6c240e950e47d709da18d91504b85fd12e980afd3c7c5b3616db0473102330`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:09 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe216118715188ef41dd0042da40ce57ed6dbd6c59af91372d10a0b93c7fa5e0`  
		Last Modified: Thu, 16 Jan 2020 03:16:20 GMT  
		Size: 291.0 MB (290958060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:1cfc6af66c45c821087cbc56b89962057a311b70abc86d4abafbe819f5cae2d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:aeb878759cd8513e13b55e0987d12fba45ab4622842038ff3e822aa80274f390
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.0 MB (489024041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fd92e3c1998ec26f18e6d3ca34b4adf47464155793a6726fa23b9270e1f323`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:07:18 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c761300cab8a90b7ebc084b6dee93b93f927af24c227bb92af16edf7cb32a8`  
		Last Modified: Thu, 16 Jan 2020 04:30:33 GMT  
		Size: 103.7 MB (103652806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:32a305cd791c38a6c6545c2d22bfb215b76b706fda39c808146388fd64606718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.7 MB (426655320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5951fea8748334e3f5e7d4445ec78f9f331aabff9fbcdb29bf2762d54e3905aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7056fc6a65ff0be249b5b431373216ab3c56f093a44e71ea4b777fe8a0ad8583`  
		Last Modified: Thu, 16 Jan 2020 03:20:42 GMT  
		Size: 90.0 MB (90046018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:178e5f46bce070516b8a6fda38e25dc1167370955b1b791d306c36868a819453
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.4 MB (444367483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db9883023c4423d6456abdc0a9222ea6fd9aa6477e2c210db912744c3ee59ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:25:42 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd09aab0d694744054ece4ceb50db6d1aa2641ad79ce63e402298fa0344b08`  
		Last Modified: Thu, 16 Jan 2020 03:14:34 GMT  
		Size: 93.9 MB (93948345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:1cfc6af66c45c821087cbc56b89962057a311b70abc86d4abafbe819f5cae2d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:aeb878759cd8513e13b55e0987d12fba45ab4622842038ff3e822aa80274f390
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.0 MB (489024041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fd92e3c1998ec26f18e6d3ca34b4adf47464155793a6726fa23b9270e1f323`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:07:18 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c761300cab8a90b7ebc084b6dee93b93f927af24c227bb92af16edf7cb32a8`  
		Last Modified: Thu, 16 Jan 2020 04:30:33 GMT  
		Size: 103.7 MB (103652806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:32a305cd791c38a6c6545c2d22bfb215b76b706fda39c808146388fd64606718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.7 MB (426655320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5951fea8748334e3f5e7d4445ec78f9f331aabff9fbcdb29bf2762d54e3905aa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:48 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7056fc6a65ff0be249b5b431373216ab3c56f093a44e71ea4b777fe8a0ad8583`  
		Last Modified: Thu, 16 Jan 2020 03:20:42 GMT  
		Size: 90.0 MB (90046018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:178e5f46bce070516b8a6fda38e25dc1167370955b1b791d306c36868a819453
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.4 MB (444367483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db9883023c4423d6456abdc0a9222ea6fd9aa6477e2c210db912744c3ee59ec`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:25:42 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdd09aab0d694744054ece4ceb50db6d1aa2641ad79ce63e402298fa0344b08`  
		Last Modified: Thu, 16 Jan 2020 03:14:34 GMT  
		Size: 93.9 MB (93948345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:0430be68be9b61d1c2e03e28bf05fa1dd3694c7af1280f770270a6998ee20715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:786f0dc7c99e43715d26bc25e5dab52bd531eba68d5967649e59046a495e4194
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385371235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2ec0c3ff726c74aab3ce1f145b2b0f62fe9e875067d01bf8bb2ae860be75537`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:3cccddc753c46115fdfa6cbe096c6007359ae0294378c900ee842b7e8d76ee4a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336609302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513334779facbcff9db0b4a3aed5fcd78395e92bb17ec906f339f21bcd898eed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:61adb8691477fa8b98139d0377cc569bd2ed042514de666a4b183afb2ff2b409
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350419138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77107989faa08df0c4a6f0882b85d6ee3689c92364bb55a6d008612739e2c16f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:0430be68be9b61d1c2e03e28bf05fa1dd3694c7af1280f770270a6998ee20715
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:786f0dc7c99e43715d26bc25e5dab52bd531eba68d5967649e59046a495e4194
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385371235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2ec0c3ff726c74aab3ce1f145b2b0f62fe9e875067d01bf8bb2ae860be75537`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:05:26 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a5e8549d86e70d3ef8ef7574bf1dc57e41604d836f288001338d4162d6d03`  
		Last Modified: Thu, 16 Jan 2020 04:30:04 GMT  
		Size: 85.5 MB (85524136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3cccddc753c46115fdfa6cbe096c6007359ae0294378c900ee842b7e8d76ee4a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336609302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513334779facbcff9db0b4a3aed5fcd78395e92bb17ec906f339f21bcd898eed`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a046a80c8e1698972206899f3517c1b14b083ba91d012a69b98b1d496830b26`  
		Last Modified: Thu, 16 Jan 2020 03:20:01 GMT  
		Size: 76.3 MB (76325441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:61adb8691477fa8b98139d0377cc569bd2ed042514de666a4b183afb2ff2b409
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350419138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77107989faa08df0c4a6f0882b85d6ee3689c92364bb55a6d008612739e2c16f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:23:39 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973c559ce2026b1ae03fa797235c10a6c9e186e5a06bd9f483b1bf291530d5a`  
		Last Modified: Thu, 16 Jan 2020 03:13:37 GMT  
		Size: 77.8 MB (77819851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:c11823d856edb73de81178998925b594ed355f00c04e72fec120f44fd7135395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:d6064a191f4d05536906c70d383bb7d6b9dc68d968f2d8421d0142c85df22f77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299847099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da2c79c08d094f07f08b9be029bcd7f4c87cad533917662552e50cbc2d61a26`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5d0ba1e209a87319c13c0dcc46624885b70f03aefbe4d674264c6bedadacd287
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260283861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7d0e47b5d227a696151c6dcb03c7d8127acdc3ef603e7317b1328604638ada`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9ef434329904a1e126b6be2a29fd78634640f3417a178cbffd08cd14bd574bc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272599287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db694db52cb9b174d57d38ba2b52b6de66f29c1c1212adfad963c71470783bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:c11823d856edb73de81178998925b594ed355f00c04e72fec120f44fd7135395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:d6064a191f4d05536906c70d383bb7d6b9dc68d968f2d8421d0142c85df22f77
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299847099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da2c79c08d094f07f08b9be029bcd7f4c87cad533917662552e50cbc2d61a26`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:21:30 GMT
ADD file:4b2eb5cd0b37ca0154f3c5ad9212f5bc7244a35806395a9c76a96723d708b83a in / 
# Thu, 16 Jan 2020 01:21:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:21:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:21:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:21:32 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:01:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:01:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:02:03 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:02:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:02:12 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:02:12 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 04:03:57 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:03:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:03:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:03:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0a01a72a686c389637334de1e2d0012da298960366f6d8f358b8e10dc3b5e330`  
		Last Modified: Wed, 15 Jan 2020 14:20:15 GMT  
		Size: 44.1 MB (44149770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc899a5544da1a6cfb970d2484d32c063f8df26a430d92f39c98e72261e226f2`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 525.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19197c55075519928dd2ff059745665a2c9b72f4e8af6f7a1ce662e696d339bd`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d454e56b61d1343a01f3b1829574333e2e3df20e77d1958d7b0b939ea1b61`  
		Last Modified: Thu, 16 Jan 2020 01:22:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010ead50ff2ec649b18dd41180cebf093d5b97c01f6a49d1946ec7b263c289f`  
		Last Modified: Thu, 16 Jan 2020 04:28:58 GMT  
		Size: 6.9 MB (6938171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec530673015c258ed1d32c117b99c651da72a0667515abf5996a0d622bc15489`  
		Last Modified: Thu, 16 Jan 2020 04:28:56 GMT  
		Size: 13.1 KB (13100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e60d0819b969cd84de779dd8ec52c6a809c022bbb15f36d83e3c01e7089ada`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645661e83f1a0793216a6d7adf0026e0317effd5bdddf2ee98d7496c1666f00`  
		Last Modified: Thu, 16 Jan 2020 04:29:11 GMT  
		Size: 54.8 MB (54775919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4eeacdef1b910fd8f881a1c08a8932662896fe4384b5afcbb99431b5fbca01`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 412.1 KB (412109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7f1bf131196a8f6ac1ec153e78523a6d2ffa038707e0f2613d7fe1f424999`  
		Last Modified: Thu, 16 Jan 2020 04:29:40 GMT  
		Size: 193.6 MB (193556074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac605ca46bc5fc154751bfab37718cbc6b5f9ae502eb985bebe6c02fcda6ad93`  
		Last Modified: Thu, 16 Jan 2020 04:28:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:5d0ba1e209a87319c13c0dcc46624885b70f03aefbe4d674264c6bedadacd287
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.3 MB (260283861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7d0e47b5d227a696151c6dcb03c7d8127acdc3ef603e7317b1328604638ada`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:03:19 GMT
ADD file:8ff374873b44e76e7a7762ed03569b1ed53a0b680461b5eab44a553e034c54ed in / 
# Thu, 16 Jan 2020 01:03:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:03:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:03:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:03:53 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:28:00 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:28:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:28:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:29:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:29:45 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:29:46 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:30:04 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:30:05 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:34:06 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:34:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:34:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e60df59fb5976f9565e2660056a379f90dbe8a58e5ee5451ec92647e519abb26`  
		Last Modified: Thu, 16 Jan 2020 01:05:33 GMT  
		Size: 38.8 MB (38847547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ba0251fafa2d367b89edee66fcb80412d5dfbf17c303256da18cf760c8a1f9`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff14f7ed750ba6c66f6be53003361516dcaa6ae4c7d88746ce88a03484db05e`  
		Last Modified: Thu, 16 Jan 2020 01:05:21 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c86faa0776e2a98a9a3d92814b0f90fb2ef3e3375d013fa61bb8c0c904046`  
		Last Modified: Thu, 16 Jan 2020 01:05:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb1a44b25d86bc6e450a95fffe5cc145f4d52f851b01c8b768e85492b7111e8`  
		Last Modified: Thu, 16 Jan 2020 03:18:33 GMT  
		Size: 5.7 MB (5702480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba76d2b9a2c976cd0cf0f3cb1bae7a32a79270aff7b737ef36b19b8bbf70b9e7`  
		Last Modified: Thu, 16 Jan 2020 03:18:32 GMT  
		Size: 13.1 KB (13104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb06998c93036fd282dbdc54607d50cc60276ec483736884a0267fb2ed57fde4`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e621b6ac96be1b25605d41923dff1cf424179836b5ffc24389925f771b4f0244`  
		Last Modified: Thu, 16 Jan 2020 03:18:49 GMT  
		Size: 50.3 MB (50348271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b926cb02815487a322cd1941f82b1e29f5fce6368ab34c3c74e2e1342617a`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 412.1 KB (412069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaa2962a935dd4e57a0e25e4fbd76cf1c7e99a5e759c7948f736bbf68396af`  
		Last Modified: Thu, 16 Jan 2020 03:19:27 GMT  
		Size: 165.0 MB (164958438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042d1b58ba351b5a7796833c505ecad1ad0c916d9f6f30a11bd16ba5699b9b8`  
		Last Modified: Thu, 16 Jan 2020 03:18:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c9ef434329904a1e126b6be2a29fd78634640f3417a178cbffd08cd14bd574bc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272599287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db694db52cb9b174d57d38ba2b52b6de66f29c1c1212adfad963c71470783bc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:42:43 GMT
ADD file:d374c720bcf7aac426612a43ac539c3bb5b831a9a9e476a3919ed185eb77deca in / 
# Thu, 16 Jan 2020 00:42:53 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:42:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:43:02 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:43:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:14:46 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:14:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:14:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:17:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:17:35 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:17:36 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:17:54 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:17:55 GMT
ENV ROS_DISTRO=kinetic
# Thu, 16 Jan 2020 02:21:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:21:51 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:21:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:21:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:185661474c6b71ced0eb4cd45f81a17a651d404bfd04903ba0bf3eb815e2cc1d`  
		Last Modified: Thu, 16 Jan 2020 00:44:31 GMT  
		Size: 39.9 MB (39890711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053aaa7a7ba304aae4e3327a0d30a33f5c3fe9fca6e8ef86dd8226b13c29e28d`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ccb1337bb94e5b9ea19de7478366666cde129fb3214d092d15ebcfb644d8bb`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1fb143b02bcaaba5f01be18d73c8072c3687fe6e24464871a825e90416f60`  
		Last Modified: Thu, 16 Jan 2020 00:44:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ceb92e6f4201bdf8793f64aa103c2c8fd72b020d1fd1cc4cbf5fff30b0a27`  
		Last Modified: Thu, 16 Jan 2020 03:12:16 GMT  
		Size: 6.0 MB (5960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a3c557b414c34ea2ae77c7881853678e332de98a573fbdddbfd4866059ee4`  
		Last Modified: Thu, 16 Jan 2020 03:12:15 GMT  
		Size: 13.1 KB (13106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75473607edc5e843ebbe5f0ac51e4931b60b4cdb86b24426f9be2390e9f14dad`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce06b66114bbeb074e9283d26e72c7fc14613491d22fda52cfaf4ddb93a7b0b`  
		Last Modified: Thu, 16 Jan 2020 03:12:29 GMT  
		Size: 52.1 MB (52072633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0742cddec8c616de16fc668ac3f8e310aa6b6f1afdccc2b4d4acf4baa0888de`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 412.2 KB (412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e24bdd50ca9c0196c66fe74e8ac74366559174d0643e94f9b1029268a7630`  
		Last Modified: Thu, 16 Jan 2020 03:13:04 GMT  
		Size: 174.2 MB (174248716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b33e51ce7794d8770ba74cb28f0312e59c72ecfe23ea6711337db42cf14159`  
		Last Modified: Thu, 16 Jan 2020 03:12:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:380a4afed7c294394662de2cbda6757ceeba499c7ff5bd41a4c3f7bc41a91aa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:051d5af176ed91de0384f4524bf6820cc325f16e32fdbb9715f7e194b5ca3a6d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.4 MB (419369514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d421f8825627e33e65ea2376c6c0f66de4fafc713c1962d5913b8b1213fa58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm variant v7

```console
$ docker pull ros@sha256:da9a0650f1934edcbe631a9baaf4c593eea71834706e18e8d6516714c7689823
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.2 MB (372195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d091638dd04ba6737e13119939ad257b24a46d5d1ff83dd5755d3a6d33af7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8691bcd38f7325d3fbe8e7203842f40d0be8bb995e792e2a019bc964dfc49b90
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395828307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378a0887ed4c6132ad327ea544378650843be5227cf6037d80635b233556dae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:380a4afed7c294394662de2cbda6757ceeba499c7ff5bd41a4c3f7bc41a91aa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:051d5af176ed91de0384f4524bf6820cc325f16e32fdbb9715f7e194b5ca3a6d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.4 MB (419369514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d421f8825627e33e65ea2376c6c0f66de4fafc713c1962d5913b8b1213fa58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:da9a0650f1934edcbe631a9baaf4c593eea71834706e18e8d6516714c7689823
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.2 MB (372195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d091638dd04ba6737e13119939ad257b24a46d5d1ff83dd5755d3a6d33af7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8691bcd38f7325d3fbe8e7203842f40d0be8bb995e792e2a019bc964dfc49b90
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395828307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378a0887ed4c6132ad327ea544378650843be5227cf6037d80635b233556dae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:36610fdd20ce4f3c64471a20788fed6a510a604b6cb1acf1128596bfc617ed19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:c42d7b6eaf842e6239771941625d487788e72e285d12c38baac66ce186405fb0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.7 MB (768664232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11088ba5f50df179c2b22e21e2f815ad7d6cc9644ccee7eb001014bd8e8f941a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:22:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114cf75d86fbd1bd7b0f8e2f0778636e7f914b9c83f71ac0907a247099d96361`  
		Last Modified: Thu, 16 Jan 2020 04:34:46 GMT  
		Size: 349.3 MB (349294718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:c8650bae35abffed746fd779459964566f400bcde0fcb94a83a2ca54294042e2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **671.5 MB (671526941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c91f3bb491038b1221748ae6912ddf255803acca694cc983ba1df0f9fb6c60`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:53 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4aec6c8ed6a2abfa34a2f9f513d4b4e5e011d04e81194e0e9559c46fafdab70`  
		Last Modified: Thu, 16 Jan 2020 03:26:22 GMT  
		Size: 299.3 MB (299331258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:88eedb427a4d287f7bcca5ca38f8148c71ffb7fed951d1bf08376dc135bddf88
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.7 MB (727739317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2929760a1bef0568837746082474f7a718c51d42cb18d9f25f7872c4783ce1f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:50:18 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62400ae97f21e77ff9ae74b582a65478d8c350b38a7436a5d15ab5c11ffc5f11`  
		Last Modified: Thu, 16 Jan 2020 03:20:27 GMT  
		Size: 331.9 MB (331911010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:36610fdd20ce4f3c64471a20788fed6a510a604b6cb1acf1128596bfc617ed19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:c42d7b6eaf842e6239771941625d487788e72e285d12c38baac66ce186405fb0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **768.7 MB (768664232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11088ba5f50df179c2b22e21e2f815ad7d6cc9644ccee7eb001014bd8e8f941a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:22:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114cf75d86fbd1bd7b0f8e2f0778636e7f914b9c83f71ac0907a247099d96361`  
		Last Modified: Thu, 16 Jan 2020 04:34:46 GMT  
		Size: 349.3 MB (349294718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:c8650bae35abffed746fd779459964566f400bcde0fcb94a83a2ca54294042e2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **671.5 MB (671526941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c91f3bb491038b1221748ae6912ddf255803acca694cc983ba1df0f9fb6c60`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:06:53 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4aec6c8ed6a2abfa34a2f9f513d4b4e5e011d04e81194e0e9559c46fafdab70`  
		Last Modified: Thu, 16 Jan 2020 03:26:22 GMT  
		Size: 299.3 MB (299331258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:88eedb427a4d287f7bcca5ca38f8148c71ffb7fed951d1bf08376dc135bddf88
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **727.7 MB (727739317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2929760a1bef0568837746082474f7a718c51d42cb18d9f25f7872c4783ce1f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:50:18 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62400ae97f21e77ff9ae74b582a65478d8c350b38a7436a5d15ab5c11ffc5f11`  
		Last Modified: Thu, 16 Jan 2020 03:20:27 GMT  
		Size: 331.9 MB (331911010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:f479c0b9b2cf1db20fcf913425f9aaf75b65c30866207a70673852e5757acb78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:4c4d41289c5c477347591ae5f7e982621e5472529c829ff8c1efa81ea41aec0b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **876.3 MB (876331066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:603424d168bbf73c728d468785aad51e2e294b582bb394a973f47ed8379b8718`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:26:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:26:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 08:26:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 08:27:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:27:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:27:03 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 08:27:21 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 08:27:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 08:29:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:29:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 08:29:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 08:29:07 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:30:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:33:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf93dae3672c4b23e304be8bfbd86a1a70e192920d9bb7d980774a433b7123`  
		Last Modified: Sat, 28 Dec 2019 08:34:45 GMT  
		Size: 10.5 MB (10476716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4d94fcfba96b58c2a901f6286ca7d1ce99dacfe09968fc037d5553f2025e8a`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa7ebb2626a2bc1ed27e07d7ca29f5a02c7cfb09f84608d38f9c99b1b798ced`  
		Last Modified: Sat, 28 Dec 2019 08:34:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08219e7fdb9a27aa4c99a6f1d467eab7640d963871a1400ebfdaae3af68c57`  
		Last Modified: Sat, 28 Dec 2019 08:35:00 GMT  
		Size: 64.8 MB (64771041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4191195f75e3d8a24ce1e680579fd09913504e418871b9b7ec1e38aaa061fdd1`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 451.5 KB (451468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fd3f2a56a2d531756ee769940fada1e88517a593b70c3e21e959874a7bc78`  
		Last Modified: Sat, 28 Dec 2019 08:35:41 GMT  
		Size: 270.4 MB (270404151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0106c5e798490c33945ce9ebe7647215eb890cf55e081b770471e498436353`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2db8c7023a66d21e38358720aab69dc412fb39a5366737c69bc7bbb76c53ba1`  
		Last Modified: Sat, 28 Dec 2019 08:36:17 GMT  
		Size: 108.5 MB (108473946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e00711f861b9c055a4a53b6b4cd5db34f3e2dd6f6919595b5630854da331048`  
		Last Modified: Sat, 28 Dec 2019 08:38:37 GMT  
		Size: 376.4 MB (376371186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a37ab6bf0820d77cc72df9028681ab1de373743fe259b5f63fa0428e5315040f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.1 MB (794089994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed189ff040a6be63c69243fa04762c1f8bfc155ee47616b03b5cc305ca617c98`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:34:23 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:34:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 18:34:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 18:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:35:40 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:35:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 18:36:03 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 18:36:04 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 18:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:39:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 18:39:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 18:39:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:40:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:47:10 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facfbd1fae886a379926b7add3095adbf575d32e87e67282e12488332f12f747`  
		Last Modified: Sat, 28 Dec 2019 18:48:28 GMT  
		Size: 9.8 MB (9774604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a6b709bed6b18e5ba839847d0f3e3a5a4e53a163b69ea7858c561fdc7f1e3a`  
		Last Modified: Sat, 28 Dec 2019 18:48:25 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9a8179e95515f1f6e62a300ca75906566906d949c7403c9f61b8511afc033`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b6ea616f3e8e138683f48ca757b84bc23de865b250839eba047a141cc6721`  
		Last Modified: Sat, 28 Dec 2019 18:48:46 GMT  
		Size: 62.1 MB (62085764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101b4656b4d26f6236d97a86a31ae20834b113b525d2830521853323cfb6369`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 451.5 KB (451514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5e52b33734a366437f8b9e807980e3273684eeef72d2fd1822dc4ea7ae5638`  
		Last Modified: Sat, 28 Dec 2019 18:49:32 GMT  
		Size: 224.6 MB (224573326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de7b9c0321a0098bd333b1ceb564c2a4389249dc4f9e3f45da7c389198a1ba`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033d8666e6f7cc5f88f89356fb0b79d8bcb42f576c433b924571484da93bdc43`  
		Last Modified: Sat, 28 Dec 2019 18:50:04 GMT  
		Size: 103.0 MB (102961244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8023d447d2b366f450e3089908dbf1ee5a2f68483463b3eec7364566a1771`  
		Last Modified: Sat, 28 Dec 2019 18:52:10 GMT  
		Size: 351.1 MB (351075248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:b1dd5077a4fc86c48f11a1e84e115f01b021674d62fbe192314f41a6167e8e8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:88ee0a6d7c386eac067943bfee350289a618636d8387b3946907cf3e7646e21d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.2 MB (457195447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d410bb05680d834ae4d80d607aae3c233bc9d817e5c8f3d9e469c783a53e14b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:17:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c185d12acf27cd0aadc34e745cf2a73e7c90fd02c2328dddeb33ba9f9a2f5a`  
		Last Modified: Thu, 16 Jan 2020 04:33:28 GMT  
		Size: 37.8 MB (37825933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:69ba7ec0b5efbf39a5b7ef367192a4afda4ea218a99efde4832363ee7ca37514
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.6 MB (405627728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9e1a93a21096872ae41b64cb23d0063104db91010b8f78bfe31faf579032c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:57:36 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40040fada30e64b2c566c0dcbe12e8ca6abc9c54ead038f4bb79208cbf7cdc7c`  
		Last Modified: Thu, 16 Jan 2020 03:24:38 GMT  
		Size: 33.4 MB (33432045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:46c29af943c0ad62231688dffb2922cfd81d8285ffe1ac4ea357c9262af2b0cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.4 MB (431428607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ce1085dca0c890444c208e463b822291d01dbb74f41ec6f714149763b4c50a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:43:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d3650c842b05112dd7c6a92df50422c0c869c50e1f1224e73d6691cd067e87`  
		Last Modified: Thu, 16 Jan 2020 03:18:36 GMT  
		Size: 35.6 MB (35600300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:b1dd5077a4fc86c48f11a1e84e115f01b021674d62fbe192314f41a6167e8e8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:88ee0a6d7c386eac067943bfee350289a618636d8387b3946907cf3e7646e21d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.2 MB (457195447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d410bb05680d834ae4d80d607aae3c233bc9d817e5c8f3d9e469c783a53e14b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:17:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c185d12acf27cd0aadc34e745cf2a73e7c90fd02c2328dddeb33ba9f9a2f5a`  
		Last Modified: Thu, 16 Jan 2020 04:33:28 GMT  
		Size: 37.8 MB (37825933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:69ba7ec0b5efbf39a5b7ef367192a4afda4ea218a99efde4832363ee7ca37514
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.6 MB (405627728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9e1a93a21096872ae41b64cb23d0063104db91010b8f78bfe31faf579032c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:57:36 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40040fada30e64b2c566c0dcbe12e8ca6abc9c54ead038f4bb79208cbf7cdc7c`  
		Last Modified: Thu, 16 Jan 2020 03:24:38 GMT  
		Size: 33.4 MB (33432045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:46c29af943c0ad62231688dffb2922cfd81d8285ffe1ac4ea357c9262af2b0cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.4 MB (431428607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ce1085dca0c890444c208e463b822291d01dbb74f41ec6f714149763b4c50a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:43:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d3650c842b05112dd7c6a92df50422c0c869c50e1f1224e73d6691cd067e87`  
		Last Modified: Thu, 16 Jan 2020 03:18:36 GMT  
		Size: 35.6 MB (35600300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:6c102c9db9a12ac05ca4ecbf00008dbb48fa6cfe74ce7e1f1b010d511c9074bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:bfe8b818535c76586b58ecc7483bdff42271664cbbebf0565bebdd546df7f060
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.3 MB (555257867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8bd493dbb7aa0c510c6b607557211be54160da982b18746d8ddeddf67a0ba9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:26:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:26:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 08:26:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 08:27:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:27:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:27:03 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 08:27:21 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 08:27:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 08:29:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:29:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 08:29:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 08:29:07 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:30:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:31:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf93dae3672c4b23e304be8bfbd86a1a70e192920d9bb7d980774a433b7123`  
		Last Modified: Sat, 28 Dec 2019 08:34:45 GMT  
		Size: 10.5 MB (10476716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4d94fcfba96b58c2a901f6286ca7d1ce99dacfe09968fc037d5553f2025e8a`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa7ebb2626a2bc1ed27e07d7ca29f5a02c7cfb09f84608d38f9c99b1b798ced`  
		Last Modified: Sat, 28 Dec 2019 08:34:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08219e7fdb9a27aa4c99a6f1d467eab7640d963871a1400ebfdaae3af68c57`  
		Last Modified: Sat, 28 Dec 2019 08:35:00 GMT  
		Size: 64.8 MB (64771041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4191195f75e3d8a24ce1e680579fd09913504e418871b9b7ec1e38aaa061fdd1`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 451.5 KB (451468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fd3f2a56a2d531756ee769940fada1e88517a593b70c3e21e959874a7bc78`  
		Last Modified: Sat, 28 Dec 2019 08:35:41 GMT  
		Size: 270.4 MB (270404151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0106c5e798490c33945ce9ebe7647215eb890cf55e081b770471e498436353`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2db8c7023a66d21e38358720aab69dc412fb39a5366737c69bc7bbb76c53ba1`  
		Last Modified: Sat, 28 Dec 2019 08:36:17 GMT  
		Size: 108.5 MB (108473946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e16b33263adec4f1c03667573f6c3b75bb569d408fcae9b0bae116cad8f387a`  
		Last Modified: Sat, 28 Dec 2019 08:36:44 GMT  
		Size: 55.3 MB (55297987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:44b25396f459f6ad6d285ad9d4baf6e8f8eadc3038876b7bdbdf977873a29a5f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.6 MB (495596210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892f7831c3059d2c225b6ded4253b3541828d9b2cc3c195d6bfd261ae98578ee`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:34:23 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:34:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 18:34:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 18:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:35:40 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:35:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 18:36:03 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 18:36:04 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 18:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:39:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 18:39:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 18:39:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:40:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:41:43 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facfbd1fae886a379926b7add3095adbf575d32e87e67282e12488332f12f747`  
		Last Modified: Sat, 28 Dec 2019 18:48:28 GMT  
		Size: 9.8 MB (9774604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a6b709bed6b18e5ba839847d0f3e3a5a4e53a163b69ea7858c561fdc7f1e3a`  
		Last Modified: Sat, 28 Dec 2019 18:48:25 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9a8179e95515f1f6e62a300ca75906566906d949c7403c9f61b8511afc033`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b6ea616f3e8e138683f48ca757b84bc23de865b250839eba047a141cc6721`  
		Last Modified: Sat, 28 Dec 2019 18:48:46 GMT  
		Size: 62.1 MB (62085764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101b4656b4d26f6236d97a86a31ae20834b113b525d2830521853323cfb6369`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 451.5 KB (451514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5e52b33734a366437f8b9e807980e3273684eeef72d2fd1822dc4ea7ae5638`  
		Last Modified: Sat, 28 Dec 2019 18:49:32 GMT  
		Size: 224.6 MB (224573326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de7b9c0321a0098bd333b1ceb564c2a4389249dc4f9e3f45da7c389198a1ba`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033d8666e6f7cc5f88f89356fb0b79d8bcb42f576c433b924571484da93bdc43`  
		Last Modified: Sat, 28 Dec 2019 18:50:04 GMT  
		Size: 103.0 MB (102961244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be1af64328e4305c7048a43c021ab70b6023255e1fef0eb01a7cd97128eec9`  
		Last Modified: Sat, 28 Dec 2019 18:50:24 GMT  
		Size: 52.6 MB (52581464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:380a4afed7c294394662de2cbda6757ceeba499c7ff5bd41a4c3f7bc41a91aa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:051d5af176ed91de0384f4524bf6820cc325f16e32fdbb9715f7e194b5ca3a6d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.4 MB (419369514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d421f8825627e33e65ea2376c6c0f66de4fafc713c1962d5913b8b1213fa58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:da9a0650f1934edcbe631a9baaf4c593eea71834706e18e8d6516714c7689823
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.2 MB (372195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d091638dd04ba6737e13119939ad257b24a46d5d1ff83dd5755d3a6d33af7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8691bcd38f7325d3fbe8e7203842f40d0be8bb995e792e2a019bc964dfc49b90
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395828307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378a0887ed4c6132ad327ea544378650843be5227cf6037d80635b233556dae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:380a4afed7c294394662de2cbda6757ceeba499c7ff5bd41a4c3f7bc41a91aa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:051d5af176ed91de0384f4524bf6820cc325f16e32fdbb9715f7e194b5ca3a6d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.4 MB (419369514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d421f8825627e33e65ea2376c6c0f66de4fafc713c1962d5913b8b1213fa58`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 04:16:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac5f454b420fcb32e3c74b5b36f06769ab69c2619538df477c7fc7a54a0bff3`  
		Last Modified: Thu, 16 Jan 2020 04:33:14 GMT  
		Size: 68.3 MB (68335269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:da9a0650f1934edcbe631a9baaf4c593eea71834706e18e8d6516714c7689823
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.2 MB (372195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d091638dd04ba6737e13119939ad257b24a46d5d1ff83dd5755d3a6d33af7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:56:17 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813469314f33aa7c67712116daba39423fe227db2c28d23d580e7a7fa0c329e1`  
		Last Modified: Thu, 16 Jan 2020 03:24:14 GMT  
		Size: 60.3 MB (60258979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8691bcd38f7325d3fbe8e7203842f40d0be8bb995e792e2a019bc964dfc49b90
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395828307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378a0887ed4c6132ad327ea544378650843be5227cf6037d80635b233556dae7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
# Thu, 16 Jan 2020 02:42:13 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cc983dd196368c762e3263e975753e3e28a3f2eb576151dd8ec809fcdf6e88`  
		Last Modified: Thu, 16 Jan 2020 03:18:15 GMT  
		Size: 62.8 MB (62842507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:5ea106fc953880e151e8b2c8afc1fb2eb9f1e8c92e419161a4f1627f67e17464
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:b03e9701a180b9ce5d6df50bc0a23b7a3dfd2fa592c7f1444343790880ec7fd8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.0 MB (499959880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cc38ae8baaac327b75ffd4fd8d36c8f4f57546d4169209651465da229f1657`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:26:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:26:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 08:26:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 08:27:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:27:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:27:03 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 08:27:21 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 08:27:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 08:29:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:29:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 08:29:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 08:29:07 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:30:14 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf93dae3672c4b23e304be8bfbd86a1a70e192920d9bb7d980774a433b7123`  
		Last Modified: Sat, 28 Dec 2019 08:34:45 GMT  
		Size: 10.5 MB (10476716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4d94fcfba96b58c2a901f6286ca7d1ce99dacfe09968fc037d5553f2025e8a`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa7ebb2626a2bc1ed27e07d7ca29f5a02c7cfb09f84608d38f9c99b1b798ced`  
		Last Modified: Sat, 28 Dec 2019 08:34:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08219e7fdb9a27aa4c99a6f1d467eab7640d963871a1400ebfdaae3af68c57`  
		Last Modified: Sat, 28 Dec 2019 08:35:00 GMT  
		Size: 64.8 MB (64771041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4191195f75e3d8a24ce1e680579fd09913504e418871b9b7ec1e38aaa061fdd1`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 451.5 KB (451468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fd3f2a56a2d531756ee769940fada1e88517a593b70c3e21e959874a7bc78`  
		Last Modified: Sat, 28 Dec 2019 08:35:41 GMT  
		Size: 270.4 MB (270404151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0106c5e798490c33945ce9ebe7647215eb890cf55e081b770471e498436353`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2db8c7023a66d21e38358720aab69dc412fb39a5366737c69bc7bbb76c53ba1`  
		Last Modified: Sat, 28 Dec 2019 08:36:17 GMT  
		Size: 108.5 MB (108473946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bda4c8f3ddfb11e74a3e7a6e33f13b388b7b667c4832e20f0e3e0b11f486dbba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.0 MB (443014746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95461410a52add4d5ba4d8315b9518d7ed40ff65a2044a57092a0b99fcbd92c5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:34:23 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:34:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 18:34:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 18:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:35:40 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:35:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 18:36:03 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 18:36:04 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 18:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:39:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 18:39:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 18:39:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:40:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facfbd1fae886a379926b7add3095adbf575d32e87e67282e12488332f12f747`  
		Last Modified: Sat, 28 Dec 2019 18:48:28 GMT  
		Size: 9.8 MB (9774604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a6b709bed6b18e5ba839847d0f3e3a5a4e53a163b69ea7858c561fdc7f1e3a`  
		Last Modified: Sat, 28 Dec 2019 18:48:25 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9a8179e95515f1f6e62a300ca75906566906d949c7403c9f61b8511afc033`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b6ea616f3e8e138683f48ca757b84bc23de865b250839eba047a141cc6721`  
		Last Modified: Sat, 28 Dec 2019 18:48:46 GMT  
		Size: 62.1 MB (62085764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101b4656b4d26f6236d97a86a31ae20834b113b525d2830521853323cfb6369`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 451.5 KB (451514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5e52b33734a366437f8b9e807980e3273684eeef72d2fd1822dc4ea7ae5638`  
		Last Modified: Sat, 28 Dec 2019 18:49:32 GMT  
		Size: 224.6 MB (224573326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de7b9c0321a0098bd333b1ceb564c2a4389249dc4f9e3f45da7c389198a1ba`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033d8666e6f7cc5f88f89356fb0b79d8bcb42f576c433b924571484da93bdc43`  
		Last Modified: Sat, 28 Dec 2019 18:50:04 GMT  
		Size: 103.0 MB (102961244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:57875f93db51408e940925dd04a9312480ce9ad1e78007bb60395a38a72552e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:55c4aad24f30758bf3cb5585fc568d009b2e43885ff4e662b9d4aab7d7671d83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (351034245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a0b423471bc8cab29d2ffc4d6cafcdc6e8f1e4231e2cf962c4785a02edf901`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:39f33fa5b1e561050a31b5eebf50ec4292e97b3c43ebee50df585174f6417b8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311936704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c516b6abff2d35fc4c614fdb223f2556298f441625f6cd86c6226a03ad1e48c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d06863fa742a162f5697f997d820e3715199d35fe5c883d5590f8421bbe5e1ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (332985800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e38fc14f69f2da932fdc039b825b011df5a463ac0911a8459af63658ddcb99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:57875f93db51408e940925dd04a9312480ce9ad1e78007bb60395a38a72552e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:55c4aad24f30758bf3cb5585fc568d009b2e43885ff4e662b9d4aab7d7671d83
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (351034245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a0b423471bc8cab29d2ffc4d6cafcdc6e8f1e4231e2cf962c4785a02edf901`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:03:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:48 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:10:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 04:10:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 04:11:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 04:11:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 04:11:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 04:11:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 04:14:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 04:14:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 04:14:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 04:14:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d3d671a391edc5fd92631386fbbc92fe5e40fa6a05d01dfbbfee269400c37`  
		Last Modified: Thu, 16 Jan 2020 02:16:29 GMT  
		Size: 837.6 KB (837636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812d1f6ed8dd1d5e59776a248058ed558bec065885af5fa552541ff4571644`  
		Last Modified: Thu, 16 Jan 2020 04:32:04 GMT  
		Size: 6.8 MB (6776606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290e7247cb8cc08ab823223cfe3cfeda5a45d02c50bb6e67ee7dbf791e230c00`  
		Last Modified: Thu, 16 Jan 2020 04:32:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147359e88db8fb8d787ec3edfd336bf8a249d225a0a5664390910d6f7939625d`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f68f113cd17c129b367d416aea1c97dc01e0eb694e94efc5cb34c5b26a0628`  
		Last Modified: Thu, 16 Jan 2020 04:32:15 GMT  
		Size: 55.1 MB (55077806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55619b268b204efa45a3b07e10c8166cb74a530da27233791a978d4b9bc44d4`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 412.1 KB (412096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38821ec799ff2d8f654ce0ec1b457890235026687eeaf4436adc3c56b69a3270`  
		Last Modified: Thu, 16 Jan 2020 04:32:53 GMT  
		Size: 261.2 MB (261201700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6ec8634ca69db0cf4576d761aea36f8b1f080bf9d06199c4ffcb7c5cb7590`  
		Last Modified: Thu, 16 Jan 2020 04:32:01 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:39f33fa5b1e561050a31b5eebf50ec4292e97b3c43ebee50df585174f6417b8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311936704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c516b6abff2d35fc4c614fdb223f2556298f441625f6cd86c6226a03ad1e48c9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:59:53 GMT
ADD file:28b9597b09e4e4e5e7dd1ff3e470cdc76c4b8dfe6f37e8e0014be90c0e172630 in / 
# Thu, 16 Jan 2020 00:59:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:59:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:02 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:21:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:22 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:46:29 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:47:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:48:05 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:48:07 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:48:25 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:48:26 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:53:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:58 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:54:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:54:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b7971fe48ea2bad85b2c477dc04973a339494497fb370b0d70644d8112e48b98`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 22.3 MB (22275271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f69e9f176e3248cd66374739e12b3cf3a04e10db7a54c44fd0e966335c47d`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 35.5 KB (35467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de5a1686ec92fdd4e9870238004fe56639bc59ce8564133b6a54176d8b4603`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bdbc1afabc79dc485c1e0c118c0dfd22850abb2909cd280cb8b38e6a5609cf`  
		Last Modified: Thu, 16 Jan 2020 01:04:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0a0e8f9a76750d5fa3cd6347459abf8f53fb7a24bff4818565277948c365d`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 838.0 KB (837972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afea582433627b44b45c209c1eafb228291d8251aadf1188815fa8b94702088`  
		Last Modified: Thu, 16 Jan 2020 03:22:35 GMT  
		Size: 5.6 MB (5627278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e04191fc517d34a6f00a9baf737f55a1eb7cbe2be06ad4e7dec27c713475267`  
		Last Modified: Thu, 16 Jan 2020 03:22:34 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3161bcbf665d558872efaff811ddf578333c5e80dd9df07fc8c627b87574`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75fb7085f80fae8085a22fa96a042a7a4759cbd79b8f880e5e06c959075ad`  
		Last Modified: Thu, 16 Jan 2020 03:22:50 GMT  
		Size: 50.1 MB (50113484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b5e115bb1d0e8acbeb041939e45c8d336d53cb60376f57c66d3da947ae5187`  
		Last Modified: Thu, 16 Jan 2020 03:22:32 GMT  
		Size: 412.1 KB (412067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de7cc621d8e90289090c4db5ccb4109b8e718431c84ad47509430e5c5f991e`  
		Last Modified: Thu, 16 Jan 2020 03:23:43 GMT  
		Size: 232.6 MB (232632283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0170bd2e00a236ce10c454d3023af83efb5b18d108ec6490d3ac8e824ba9a81`  
		Last Modified: Thu, 16 Jan 2020 03:22:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d06863fa742a162f5697f997d820e3715199d35fe5c883d5590f8421bbe5e1ef
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (332985800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e38fc14f69f2da932fdc039b825b011df5a463ac0911a8459af63658ddcb99`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:52:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:32:56 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:33:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 16 Jan 2020 02:33:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 16 Jan 2020 02:34:27 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:34:31 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jan 2020 02:34:33 GMT
ENV LC_ALL=C.UTF-8
# Thu, 16 Jan 2020 02:34:50 GMT
RUN rosdep init     && rosdep update
# Thu, 16 Jan 2020 02:34:51 GMT
ENV ROS_DISTRO=melodic
# Thu, 16 Jan 2020 02:39:33 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:39:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 16 Jan 2020 02:39:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 16 Jan 2020 02:39:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b42839d03341491d16e4449922b9674f34688930e1dad70b4fd9ab728504074`  
		Last Modified: Thu, 16 Jan 2020 02:11:31 GMT  
		Size: 837.7 KB (837706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c0632a1e3af7dcdbb482f388a48cc0b2a87ed266502df602e07070e80a46a9`  
		Last Modified: Thu, 16 Jan 2020 03:16:31 GMT  
		Size: 6.1 MB (6093848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3cfa95b8905719876b58d047407cdc5783a82d58185bf1a638b87ca54e2f6`  
		Last Modified: Thu, 16 Jan 2020 03:16:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c79eaf7f345ef3a8519f515ee4189df260d7d9aebfe5e91a36032de95b88ae`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9581c522759aa50955b6e7e59bb2eae77e44155a362662299a8dc4f0bf8b099`  
		Last Modified: Thu, 16 Jan 2020 03:16:50 GMT  
		Size: 52.9 MB (52924682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a6c5571d269d265635f78d7e090eabad27ecc6ce711a38f6cb80257e103dd`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 412.2 KB (412159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa09e580018b5005a473fcb32bd2f97d8895261faeebbae544060efc706b82d`  
		Last Modified: Thu, 16 Jan 2020 03:17:36 GMT  
		Size: 249.0 MB (248959829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55a63abafead34aa0be1edc317c2c83c1a2ba881a9e069beb7e7bca006a668f`  
		Last Modified: Thu, 16 Jan 2020 03:16:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:7f6d57bf3e025d7f7311adeee42aa8042c51c5f2decb742908aad12d1444c56f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:43aaaa6cfb47d8de9eb5b33e656a4e9747a57a7c09c3933cac178d0052794aea
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.5 MB (391485934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bac88139a4ae488377be19ec7123f1ce8e6e1e001bef55d16813f80f4aa1e54`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:26:02 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:26:06 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 08:26:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 08:27:02 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:27:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:27:03 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 08:27:21 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 08:27:21 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 08:29:05 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:29:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 08:29:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 08:29:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf93dae3672c4b23e304be8bfbd86a1a70e192920d9bb7d980774a433b7123`  
		Last Modified: Sat, 28 Dec 2019 08:34:45 GMT  
		Size: 10.5 MB (10476716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4d94fcfba96b58c2a901f6286ca7d1ce99dacfe09968fc037d5553f2025e8a`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa7ebb2626a2bc1ed27e07d7ca29f5a02c7cfb09f84608d38f9c99b1b798ced`  
		Last Modified: Sat, 28 Dec 2019 08:34:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08219e7fdb9a27aa4c99a6f1d467eab7640d963871a1400ebfdaae3af68c57`  
		Last Modified: Sat, 28 Dec 2019 08:35:00 GMT  
		Size: 64.8 MB (64771041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4191195f75e3d8a24ce1e680579fd09913504e418871b9b7ec1e38aaa061fdd1`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 451.5 KB (451468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fd3f2a56a2d531756ee769940fada1e88517a593b70c3e21e959874a7bc78`  
		Last Modified: Sat, 28 Dec 2019 08:35:41 GMT  
		Size: 270.4 MB (270404151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0106c5e798490c33945ce9ebe7647215eb890cf55e081b770471e498436353`  
		Last Modified: Sat, 28 Dec 2019 08:34:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f5ec08ded445c9338b439668c8e668290ed0528a5cc3278334fe8e7b6a44f748
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340053502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eed90e0838aeb67fd3fa8237f21c25198eacd48a0305185d1e41973423fc8b5e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:34:23 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:34:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 28 Dec 2019 18:34:32 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 28 Dec 2019 18:35:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:35:40 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 18:35:41 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Dec 2019 18:36:03 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Dec 2019 18:36:04 GMT
ENV ROS_DISTRO=melodic
# Sat, 28 Dec 2019 18:38:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:39:00 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 28 Dec 2019 18:39:01 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Dec 2019 18:39:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facfbd1fae886a379926b7add3095adbf575d32e87e67282e12488332f12f747`  
		Last Modified: Sat, 28 Dec 2019 18:48:28 GMT  
		Size: 9.8 MB (9774604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a6b709bed6b18e5ba839847d0f3e3a5a4e53a163b69ea7858c561fdc7f1e3a`  
		Last Modified: Sat, 28 Dec 2019 18:48:25 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9a8179e95515f1f6e62a300ca75906566906d949c7403c9f61b8511afc033`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b6ea616f3e8e138683f48ca757b84bc23de865b250839eba047a141cc6721`  
		Last Modified: Sat, 28 Dec 2019 18:48:46 GMT  
		Size: 62.1 MB (62085764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101b4656b4d26f6236d97a86a31ae20834b113b525d2830521853323cfb6369`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 451.5 KB (451514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5e52b33734a366437f8b9e807980e3273684eeef72d2fd1822dc4ea7ae5638`  
		Last Modified: Sat, 28 Dec 2019 18:49:32 GMT  
		Size: 224.6 MB (224573326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de7b9c0321a0098bd333b1ceb564c2a4389249dc4f9e3f45da7c389198a1ba`  
		Last Modified: Sat, 28 Dec 2019 18:48:24 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
