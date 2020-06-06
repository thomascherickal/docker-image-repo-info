## `ros:foxy-ros-core-focal`

```console
$ docker pull ros@sha256:51f43d86c94eb16adcd288b26f223f8061f8168e1d55df3f67f1b9a33d257cfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `ros:foxy-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fb9008a238d58643fbb9070c152c8fc0e1403a89004b2a97583328b451020fd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137361413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a191838183e06272e7df9b897f954aba876834a04b97590cadc2a650c5f279b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:18:16 GMT
ADD file:e9947aff2dfa8f220d4b25dc0770aff8d9ffc08482e52f54833f39e1c3ec08bf in / 
# Fri, 24 Apr 2020 00:18:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:18:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:18:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:18:29 GMT
CMD ["/bin/bash"]
# Wed, 27 May 2020 01:42:44 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 01:43:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 06 Jun 2020 00:42:37 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 06 Jun 2020 00:42:38 GMT
ENV LANG=C.UTF-8
# Sat, 06 Jun 2020 00:42:39 GMT
ENV LC_ALL=C.UTF-8
# Sat, 06 Jun 2020 00:42:40 GMT
ENV ROS_DISTRO=foxy
# Sat, 06 Jun 2020 00:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.1-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 06 Jun 2020 00:44:36 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 06 Jun 2020 00:44:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 06 Jun 2020 00:44:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6c2d76ba33f8d52087147ce28d8f03c08f69677591e3e10db810bf76a6e09427`  
		Last Modified: Fri, 24 Apr 2020 00:22:00 GMT  
		Size: 27.2 MB (27158644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d4cfc71d3821474946021fdbf241a74992a84c6269c3e9a052ce7fc56cece`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 32.3 KB (32326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63063bfe137200b3c8d1ee8d819124352c20ee8c189a0388f461ec66bb759310`  
		Last Modified: Fri, 24 Apr 2020 00:21:53 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38385900086ffa7d7cb9c3bbeabaf2176d7d7958ebf0736d2a01773a830201ee`  
		Last Modified: Fri, 24 Apr 2020 00:21:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee47658e5a2b6951b5c8f1df079e5f94fa5babfcb132843f7e89a21a531555f5`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 1.2 MB (1175483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b7e5841799d26c7c96bfbade1ef6d8be3e67adbbc8402a26e6a6cf491a849`  
		Last Modified: Wed, 27 May 2020 02:09:35 GMT  
		Size: 5.5 MB (5515489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079fbc9cd40b2782019694e3fdfea45d641b7cd63c3e41e193edc9581c050ee`  
		Last Modified: Wed, 27 May 2020 02:09:33 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3ec18d9d03c6ef880ba9e4caecbbfd50402843b4d260e38bf7d308700a606`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526f25ed5278e2e7a7fde79b21330117bd4b9e32b6b5232ae881703bdcd287aa`  
		Last Modified: Sat, 06 Jun 2020 00:47:30 GMT  
		Size: 103.5 MB (103476592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc209a31a5ea7c241b1c1de254415f9a26b41a629573e40f2deb838c76a0571`  
		Last Modified: Sat, 06 Jun 2020 00:46:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
