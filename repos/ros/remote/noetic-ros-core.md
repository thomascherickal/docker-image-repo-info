## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:4849cd61f6b48dfaef445bd11da21e238f6f7d58df31129c17a7a617c97ae172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:44180155f2353309dcbca40df53b3cf1e5c0397c9b4343ccbfa3cde9c7d78102
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.8 MB (208823685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6dc7028366dda0ba1fd93f30c3f7b73525ae0858536b1ee9caddfc1f07be10`
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
# Thu, 03 Jun 2021 18:21:49 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 03 Jun 2021 18:21:51 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 03 Jun 2021 18:21:51 GMT
ENV LANG=C.UTF-8
# Thu, 03 Jun 2021 18:21:51 GMT
ENV LC_ALL=C.UTF-8
# Thu, 03 Jun 2021 18:21:51 GMT
ENV ROS_DISTRO=noetic
# Thu, 03 Jun 2021 18:23:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:23:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 03 Jun 2021 18:23:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 03 Jun 2021 18:23:35 GMT
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
	-	`sha256:856beeab8b0c0cb01ff1528910349b59189125f214a7f20d92f531a73a70e903`  
		Last Modified: Thu, 03 Jun 2021 18:38:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b6ec483f8f5e426c9ae3693f45bfce53ea1238328d23b1e1c60ba0c12cf731`  
		Last Modified: Thu, 03 Jun 2021 18:38:58 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f282b871b45df91e76adff32df10e1b98066d3976be845be2718241f10104f`  
		Last Modified: Thu, 03 Jun 2021 18:39:30 GMT  
		Size: 173.5 MB (173548349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619ea56a04e708c30f77546baa92406060e4a5cdd994e462fa7243b9f4aa10a9`  
		Last Modified: Thu, 03 Jun 2021 18:38:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:28a324e01144630b93aeff09eac5d269bc0ab5f7972bf4e05b5ac6e01b4dbedd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187129882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72d2ae964eb75cd7f62011efa40465869133d26992a4d10e8734b683b7dfd16e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 May 2021 17:00:36 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Wed, 26 May 2021 17:00:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 17:00:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 17:00:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 17:00:38 GMT
CMD ["/bin/bash"]
# Thu, 27 May 2021 00:05:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:05:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:23:51 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 03 Jun 2021 18:23:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 03 Jun 2021 18:23:52 GMT
ENV LANG=C.UTF-8
# Thu, 03 Jun 2021 18:23:53 GMT
ENV LC_ALL=C.UTF-8
# Thu, 03 Jun 2021 18:23:53 GMT
ENV ROS_DISTRO=noetic
# Thu, 03 Jun 2021 18:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:24:50 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 03 Jun 2021 18:24:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 03 Jun 2021 18:24:50 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d9a278ae85c6e20b2a660aec6ce81a669bf95f4bcc1f342352c4bcd340f086`  
		Last Modified: Wed, 26 May 2021 17:03:21 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5bd319502444cd19bef903c9880fd79e6a3e4992ce96feea91b56600320b0a`  
		Last Modified: Wed, 26 May 2021 17:03:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944fd4ab8f3cfc07b27885e5b3c0da643c62e1a8b62f017ac6866dfce12d87d6`  
		Last Modified: Thu, 27 May 2021 00:28:53 GMT  
		Size: 1.2 MB (1183201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00163d0e6cbc90b94fbbc0f937861d21102d23e965135395e7f3a45e8e65eed`  
		Last Modified: Thu, 27 May 2021 00:28:51 GMT  
		Size: 4.7 MB (4676239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba5b0ac5d30e15736c4262e462c42f3a073b4b861c714ccefc37af96dbdc53c`  
		Last Modified: Thu, 03 Jun 2021 18:30:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc9a52cbad0e7b4d3535ecf2227c680f4e36d73a38bb311d5a24bb6d72bc0f6`  
		Last Modified: Thu, 03 Jun 2021 18:30:57 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3cff19bc7c1a7b5145e8b28fecba31478e650cbc1a7484173fd6b197065fb5`  
		Last Modified: Thu, 03 Jun 2021 18:31:35 GMT  
		Size: 157.2 MB (157228443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e444d9f621e8655f5c00e6d4275b6e204126048e39f9d00e710590a1c8a1b`  
		Last Modified: Thu, 03 Jun 2021 18:30:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:13016ed381ad920512898aa5f6256377910e88349047440f65a406da11b7b369
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.7 MB (201681625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0beb93f54bab321e79ed3f1f5d47edb78414d6348afc3e35b0bb0a9ba09eca`
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
# Thu, 03 Jun 2021 18:41:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 03 Jun 2021 18:41:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 03 Jun 2021 18:41:56 GMT
ENV LANG=C.UTF-8
# Thu, 03 Jun 2021 18:41:56 GMT
ENV LC_ALL=C.UTF-8
# Thu, 03 Jun 2021 18:41:56 GMT
ENV ROS_DISTRO=noetic
# Thu, 03 Jun 2021 18:42:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Jun 2021 18:42:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 03 Jun 2021 18:42:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 03 Jun 2021 18:42:45 GMT
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
	-	`sha256:bb8c4a76a314725d5863a61d215ef4aea038563d3234153aa8e23ba1985db7db`  
		Last Modified: Thu, 03 Jun 2021 18:51:59 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8beb2dcf01b8c4f0900d357b7e3221b4fde947f523a857a6bd7a625c822a90aa`  
		Last Modified: Thu, 03 Jun 2021 18:51:59 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea966986035f5ff192931f524a571289133ffdbeb94fe41144ffa9c0d6745aa`  
		Last Modified: Thu, 03 Jun 2021 18:52:33 GMT  
		Size: 167.8 MB (167837691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357fdb284c5ceb936c9122007b13a340ea423020279546ac4ced95cde60b191`  
		Last Modified: Thu, 03 Jun 2021 18:52:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
