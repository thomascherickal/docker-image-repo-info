## `ros:foxy-ros-core`

```console
$ docker pull ros@sha256:653bae24febf4eaf082f3887f4a944631dc710773aae0b84c1bd2dd335238211
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ff73d0c1178914c7e2b09086031bbac7d898e069f320e5913681d5a9f8cdce93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155244012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f689a2db8436e9e33695e0bb66608cc9e5b92b2885b9073d99d8baa063b9dac5`
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

### `ros:foxy-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2610a6cf9e55366a1e3fe7e27d5137f3983a9c72c7a13815a5da52e8dd140801
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137986560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ebf4b2c4bb0d9fc8a26ce826b3168f49e24fe1c85511ee3cb61cfb7c503d573`
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
