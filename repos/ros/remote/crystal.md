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
