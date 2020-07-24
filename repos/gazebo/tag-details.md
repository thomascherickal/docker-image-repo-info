<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `gazebo`

-	[`gazebo:gzserver10`](#gazebogzserver10)
-	[`gazebo:gzserver10-bionic`](#gazebogzserver10-bionic)
-	[`gazebo:gzserver11`](#gazebogzserver11)
-	[`gazebo:gzserver11-bionic`](#gazebogzserver11-bionic)
-	[`gazebo:gzserver11-focal`](#gazebogzserver11-focal)
-	[`gazebo:gzserver7`](#gazebogzserver7)
-	[`gazebo:gzserver7-xenial`](#gazebogzserver7-xenial)
-	[`gazebo:gzserver9`](#gazebogzserver9)
-	[`gazebo:gzserver9-bionic`](#gazebogzserver9-bionic)
-	[`gazebo:gzserver9-stretch`](#gazebogzserver9-stretch)
-	[`gazebo:gzserver9-xenial`](#gazebogzserver9-xenial)
-	[`gazebo:latest`](#gazebolatest)
-	[`gazebo:libgazebo10`](#gazebolibgazebo10)
-	[`gazebo:libgazebo10-bionic`](#gazebolibgazebo10-bionic)
-	[`gazebo:libgazebo11`](#gazebolibgazebo11)
-	[`gazebo:libgazebo11-bionic`](#gazebolibgazebo11-bionic)
-	[`gazebo:libgazebo11-focal`](#gazebolibgazebo11-focal)
-	[`gazebo:libgazebo7`](#gazebolibgazebo7)
-	[`gazebo:libgazebo7-xenial`](#gazebolibgazebo7-xenial)
-	[`gazebo:libgazebo9`](#gazebolibgazebo9)
-	[`gazebo:libgazebo9-bionic`](#gazebolibgazebo9-bionic)
-	[`gazebo:libgazebo9-stretch`](#gazebolibgazebo9-stretch)
-	[`gazebo:libgazebo9-xenial`](#gazebolibgazebo9-xenial)

## `gazebo:gzserver10`

```console
$ docker pull gazebo@sha256:d058162b2cfe6b009a7d043a1be00b64cd3065379fe47c987248acce5b10ccb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10` - linux; amd64

```console
$ docker pull gazebo@sha256:5935c13ecaf46f4a53d22e96f49c5d900386ff6edd2516e26f3fd9258ac5e005
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268356786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95eb67fd427b52dbef7bf5aecd17b1ed31f9f1271df6d5b90bd8ae289626801d`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:50:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:50:22 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:50:22 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:50:22 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:50:22 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2136304acc7b103065d44fc33a16d51321855ce86883acc7ee0344a50a65ea`  
		Last Modified: Fri, 24 Jul 2020 16:07:00 GMT  
		Size: 226.1 MB (226083084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf286a152c343615b29996621748404ca473e9a2f131f56c1af01318b2b8c80a`  
		Last Modified: Fri, 24 Jul 2020 16:06:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver10-bionic`

```console
$ docker pull gazebo@sha256:d058162b2cfe6b009a7d043a1be00b64cd3065379fe47c987248acce5b10ccb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:5935c13ecaf46f4a53d22e96f49c5d900386ff6edd2516e26f3fd9258ac5e005
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268356786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95eb67fd427b52dbef7bf5aecd17b1ed31f9f1271df6d5b90bd8ae289626801d`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:50:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:50:22 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:50:22 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:50:22 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:50:22 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2136304acc7b103065d44fc33a16d51321855ce86883acc7ee0344a50a65ea`  
		Last Modified: Fri, 24 Jul 2020 16:07:00 GMT  
		Size: 226.1 MB (226083084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf286a152c343615b29996621748404ca473e9a2f131f56c1af01318b2b8c80a`  
		Last Modified: Fri, 24 Jul 2020 16:06:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:d9fbce31a88883cf385982fb4330514ec34ac98d051858c514a6f00e9ef83baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:60bddfe1e234c434ed4aefc7cf52c6926d7d53a7c0eed130e0c2df437cb78c9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.1 MB (305113451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e56f18de5a4eccf8bd60894691d763321dd06265b7fb7976642174e97c956`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:55:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:57:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:57:56 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:57:57 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:57:57 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:57:57 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2d7723dd72e12ca83677461008088ab189b85e21729ed2df2106aeb8ceb5`  
		Last Modified: Fri, 24 Jul 2020 16:09:41 GMT  
		Size: 16.1 MB (16116617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae815d31d793deb6003ddfe8440a24aba86ed48affc5cf7c0ba7ea2f43897f8`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d0bfc1d2a53af92118ace3ad3cc0966738e4a0efb82ed791a75ac8be2bcee`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 5.5 KB (5472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cf0ba06cf569fe44ed78e01cc74d1bdb746436f69c5f7ed9142fc4edec472`  
		Last Modified: Fri, 24 Jul 2020 16:10:15 GMT  
		Size: 259.2 MB (259222621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3a6a361742ab72ce4097ca8dfa8893ada08facb004f3d6bc7fe476b43bb0e6`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:0348c3b5165f06e2845a0006fe811f489e29fc865cc4fcc2109ed64123615389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:061f5bc815bb328945748023bd75638e130ef2f1992b2a83ae97326595e48fc5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269896187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c793c5d4e73b4068452fb2e7bffc8936ec96ce8210f9fb44b90c291aa8ee59`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:53:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:53:20 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:53:20 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:53:21 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:53:21 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d336f5ab998002a7fd27f7f97823a79da33db94abf32261ea0c04540821434bc`  
		Last Modified: Fri, 24 Jul 2020 16:08:35 GMT  
		Size: 227.6 MB (227622485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479035b2b323db88d46c9c942312551f91f9ddc329bb79cf9346cda8527bbe6e`  
		Last Modified: Fri, 24 Jul 2020 16:08:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11-focal`

```console
$ docker pull gazebo@sha256:d9fbce31a88883cf385982fb4330514ec34ac98d051858c514a6f00e9ef83baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:60bddfe1e234c434ed4aefc7cf52c6926d7d53a7c0eed130e0c2df437cb78c9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.1 MB (305113451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e56f18de5a4eccf8bd60894691d763321dd06265b7fb7976642174e97c956`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:55:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:57:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:57:56 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:57:57 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:57:57 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:57:57 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2d7723dd72e12ca83677461008088ab189b85e21729ed2df2106aeb8ceb5`  
		Last Modified: Fri, 24 Jul 2020 16:09:41 GMT  
		Size: 16.1 MB (16116617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae815d31d793deb6003ddfe8440a24aba86ed48affc5cf7c0ba7ea2f43897f8`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d0bfc1d2a53af92118ace3ad3cc0966738e4a0efb82ed791a75ac8be2bcee`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 5.5 KB (5472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cf0ba06cf569fe44ed78e01cc74d1bdb746436f69c5f7ed9142fc4edec472`  
		Last Modified: Fri, 24 Jul 2020 16:10:15 GMT  
		Size: 259.2 MB (259222621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3a6a361742ab72ce4097ca8dfa8893ada08facb004f3d6bc7fe476b43bb0e6`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7`

```console
$ docker pull gazebo@sha256:b0808ed792a12f4cacebee76e9225e80158a0f81efb9b419ab94ab6bb84ef90a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7` - linux; amd64

```console
$ docker pull gazebo@sha256:e6a93c48d88695c2494fbeb4cd6ecaa35d775f8a42633b9083ff645c980fd436
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242335131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8add8ce57f2b03debff57ee7a361929a127143649db65ea827118622ca333afd`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:39:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:39:06 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:39:06 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:39:06 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:39:07 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565f7ba5a4480b9dbb73fbe9ef70a939fda13b0450b3f7bb388c24930812c4ba`  
		Last Modified: Fri, 24 Jul 2020 16:02:25 GMT  
		Size: 181.6 MB (181636157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027827d3746e81be8ff2c5a4f4ce2d41188d09f1f79fdd74fea3a44908359a69`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7-xenial`

```console
$ docker pull gazebo@sha256:b0808ed792a12f4cacebee76e9225e80158a0f81efb9b419ab94ab6bb84ef90a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:e6a93c48d88695c2494fbeb4cd6ecaa35d775f8a42633b9083ff645c980fd436
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242335131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8add8ce57f2b03debff57ee7a361929a127143649db65ea827118622ca333afd`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:39:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:39:06 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:39:06 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:39:06 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:39:07 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565f7ba5a4480b9dbb73fbe9ef70a939fda13b0450b3f7bb388c24930812c4ba`  
		Last Modified: Fri, 24 Jul 2020 16:02:25 GMT  
		Size: 181.6 MB (181636157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027827d3746e81be8ff2c5a4f4ce2d41188d09f1f79fdd74fea3a44908359a69`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:198336d132193c706c2b3ad50354e0de78ed09e1104e36c781a58dbe571eec38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:64388ddd04d8ea97d01468dc45aa2781ff01834f857ed8832c97d851bd836d87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268365638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f59c41525ca8b27e0db0fc41e6e23e5747a4c9d874c59ab51c045c22272df62`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:46:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:46:54 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:46:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:46:55 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:46:55 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f0cacf50bd70ab4996e149569724c77cbb56990680917b81c3f89379426f60`  
		Last Modified: Fri, 24 Jul 2020 16:05:40 GMT  
		Size: 226.1 MB (226091936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c502d339a3332e46a90e7e477816d15337c6a2a520a0d52d899121aa4bafe7a2`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:198336d132193c706c2b3ad50354e0de78ed09e1104e36c781a58dbe571eec38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:64388ddd04d8ea97d01468dc45aa2781ff01834f857ed8832c97d851bd836d87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268365638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f59c41525ca8b27e0db0fc41e6e23e5747a4c9d874c59ab51c045c22272df62`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:46:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:46:54 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:46:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:46:55 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:46:55 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f0cacf50bd70ab4996e149569724c77cbb56990680917b81c3f89379426f60`  
		Last Modified: Fri, 24 Jul 2020 16:05:40 GMT  
		Size: 226.1 MB (226091936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c502d339a3332e46a90e7e477816d15337c6a2a520a0d52d899121aa4bafe7a2`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:4b670af9f10655501877e12cf0ba1409b90463851224b155f3f499aab9a8ad22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:cef5499d6759a861ec781da81c33138d462f73aecfd3964a3890f9609c5f2bc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.9 MB (265871238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd0cd38a912f0ba5e5ba98baf45bf5e08bb7fd13182662c688e3480cce0570`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Wed, 22 Jul 2020 20:07:30 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Jul 2020 10:23:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 10:23:49 GMT
EXPOSE 11345
# Thu, 23 Jul 2020 10:23:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Jul 2020 10:23:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Jul 2020 10:23:49 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4411483707592dcbac4314bc6194422b5b610683b5131926b750e3cbe20602`  
		Last Modified: Thu, 23 Jul 2020 10:28:29 GMT  
		Size: 18.5 MB (18514095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0dad0c2e98fc85f183e39744e915ce3092535269bc6dbad7a2c9c10f6db53b`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f94ffd189798ed034f2f550bfa7dc551f941f787e3d79b8e2a1d8b3e95e56`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11cdf511ee14cfb3e4d0d1f1d818a9c0697d7f1c26b2863d4e3150d10e4874`  
		Last Modified: Thu, 23 Jul 2020 10:28:52 GMT  
		Size: 202.0 MB (201980881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250ff4fbe3764f76e0b5c60de30521e67122cf9c39b8d5113e6c9755e1669435`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-xenial`

```console
$ docker pull gazebo@sha256:9ffecaa2f4b28746b3433e5dbcb217d67bcf18f627f9d88b6867fba4d08cdf37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:301788e72b63fab786640ccbfe3427ddf7861e6f3d2bd6e28f3efae9cdb6b902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.9 MB (268928201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417d2ecb062c87a8a6ca8c6bd6738eb3c2a3d895f27099f9fbe868b93a4626af`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:42:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:42:36 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:42:36 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:42:36 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:42:36 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba09bf0088affd311d90108b84c0a478a3f7f131f996f27358433f647758b669`  
		Last Modified: Fri, 24 Jul 2020 16:03:53 GMT  
		Size: 208.2 MB (208229225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7f21021ada008f3f0a02f1b4703dc12078c4a954562f101187c37767883f68`  
		Last Modified: Fri, 24 Jul 2020 16:03:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:latest`

```console
$ docker pull gazebo@sha256:34195d47629c894b00cb189e1ca90ab228826582697c601aaae1791c376aec22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:bbccff74f6feb6d74b15f8ad268ca9e62a9d15d4b33aff368143659dea77ac1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.1 MB (572065892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33f9f563386a6f85218580554738f06853b83b2a251b472925b43d1c90e696f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:55:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:57:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:57:56 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:57:57 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:57:57 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:57:57 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 16:01:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2d7723dd72e12ca83677461008088ab189b85e21729ed2df2106aeb8ceb5`  
		Last Modified: Fri, 24 Jul 2020 16:09:41 GMT  
		Size: 16.1 MB (16116617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae815d31d793deb6003ddfe8440a24aba86ed48affc5cf7c0ba7ea2f43897f8`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d0bfc1d2a53af92118ace3ad3cc0966738e4a0efb82ed791a75ac8be2bcee`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 5.5 KB (5472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cf0ba06cf569fe44ed78e01cc74d1bdb746436f69c5f7ed9142fc4edec472`  
		Last Modified: Fri, 24 Jul 2020 16:10:15 GMT  
		Size: 259.2 MB (259222621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3a6a361742ab72ce4097ca8dfa8893ada08facb004f3d6bc7fe476b43bb0e6`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0250f8e8cd6ce7a10de5e6f1df48e9ac114db403c09f407795889af5cb974263`  
		Last Modified: Fri, 24 Jul 2020 16:11:23 GMT  
		Size: 267.0 MB (266952441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10`

```console
$ docker pull gazebo@sha256:db1478a37bc14ea5d76c83463ae23ec93c58601e4284a4b9a827487a27faa9a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10` - linux; amd64

```console
$ docker pull gazebo@sha256:dc7c96b4439bb500e3957b7b95b4c4e5310a94ef32f02169f70f492ffe2c6bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.0 MB (521979186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc53cf75bff43c6b0b4b39c6ca871625ea5db85e1f3cb4d1ea24f8bf048df2d4`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:50:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:50:22 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:50:22 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:50:22 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:50:22 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2136304acc7b103065d44fc33a16d51321855ce86883acc7ee0344a50a65ea`  
		Last Modified: Fri, 24 Jul 2020 16:07:00 GMT  
		Size: 226.1 MB (226083084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf286a152c343615b29996621748404ca473e9a2f131f56c1af01318b2b8c80a`  
		Last Modified: Fri, 24 Jul 2020 16:06:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e2d9ff8a1ae3fa033bc7c2e7301a7590297c5a01c50eefa64cbe4f6921df3e`  
		Last Modified: Fri, 24 Jul 2020 16:07:57 GMT  
		Size: 253.6 MB (253622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10-bionic`

```console
$ docker pull gazebo@sha256:db1478a37bc14ea5d76c83463ae23ec93c58601e4284a4b9a827487a27faa9a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:dc7c96b4439bb500e3957b7b95b4c4e5310a94ef32f02169f70f492ffe2c6bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.0 MB (521979186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc53cf75bff43c6b0b4b39c6ca871625ea5db85e1f3cb4d1ea24f8bf048df2d4`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:50:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:50:22 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:50:22 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:50:22 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:50:22 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:52:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2136304acc7b103065d44fc33a16d51321855ce86883acc7ee0344a50a65ea`  
		Last Modified: Fri, 24 Jul 2020 16:07:00 GMT  
		Size: 226.1 MB (226083084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf286a152c343615b29996621748404ca473e9a2f131f56c1af01318b2b8c80a`  
		Last Modified: Fri, 24 Jul 2020 16:06:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e2d9ff8a1ae3fa033bc7c2e7301a7590297c5a01c50eefa64cbe4f6921df3e`  
		Last Modified: Fri, 24 Jul 2020 16:07:57 GMT  
		Size: 253.6 MB (253622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:34195d47629c894b00cb189e1ca90ab228826582697c601aaae1791c376aec22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:bbccff74f6feb6d74b15f8ad268ca9e62a9d15d4b33aff368143659dea77ac1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.1 MB (572065892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33f9f563386a6f85218580554738f06853b83b2a251b472925b43d1c90e696f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:55:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:57:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:57:56 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:57:57 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:57:57 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:57:57 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 16:01:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2d7723dd72e12ca83677461008088ab189b85e21729ed2df2106aeb8ceb5`  
		Last Modified: Fri, 24 Jul 2020 16:09:41 GMT  
		Size: 16.1 MB (16116617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae815d31d793deb6003ddfe8440a24aba86ed48affc5cf7c0ba7ea2f43897f8`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d0bfc1d2a53af92118ace3ad3cc0966738e4a0efb82ed791a75ac8be2bcee`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 5.5 KB (5472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cf0ba06cf569fe44ed78e01cc74d1bdb746436f69c5f7ed9142fc4edec472`  
		Last Modified: Fri, 24 Jul 2020 16:10:15 GMT  
		Size: 259.2 MB (259222621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3a6a361742ab72ce4097ca8dfa8893ada08facb004f3d6bc7fe476b43bb0e6`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0250f8e8cd6ce7a10de5e6f1df48e9ac114db403c09f407795889af5cb974263`  
		Last Modified: Fri, 24 Jul 2020 16:11:23 GMT  
		Size: 267.0 MB (266952441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:97e27d9f82e90d8fd5ca34a7a885e0aaaad1c748a17c5a8718ce31dea6acaef8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:180eb43b0f7da835adb11256efd8449349f027d6b1368bdb2aefd2c2f1238906
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531507725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef7e25d23a2b1f9aa9d7cd1e001927a4f148b307cd0f0cfd21345b5db51724af`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:53:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:53:20 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:53:20 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:53:21 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:53:21 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:54:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d336f5ab998002a7fd27f7f97823a79da33db94abf32261ea0c04540821434bc`  
		Last Modified: Fri, 24 Jul 2020 16:08:35 GMT  
		Size: 227.6 MB (227622485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479035b2b323db88d46c9c942312551f91f9ddc329bb79cf9346cda8527bbe6e`  
		Last Modified: Fri, 24 Jul 2020 16:08:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb199665193c7552b70e9b701641ee3821ea675406a285d9592bb0e079cb74b3`  
		Last Modified: Fri, 24 Jul 2020 16:09:32 GMT  
		Size: 261.6 MB (261611538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:34195d47629c894b00cb189e1ca90ab228826582697c601aaae1791c376aec22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:bbccff74f6feb6d74b15f8ad268ca9e62a9d15d4b33aff368143659dea77ac1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.1 MB (572065892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33f9f563386a6f85218580554738f06853b83b2a251b472925b43d1c90e696f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:55:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:55:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:55:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:57:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo11=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:57:56 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:57:57 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:57:57 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:57:57 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 16:01:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo11-dev=11.0.0-2*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d29a1172b44604004acb6860f11804dfd81393735d3d5c9849170f1e36b5`  
		Last Modified: Fri, 24 Jul 2020 16:09:39 GMT  
		Size: 1.2 MB (1176480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2d7723dd72e12ca83677461008088ab189b85e21729ed2df2106aeb8ceb5`  
		Last Modified: Fri, 24 Jul 2020 16:09:41 GMT  
		Size: 16.1 MB (16116617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae815d31d793deb6003ddfe8440a24aba86ed48affc5cf7c0ba7ea2f43897f8`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d0bfc1d2a53af92118ace3ad3cc0966738e4a0efb82ed791a75ac8be2bcee`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 5.5 KB (5472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cf0ba06cf569fe44ed78e01cc74d1bdb746436f69c5f7ed9142fc4edec472`  
		Last Modified: Fri, 24 Jul 2020 16:10:15 GMT  
		Size: 259.2 MB (259222621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3a6a361742ab72ce4097ca8dfa8893ada08facb004f3d6bc7fe476b43bb0e6`  
		Last Modified: Fri, 24 Jul 2020 16:09:37 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0250f8e8cd6ce7a10de5e6f1df48e9ac114db403c09f407795889af5cb974263`  
		Last Modified: Fri, 24 Jul 2020 16:11:23 GMT  
		Size: 267.0 MB (266952441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7`

```console
$ docker pull gazebo@sha256:e756786f9f8749e713aa59a0822bdc11c5c78346d49019cce63a200e4ce0fbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7` - linux; amd64

```console
$ docker pull gazebo@sha256:fd3a645e6b01c50d742bbe1420fab7448f00e67018a7acd8ab226b6d7cb2f603
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.7 MB (482737975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37f40f31c28a80be53033749db7619d2e7c22550aeb5dd1ff36f62a4c1cb912`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:39:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:39:06 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:39:06 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:39:06 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:39:07 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:41:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo7-dev=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565f7ba5a4480b9dbb73fbe9ef70a939fda13b0450b3f7bb388c24930812c4ba`  
		Last Modified: Fri, 24 Jul 2020 16:02:25 GMT  
		Size: 181.6 MB (181636157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027827d3746e81be8ff2c5a4f4ce2d41188d09f1f79fdd74fea3a44908359a69`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110ce4403e5fe7525016881f447f51e4df228dbcb2a750b0b1a1cf86cf92ac66`  
		Last Modified: Fri, 24 Jul 2020 16:03:19 GMT  
		Size: 240.4 MB (240402844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7-xenial`

```console
$ docker pull gazebo@sha256:e756786f9f8749e713aa59a0822bdc11c5c78346d49019cce63a200e4ce0fbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:fd3a645e6b01c50d742bbe1420fab7448f00e67018a7acd8ab226b6d7cb2f603
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.7 MB (482737975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37f40f31c28a80be53033749db7619d2e7c22550aeb5dd1ff36f62a4c1cb912`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:39:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:39:06 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:39:06 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:39:06 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:39:07 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:41:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo7-dev=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565f7ba5a4480b9dbb73fbe9ef70a939fda13b0450b3f7bb388c24930812c4ba`  
		Last Modified: Fri, 24 Jul 2020 16:02:25 GMT  
		Size: 181.6 MB (181636157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027827d3746e81be8ff2c5a4f4ce2d41188d09f1f79fdd74fea3a44908359a69`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110ce4403e5fe7525016881f447f51e4df228dbcb2a750b0b1a1cf86cf92ac66`  
		Last Modified: Fri, 24 Jul 2020 16:03:19 GMT  
		Size: 240.4 MB (240402844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:18fb9ec1275aacad1576192b8adf0d6b55793dfa751511869a32f8035fd0c70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:286e645bb0ac74867c1d902455e144ab5b56e00a6fc0ffb9e1f980e355209d0b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.5 MB (413466911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad2afb823b46e2206afe99d95a0397847bd65cccfb36e85163589f04e4c3e1b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:46:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:46:54 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:46:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:46:55 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:46:55 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:49:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f0cacf50bd70ab4996e149569724c77cbb56990680917b81c3f89379426f60`  
		Last Modified: Fri, 24 Jul 2020 16:05:40 GMT  
		Size: 226.1 MB (226091936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c502d339a3332e46a90e7e477816d15337c6a2a520a0d52d899121aa4bafe7a2`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbfde4c7d0e7b20c26672bbf31f444d7ffd54e9dfe527ef87ee29517857e3ce`  
		Last Modified: Fri, 24 Jul 2020 16:06:22 GMT  
		Size: 145.1 MB (145101273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-bionic`

```console
$ docker pull gazebo@sha256:18fb9ec1275aacad1576192b8adf0d6b55793dfa751511869a32f8035fd0c70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:286e645bb0ac74867c1d902455e144ab5b56e00a6fc0ffb9e1f980e355209d0b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.5 MB (413466911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad2afb823b46e2206afe99d95a0397847bd65cccfb36e85163589f04e4c3e1b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:44:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:44:44 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:44:45 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:46:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:46:54 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:46:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:46:55 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:46:55 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:49:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89062ead0c63c49ab543a80b545a2b3d1eeac6fe590f13f7ad88bc08dd47cd9`  
		Last Modified: Fri, 24 Jul 2020 16:05:09 GMT  
		Size: 837.9 KB (837870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc69889f3708bf175e814f9bdff1d20a21b0b3f71c7d71b9ed8db2bfdbce416`  
		Last Modified: Fri, 24 Jul 2020 16:05:10 GMT  
		Size: 14.7 MB (14695275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9257a9f3760eef737fb2f180510c9b78d6d13bfbe960a0e0149f489887365ec4`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0d875be951cc79b57471536899adefe285c4da6c6b32331edfb06c8e379558`  
		Last Modified: Fri, 24 Jul 2020 16:05:06 GMT  
		Size: 5.4 KB (5431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f0cacf50bd70ab4996e149569724c77cbb56990680917b81c3f89379426f60`  
		Last Modified: Fri, 24 Jul 2020 16:05:40 GMT  
		Size: 226.1 MB (226091936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c502d339a3332e46a90e7e477816d15337c6a2a520a0d52d899121aa4bafe7a2`  
		Last Modified: Fri, 24 Jul 2020 16:05:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbfde4c7d0e7b20c26672bbf31f444d7ffd54e9dfe527ef87ee29517857e3ce`  
		Last Modified: Fri, 24 Jul 2020 16:06:22 GMT  
		Size: 145.1 MB (145101273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:2db78b0cc1ab5d3c2464459cf202166cf85e05c74b42bb55f4423062ba1ce41b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:d33bfcd93d57ad09ec6dfce460203ac9a3fbd28c3a26728e786b083e5b9a75fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.5 MB (569542261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3658225933b1f125c2a0b1f503683a8ee50fa257a3c7dfd4182e27bc76c8f6d4`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Wed, 22 Jul 2020 20:07:30 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Jul 2020 10:23:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 10:23:49 GMT
EXPOSE 11345
# Thu, 23 Jul 2020 10:23:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Jul 2020 10:23:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Jul 2020 10:23:49 GMT
CMD ["gzserver"]
# Thu, 23 Jul 2020 10:25:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4411483707592dcbac4314bc6194422b5b610683b5131926b750e3cbe20602`  
		Last Modified: Thu, 23 Jul 2020 10:28:29 GMT  
		Size: 18.5 MB (18514095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0dad0c2e98fc85f183e39744e915ce3092535269bc6dbad7a2c9c10f6db53b`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f94ffd189798ed034f2f550bfa7dc551f941f787e3d79b8e2a1d8b3e95e56`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11cdf511ee14cfb3e4d0d1f1d818a9c0697d7f1c26b2863d4e3150d10e4874`  
		Last Modified: Thu, 23 Jul 2020 10:28:52 GMT  
		Size: 202.0 MB (201980881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250ff4fbe3764f76e0b5c60de30521e67122cf9c39b8d5113e6c9755e1669435`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e58c5d82fd76d7425f6b468b16b5c8ca19358ea4858dc87373311dda556a477`  
		Last Modified: Thu, 23 Jul 2020 10:29:45 GMT  
		Size: 303.7 MB (303671023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-xenial`

```console
$ docker pull gazebo@sha256:0a419782150ae56925874117a51f5c197e9172d54630dfe2accdc2228244f50b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:0ce65710641e60b6747a1a719e7b21edff86c5f7b68a41814dafc1fea94214c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.6 MB (493601923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4eff2ac2397a7365bca9b5f6330078c847f312f337edf5c9e58f9d95866b149`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:37:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:37:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 24 Jul 2020 15:37:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 24 Jul 2020 15:42:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:42:36 GMT
EXPOSE 11345
# Fri, 24 Jul 2020 15:42:36 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 24 Jul 2020 15:42:36 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 24 Jul 2020 15:42:36 GMT
CMD ["gzserver"]
# Fri, 24 Jul 2020 15:44:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d916041f92a6961d82541630abdb30c1498f924d9977c3b38b91678d1c02a601`  
		Last Modified: Fri, 24 Jul 2020 16:01:59 GMT  
		Size: 16.3 MB (16275937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27666f170c8634cda060ed942cc86470f03058b3e1544ed9a00a260afe6772ac`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238795d3354ffbeb7f8a071aadaa9303991d0ac42081be50479bbb688b7c69e`  
		Last Modified: Fri, 24 Jul 2020 16:01:55 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba09bf0088affd311d90108b84c0a478a3f7f131f996f27358433f647758b669`  
		Last Modified: Fri, 24 Jul 2020 16:03:53 GMT  
		Size: 208.2 MB (208229225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7f21021ada008f3f0a02f1b4703dc12078c4a954562f101187c37767883f68`  
		Last Modified: Fri, 24 Jul 2020 16:03:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522dcef8c3ea4b77f4b31abd70d0361e487bbf589c2c0838bba94d561c3aa5a9`  
		Last Modified: Fri, 24 Jul 2020 16:05:03 GMT  
		Size: 224.7 MB (224673722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
