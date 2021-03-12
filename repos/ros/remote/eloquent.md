## `ros:eloquent`

```console
$ docker pull ros@sha256:c20b1d3dce59d113f8b79401e663c64032e21f2c1ac8a605c56471e1d5a7dbb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent` - linux; amd64

```console
$ docker pull ros@sha256:3b4c524b7af3b34909c36d928044bb599b6b998e608a1bbd88dd63e33c0d5393
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.8 MB (283760634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8af65fbdcd3ec748f7c03346ca555ff1d13a6cf71e34a2f5c1effd24ca719a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 09:43:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:49:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:49:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 12 Mar 2021 14:34:35 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 12 Mar 2021 14:34:36 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 14:34:36 GMT
ENV LC_ALL=C.UTF-8
# Fri, 12 Mar 2021 14:42:38 GMT
ENV ROS_DISTRO=eloquent
# Fri, 12 Mar 2021 14:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:44:02 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 12 Mar 2021 14:44:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 12 Mar 2021 14:44:02 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 14:44:38 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 14:44:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 12 Mar 2021 14:44:48 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 12 Mar 2021 14:44:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ed3fdd01cb132a75576627b585cbad41af7070332373601bf156cf4196736`  
		Last Modified: Fri, 12 Mar 2021 10:19:48 GMT  
		Size: 841.3 KB (841338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e14253e5e1988d1da318161fcd62f7283c85a895d3290c387f20568717ed1a`  
		Last Modified: Fri, 12 Mar 2021 15:02:27 GMT  
		Size: 4.9 MB (4872989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72cfe4cc8a334266cf329ea82265f2fd5aba02064102886f265705a681ccdb1`  
		Last Modified: Fri, 12 Mar 2021 15:02:25 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e32e6704570881b3a6cdc732b74410b5febf79730e8b2a908e20461a4fbbb`  
		Last Modified: Fri, 12 Mar 2021 15:17:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ef4d5648b0285a36972e35d689cb35b4efbcab7742ce860d24ca2511545601`  
		Last Modified: Fri, 12 Mar 2021 15:20:14 GMT  
		Size: 183.0 MB (183011787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759770b0831d0f3cc47795131ca2bddafee77b35116da0548b9c981236279222`  
		Last Modified: Fri, 12 Mar 2021 15:19:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bab687d7eca7e18125d2a6b895957f563b27f5445360be29270d2c55cfba3c`  
		Last Modified: Fri, 12 Mar 2021 15:20:37 GMT  
		Size: 63.5 MB (63528696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867df2c69103cf8ea59f19f295afab2782741e2ebcfef18e1021e80528e12dc7`  
		Last Modified: Fri, 12 Mar 2021 15:20:27 GMT  
		Size: 201.8 KB (201793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae0d1e977c08796af89cfd7c7b00440aafb1a52be96f99f959145d07d0f9725`  
		Last Modified: Fri, 12 Mar 2021 15:20:26 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e601e15c1a6c49581f10fac5afae3db9175b87ff54deeb929461939dd986c75c`  
		Last Modified: Fri, 12 Mar 2021 15:20:27 GMT  
		Size: 4.6 MB (4588978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm variant v7

```console
$ docker pull ros@sha256:f6fff9c0b7907f7a6fb03ed749a29d30345a33c329cb2fbc0a903a2755768ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235451443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b234f321dcf076ba15747299838eee178aa5920431fd1af1da2c18fd2b49db98`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 03:11:28 GMT
ADD file:40381fcd77266e4b2259c02af63359b9cff79b4908e5f800f2b3cb9c555e092c in / 
# Thu, 04 Mar 2021 03:11:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 03:11:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 03:11:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 03:11:35 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:03:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:03:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:03:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 04:24:58 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 04 Mar 2021 04:24:59 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 04:25:00 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 04:32:24 GMT
ENV ROS_DISTRO=eloquent
# Thu, 04 Mar 2021 04:34:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:34:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 04 Mar 2021 04:34:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 04:34:49 GMT
CMD ["bash"]
# Thu, 04 Mar 2021 04:35:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:35:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 04 Mar 2021 04:35:54 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 04 Mar 2021 04:36:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ac910c0311f3581d0d4d512d5b9cb75f3cb4ac0ac05c27d5afe506d19ede5a4`  
		Last Modified: Mon, 01 Mar 2021 16:09:58 GMT  
		Size: 22.3 MB (22290308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b89a6b5bccf38a10ff30cb0b414a7e2dec5567d954850dfb98d67977e13fc38`  
		Last Modified: Thu, 04 Mar 2021 03:13:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36058ccabae5f30074009cee645af7e052db260738cc0bc08ec9386b0f8cf37e`  
		Last Modified: Thu, 04 Mar 2021 03:13:18 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055861ede19fe8606dca16da2271075d5d46ad1234acc782d134f1c941be2c72`  
		Last Modified: Thu, 04 Mar 2021 04:40:54 GMT  
		Size: 841.1 KB (841118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6fbf11975e6d976397a06700430b7ac889c14444fc7ad18a7be40983d9d468`  
		Last Modified: Thu, 04 Mar 2021 04:40:53 GMT  
		Size: 4.1 MB (4085567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e165c7fe50b6918ba96d9a80c7d25887947ae8b8aa8fd70fe773e79a745dff1b`  
		Last Modified: Thu, 04 Mar 2021 04:40:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cced3fb2c3ab38fac875c419ff81df8ddcc53b538cb2f9094df0e2f8de49339a`  
		Last Modified: Thu, 04 Mar 2021 04:48:28 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610ebe712acc613ed4684f809c031e5f92683905e6428dc3ab5868576d14485`  
		Last Modified: Thu, 04 Mar 2021 04:51:12 GMT  
		Size: 156.6 MB (156616799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81655ee6f1bdd57ccd4505d3859ab7e34e47f585c4ea4de7dbca1866600a40ee`  
		Last Modified: Thu, 04 Mar 2021 04:50:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9972e48fe8245a8298189943a2fdee353bb8bf0ca7d4c6a8e13336953ed4036a`  
		Last Modified: Thu, 04 Mar 2021 04:51:37 GMT  
		Size: 47.9 MB (47914711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db555332ef59faf7be7da641813c3345005466ebd8e9ae75aea20547e48b881`  
		Last Modified: Thu, 04 Mar 2021 04:51:25 GMT  
		Size: 201.7 KB (201677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf16d393b823c78b15cfc51130e23ad305e2b4a4166f575c2eaf0193458536b0`  
		Last Modified: Thu, 04 Mar 2021 04:51:25 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1034e7a69686363691522efd2fdf8e5c26fa416cd5250b53a23df2c558d2cc17`  
		Last Modified: Thu, 04 Mar 2021 04:51:26 GMT  
		Size: 3.5 MB (3496339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6cdfeb94c4afbc53e9990e86b918a70afc894dc4ffe268711aa4430ce691a631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.8 MB (257820981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53bbb5a6f661f3530e0fa2ca1ba23cd1e34a66d47e098d327103be4b9a78d97c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:12:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:13:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:13:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 04 Mar 2021 03:32:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 04 Mar 2021 03:32:27 GMT
ENV LANG=C.UTF-8
# Thu, 04 Mar 2021 03:32:28 GMT
ENV LC_ALL=C.UTF-8
# Thu, 04 Mar 2021 03:39:09 GMT
ENV ROS_DISTRO=eloquent
# Thu, 04 Mar 2021 03:41:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:41:26 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Thu, 04 Mar 2021 03:41:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 04 Mar 2021 03:41:29 GMT
CMD ["bash"]
# Thu, 04 Mar 2021 03:42:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:42:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 04 Mar 2021 03:42:44 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 04 Mar 2021 03:43:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-base=0.8.5-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb395c83b2a400ee825ab384f2c51674c732ff599742e127b5639756b0cc7a8b`  
		Last Modified: Thu, 04 Mar 2021 04:00:41 GMT  
		Size: 840.9 KB (840907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3418e9c274d60c6f142b25861afead56aafa5ece244d451cab264c52961bc618`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 4.5 MB (4453487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ee6263fb6dc4f04d5d149d5aa0d9932daea95f32e0478a12a5e66a986a1931`  
		Last Modified: Thu, 04 Mar 2021 04:00:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba1f39d246b743a36739f550b8be9d8c7d9eabc3ef41854beda836da5a2a313`  
		Last Modified: Thu, 04 Mar 2021 04:07:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce0ebfeb4d2e555323f5c06e4cb35d0d4c4ed1bc771dd6693499f5c1759d37`  
		Last Modified: Thu, 04 Mar 2021 04:10:29 GMT  
		Size: 168.4 MB (168425669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa1bde67253b6384c49fc47b08dfbf5a701284a6f173e3b5c0db2e0226e87b`  
		Last Modified: Thu, 04 Mar 2021 04:09:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff496571ec081faf7c4d5caeb40984e7c77ad7b14f21c20cac20cc94b3b1ced`  
		Last Modified: Thu, 04 Mar 2021 04:10:51 GMT  
		Size: 56.2 MB (56227443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35b9da9925b4002ad595d3a955ee82f9dc2798259f31f2dc8f84676f1e10355`  
		Last Modified: Thu, 04 Mar 2021 04:10:36 GMT  
		Size: 201.7 KB (201679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60ca71c09c1715d7d1bb735e03591cea0530693ac6e7484eecfc1afc171614`  
		Last Modified: Thu, 04 Mar 2021 04:10:36 GMT  
		Size: 2.0 KB (2036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265b99736ec68040007fc9e8cb5649c8d4320061e66e6d0e9cd6dabfaa0088b7`  
		Last Modified: Thu, 04 Mar 2021 04:10:38 GMT  
		Size: 3.9 MB (3934828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
