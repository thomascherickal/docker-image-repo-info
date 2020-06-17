## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:0c3928d4743ded527f471714b7c8a86374362b20b892ccd0dcb8999b00d7bd75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:90a5fb536a6e627e4f2e5cc66d204c5c12a0e5c79fa01e097b234fbba7a28a55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.7 MB (291680947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36f2c4f984c7ca201f30d80feb05faadd0d856b829f46c8ea6449bbb0fe8ce8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:20:29 GMT
ADD file:1e8d02626176dc8141df3c0a1365774ce73d79934654fe24a4b1e7f173108232 in / 
# Wed, 17 Jun 2020 01:20:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:20:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:20:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:20:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:14:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:27:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:27:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 05:27:26 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 05:27:26 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:27:27 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:27:27 GMT
ENV ROS_DISTRO=melodic
# Wed, 17 Jun 2020 05:30:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:30:21 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 05:30:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:30:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d7c3167c320d7a820935f54cf4290890ea19567da496ecf774e8773b35d5f065`  
		Last Modified: Wed, 27 May 2020 12:21:15 GMT  
		Size: 26.7 MB (26688718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131f805ec7fd68d45a887e2ef82de61de0247b4eb934ab03b7c933650e854baa`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 35.4 KB (35369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322ed380e680a77f30528ba013e3a802a7b44948a0609c7d1d732dd46a9a310d`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac240b130982ad1c3ba3188abbf18ba4e54bdd9e504ce2d5c2eff6d3e86b8dd`  
		Last Modified: Wed, 17 Jun 2020 01:21:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64a7083ea96b95855d3cee6bcab14b90b20d9bfd209d123ecb0caa88322c7ae`  
		Last Modified: Wed, 17 Jun 2020 03:31:48 GMT  
		Size: 837.6 KB (837600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc602a4d0af8ead24cc13540f49a0fff8887a95b19f7167d71c673468d08954e`  
		Last Modified: Wed, 17 Jun 2020 06:03:08 GMT  
		Size: 4.9 MB (4867669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13ebfa6253ab146de4b680f495660841c32931dfc6640051a14000c8c18ac49`  
		Last Modified: Wed, 17 Jun 2020 06:03:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e357f79e762b301a72bfc29c53b477116db00825dab096e69c4b22309aa72edf`  
		Last Modified: Wed, 17 Jun 2020 06:03:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4426cc1b5ab808a5916e33dd02e4b7bd626d04ee88a6f0020db75bf20ab8eaba`  
		Last Modified: Wed, 17 Jun 2020 06:03:58 GMT  
		Size: 259.2 MB (259248746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c6421f726415d8084d253ffe8760cd196ebc9e5488080af5b60e09a1bd388c`  
		Last Modified: Wed, 17 Jun 2020 06:03:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:5633e7fb9c240c5b7d46d4ae1dd326f14501b942f56ad3eb0868f2eb6f6341f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265970257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd0f2d436a5fd84a54ea25ca354e258417a02f781fb2cb08950834afca71f64`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 02:02:00 GMT
ADD file:579f3bbed274bd8ec97aa5bfc4eb09fdcfe3e12e37fb3739f3096138b765581c in / 
# Wed, 17 Jun 2020 02:02:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 02:02:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 02:02:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 02:02:09 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:20:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:20:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:21:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:21:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:21:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:21:04 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:21:05 GMT
ENV ROS_DISTRO=melodic
# Wed, 17 Jun 2020 03:24:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:24:28 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 03:24:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:24:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2d63ac53d1bca136340c80fe8b64c0b8e2d9a62eddb6fcb794c489840dc027d6`  
		Last Modified: Sat, 30 May 2020 09:27:47 GMT  
		Size: 22.3 MB (22275987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e03e3a8e7321c64d7a483fc9cc0054ce81e5b230b32300b7c68d21001f661a`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 35.5 KB (35459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0e8090890c513488a0f67683f23dcfcfbf2b67e5be854edf1323ad87a60b26`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b801ccb19e43939aa60383f674f0e1f65ab062890870d42d0fa7a7a62fc5b708`  
		Last Modified: Wed, 17 Jun 2020 02:05:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd193992630ce3c05616b2d6384bc7261c04210de22ad6879778b9aca67aaa81`  
		Last Modified: Wed, 17 Jun 2020 03:55:51 GMT  
		Size: 838.2 KB (838177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a62e43a84ad9c1d846a6d034c6ec80467b2e21c620fd37591f04eba4cdb0c01`  
		Last Modified: Wed, 17 Jun 2020 03:55:49 GMT  
		Size: 4.1 MB (4083577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76400ef72b32df9a8e2460f1a21fdf6afb134ef4aa07c8141f7bb89eb6dcff9c`  
		Last Modified: Wed, 17 Jun 2020 03:55:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a72f5b0368ec63ae50fd9b88d2d9327d6a43fa47fadbad4ba783fa8b2f89d`  
		Last Modified: Wed, 17 Jun 2020 03:55:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39eace094cd15bc078328e4182a5ba21e23c56fe73131f5dfde1840d01e446b`  
		Last Modified: Wed, 17 Jun 2020 03:57:05 GMT  
		Size: 238.7 MB (238734177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cc894cd279dd9a2a095c4c2eb5717ad09ac5e1c26f29112e1c8238a26e25ba`  
		Last Modified: Wed, 17 Jun 2020 03:55:48 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e37ae0b2cd64c71d61404ff303c770235dabe5a927a578fdcda77ce495b2a761
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281263784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb1a5c6604e7c5f96492cdcf74072ba959f36a18f9baaad962a6e1edea202f8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:46:41 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Jun 2020 03:47:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Jun 2020 03:47:14 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:47:15 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:47:15 GMT
ENV ROS_DISTRO=melodic
# Wed, 17 Jun 2020 03:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:50:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Jun 2020 03:50:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:50:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fa5af0f7212815117da17900293ea522ed8cf971e727597f85ee658d8f8c1a`  
		Last Modified: Wed, 17 Jun 2020 04:36:48 GMT  
		Size: 838.3 KB (838254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bf6eb80e593e6f6e4ece6d710b03a4d7d8f378c1d6f2a1bef7a7b4c68009b3`  
		Last Modified: Wed, 17 Jun 2020 04:36:46 GMT  
		Size: 4.5 MB (4451304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ce79b03ccae069bcf39b72bb491ba542a576507093bcf66aaeaf82c94c1d8`  
		Last Modified: Wed, 17 Jun 2020 04:36:45 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319dd37aab02f6a817505d739ba55fae6d50a43ca603076fa863131ccd36107`  
		Last Modified: Wed, 17 Jun 2020 04:36:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6f2fe59de45e53d860bdbe6b09e207b2ce51f5859907b0768bf071a78193e`  
		Last Modified: Wed, 17 Jun 2020 04:37:52 GMT  
		Size: 252.2 MB (252214465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fde26335cfaf97f11e2339d3ab139f78cd24fd6df8c00514aa0b03faa24c4f`  
		Last Modified: Wed, 17 Jun 2020 04:36:46 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
