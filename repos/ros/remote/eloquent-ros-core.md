## `ros:eloquent-ros-core`

```console
$ docker pull ros@sha256:fa39348b27a14496afbcfa1ca30446789240130e992bf3ca66476f35dbc5142e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:eloquent-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:e82a6926198b7dae2a1cb886ed7fda20bb30c3984a1c5cb3d4cf8a2cc71e8e49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215392714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002e2bfd6abc385e5787ef6c7c8befd0353376792d7e5ad7b9aae05410cf88a`
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
# Wed, 17 Jun 2020 05:48:08 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 05:48:08 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 05:48:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 05:53:44 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 05:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 05:54:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 05:54:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 05:54:48 GMT
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
	-	`sha256:e22b4d4694e78be7232b3d308841e35b90c3f15975115584463ca3eb734f81b5`  
		Last Modified: Wed, 17 Jun 2020 06:08:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dbba4e323e93c2e7319117cf60d51465bef774f27ea2e8be04a1a4920e5a1b`  
		Last Modified: Wed, 17 Jun 2020 06:11:23 GMT  
		Size: 183.0 MB (182960509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e559b1e43395acc7e375c1e56941c4b220d965384f03fda5576b0aa99734c`  
		Last Modified: Wed, 17 Jun 2020 06:10:44 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:054213832517df926388b0747fccb6e53ae16806593d0868c7ad92a8c93a64a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183814766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21346975565a74840c4e2b48867933effc988be3d084bb6fca0966ad466ac6b`
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
# Wed, 17 Jun 2020 03:34:14 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 03:34:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 03:34:17 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 03:44:25 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 03:47:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:47:11 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 03:47:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 03:47:14 GMT
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
	-	`sha256:918fdc185d3fb3945554b26f476ae406a19ce7616be5e247ed94bf07f74d446e`  
		Last Modified: Wed, 17 Jun 2020 03:59:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa41bff48ade208264d42231471d8f6e03dcb6d4d122a9a1b5263314090c468`  
		Last Modified: Wed, 17 Jun 2020 04:02:16 GMT  
		Size: 156.6 MB (156578683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e295d701386a1ca525f379d6ffd7cc280ed098c98c41f9f2fc37595942585`  
		Last Modified: Wed, 17 Jun 2020 04:01:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:eloquent-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:71e9a8facbe2f4af2cfa70fe42b424e5973d4bacf44933abc21da153ed6da2cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.4 MB (197400382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef12a224b0f14aeb1e450c05aaaf358ed367dac50d6831ccf5da989d878da1f9`
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
# Wed, 17 Jun 2020 04:08:37 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu bionic main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 17 Jun 2020 04:08:37 GMT
ENV LANG=C.UTF-8
# Wed, 17 Jun 2020 04:08:38 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Jun 2020 04:17:00 GMT
ENV ROS_DISTRO=eloquent
# Wed, 17 Jun 2020 04:19:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-eloquent-ros-core=0.8.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 04:19:57 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 17 Jun 2020 04:19:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Jun 2020 04:19:59 GMT
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
	-	`sha256:9b2865f2c14406dc3fd3434efdbcb197cb35e58ae34baddd5311196da42e6b8f`  
		Last Modified: Wed, 17 Jun 2020 04:44:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24244156a34df6d325502e451abab9668b3accc6f7f8270c8d733c9649a58f01`  
		Last Modified: Wed, 17 Jun 2020 04:47:12 GMT  
		Size: 168.4 MB (168351060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed77c1acf2662e22120674aea71547c6c7697480aabe1bf3b2c6d16c7a7c3c0`  
		Last Modified: Wed, 17 Jun 2020 04:46:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
