## `ros:noetic-ros-core`

```console
$ docker pull ros@sha256:d4c1f95ad09bcfa86e61883d9f02ba18c57c39b377406f5474baec63445d2fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:c4307b48fbc5786cee96fd12e3b64fab0917daef9f4b394073df1e4c69145a2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208379951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bc82724f55445e5d7b02ae4e5a146bd6d499512e3ba55d5cccf2adc55399d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:34 GMT
ADD file:9f937f4889e7bf6467d34e7ac4f093054993a93399443dc7469d53750a62234f in / 
# Wed, 19 Aug 2020 21:14:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:39 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:56:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:10:57 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:10:58 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 20 Aug 2020 00:10:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 20 Aug 2020 00:10:59 GMT
ENV LANG=C.UTF-8
# Thu, 20 Aug 2020 00:10:59 GMT
ENV LC_ALL=C.UTF-8
# Thu, 20 Aug 2020 00:10:59 GMT
ENV ROS_DISTRO=noetic
# Thu, 20 Aug 2020 00:13:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 20 Aug 2020 00:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 20 Aug 2020 00:13:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:54ee1f796a1e650627269605cb8e6a596b77b324e6f0a1e4443dc41def0e58a6`  
		Last Modified: Wed, 29 Jul 2020 15:19:55 GMT  
		Size: 28.6 MB (28558017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bfea53ad120b47cea5488f0b8331e737a97b33003517b0bd05e83925b578f0`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d371e02073acecf750a166495a63358517af793de739a51b680c973fae8fb9`  
		Last Modified: Wed, 19 Aug 2020 21:16:55 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66c17bbf772fa072c280b10fe87bc999420042b5fce5b111db38b4fe7c40b49`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa557cc6371ecdf29da34fb9617bb250fff91a99f8d09bd3b5f4ba454d5c4d8b`  
		Last Modified: Wed, 19 Aug 2020 23:11:16 GMT  
		Size: 1.2 MB (1175798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d14d67fb1371eab29e8b3ebd3cc38806d01da3fe7d7dacf2ee8fe215c2f74b`  
		Last Modified: Thu, 20 Aug 2020 00:42:13 GMT  
		Size: 5.5 MB (5546328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f0cb43f8f135cf525d89b3ea013f7c5b7c19e56d68b80ca9c9473ad7f98f2`  
		Last Modified: Thu, 20 Aug 2020 00:42:11 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1535741ea4a953a7ea47c7ced196baa4cf6ef8d3122d004c004b977b8535d58`  
		Last Modified: Thu, 20 Aug 2020 00:42:11 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e241e09adea6c38601f73735da1202dc34df0517fcb6c9c3a30658f4a16df23`  
		Last Modified: Thu, 20 Aug 2020 00:42:56 GMT  
		Size: 173.1 MB (173064631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5c25c62e4696ba3ec76c6c045700b916aecb922b18e2358e203b0c2df831c6`  
		Last Modified: Thu, 20 Aug 2020 00:42:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:fc59e886730cd825496485547bbf7d3f8bd5e27641555a4a535782f48aeeee96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.9 MB (186868537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5365926ae398188ffb26f7e008e81e440efbae6467787daabf3b604d3ea55e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Sep 2020 22:28:57 GMT
ADD file:ce07e6476bcfebee9c9ae22fe9e7881c3b6edcc56157604c6c55ced644f539c5 in / 
# Wed, 16 Sep 2020 22:28:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:29:01 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:29:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:29:04 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:50:36 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:50:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:50:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 16 Sep 2020 23:51:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 16 Sep 2020 23:51:06 GMT
ENV LANG=C.UTF-8
# Wed, 16 Sep 2020 23:51:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 Sep 2020 23:51:08 GMT
ENV ROS_DISTRO=noetic
# Wed, 16 Sep 2020 23:53:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:53:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 16 Sep 2020 23:53:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 16 Sep 2020 23:53:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c0b9d1d819e14fc43d183c6c727578dacab2a0ab57acc8f7eb1b773461fa00d8`  
		Last Modified: Wed, 16 Sep 2020 22:30:51 GMT  
		Size: 24.0 MB (24037417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d52142459eedcf7b55ad3755a75a1dd79a073f17d8c501c00651238a08915`  
		Last Modified: Wed, 16 Sep 2020 22:30:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8ca4f0a4d118843f1302740eace8e6c9d535e2840ae7cd1f09487b313ac810`  
		Last Modified: Wed, 16 Sep 2020 22:30:45 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24476fde0be6095639699705946f8dba94931a619fb0792ad19d9a9e46b40fb2`  
		Last Modified: Thu, 17 Sep 2020 00:24:41 GMT  
		Size: 1.2 MB (1177744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3093654782f4c282d0a8f8818bb8de76156c1c3118cf9471785d0df83b368`  
		Last Modified: Thu, 17 Sep 2020 00:24:40 GMT  
		Size: 4.7 MB (4676133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e5e6cd77111d0a439f5c23ae663ef960b63276d74d8dce3c7f309b3ead5b6`  
		Last Modified: Thu, 17 Sep 2020 00:24:39 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe20ad7fe1e9f4600161aa90611b0e5b5ae7cf5b643b9c59c468df529a3e30c9`  
		Last Modified: Thu, 17 Sep 2020 00:24:39 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7be5debb43675263045066ec61b1261ffde8e84fc0dc3411ab2d9ea0490b6d`  
		Last Modified: Thu, 17 Sep 2020 00:25:35 GMT  
		Size: 157.0 MB (156974372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a15e2daa5ef016de5f07d6d7b548fe8897f1753b48c6971a33ec32a89b638a7`  
		Last Modified: Thu, 17 Sep 2020 00:24:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a1f4f783bca1d11084f6ab3a200a2b582cb27cfbf5133b04bef12eeb4c9f189f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201418264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4336252e1133d95bdfa54e578d49e0bbe56a4990ba533cbf71f1171d614398c3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:30:23 GMT
ADD file:a332d170aaa2d4c28c85289b62d33de68027ce4d6b0616292ee2252dfdf2628b in / 
# Wed, 19 Aug 2020 21:30:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:30:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:30:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:30:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:24:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:25:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 19 Aug 2020 23:25:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 19 Aug 2020 23:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 19 Aug 2020 23:25:08 GMT
ENV LC_ALL=C.UTF-8
# Wed, 19 Aug 2020 23:25:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 19 Aug 2020 23:26:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:27:04 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 19 Aug 2020 23:27:05 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:61ca5746b6ffb91caaaa0eb4b9678ae147ad24bd40ac203758a90af376976f98`  
		Last Modified: Wed, 29 Jul 2020 08:25:33 GMT  
		Size: 27.2 MB (27162745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d07cd4558d7ea5ba152468ba362cbf62a56cfab14976467187d3943013a932`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 32.3 KB (32335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ef536d7ca531a0dce4a70ac7ad7d9b7ed27c56c7f0953bbec370e4299b951`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d5c7c4a6e93095601576a7663dde336974f6a96329ae2a613511662ed8744`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4083e46f11503c80095b52102ecdb34f1f88359ab6776daee0f399dd71c60372`  
		Last Modified: Thu, 20 Aug 2020 00:11:52 GMT  
		Size: 1.2 MB (1176161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7764603dd05c49038a524211ad7ceb67d2670cab2505beea1af401cca1e779`  
		Last Modified: Thu, 20 Aug 2020 00:11:48 GMT  
		Size: 5.5 MB (5511900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036f7ca74d2d186cd0993ac4fc4b9cef66c4777f93b40d28474a8e487429514f`  
		Last Modified: Thu, 20 Aug 2020 00:11:47 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f4e729660f1f0fbe6d83689811a5451fad053330c1e0b55ef6342e94717c9e`  
		Last Modified: Thu, 20 Aug 2020 00:11:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8c5132be159829ca825ced79895fd329bc9f13ce1b95a7cd45b86ba2fafef1`  
		Last Modified: Thu, 20 Aug 2020 00:13:11 GMT  
		Size: 167.5 MB (167532251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9bc6d8a25c406921c7218c11379caf00341a5f0c2e57351ac166de7421343`  
		Last Modified: Thu, 20 Aug 2020 00:11:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
