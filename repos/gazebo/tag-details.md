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
$ docker pull gazebo@sha256:e89344adae455c894c525c9fb85ebed498f4055a3635f66c0934f5b3bcb31045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10` - linux; amd64

```console
$ docker pull gazebo@sha256:00aa89ef1b9eaf00db8ad681035b9ccd42b2eeec087dcfafbb2ce9581122ced9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268498514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990012ac316ac58bfa423df7d9b3d291ab6b7c4949dccce3568014d6cb8f6c88`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:19:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:20:01 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:20:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:20:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:20:01 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c657cda42b070ca62fc738fcb7ab5cfea8b1f47ac702623cb20614771eef5`  
		Last Modified: Fri, 26 Mar 2021 11:42:26 GMT  
		Size: 226.2 MB (226238115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b9ae36cc6518d0eea17ceb7f889439eba31247373c7ba8cd50f4d05b6c19c5`  
		Last Modified: Fri, 26 Mar 2021 11:41:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver10-bionic`

```console
$ docker pull gazebo@sha256:e89344adae455c894c525c9fb85ebed498f4055a3635f66c0934f5b3bcb31045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:00aa89ef1b9eaf00db8ad681035b9ccd42b2eeec087dcfafbb2ce9581122ced9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268498514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:990012ac316ac58bfa423df7d9b3d291ab6b7c4949dccce3568014d6cb8f6c88`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:19:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:20:01 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:20:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:20:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:20:01 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c657cda42b070ca62fc738fcb7ab5cfea8b1f47ac702623cb20614771eef5`  
		Last Modified: Fri, 26 Mar 2021 11:42:26 GMT  
		Size: 226.2 MB (226238115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b9ae36cc6518d0eea17ceb7f889439eba31247373c7ba8cd50f4d05b6c19c5`  
		Last Modified: Fri, 26 Mar 2021 11:41:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:a7dd8e363c0cf59b746c7083e42f9244a7cfd3978ca3c7d6446c8ac52403a036
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:7c3abf30f66af91c506c4cf4d94567c6a18ff3dc99a30b6fd6305c20d34eee59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.6 MB (318622773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ff4d5712798a90bfed7b6a7b0977557e3ac9dd7c5b6faa5753350f67a325db`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:26:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:30:30 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:30:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:30:31 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:30:31 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c238a927e44fc68e49f93b318a224102c5d7eed49fc3af359975559e12857`  
		Last Modified: Fri, 26 Mar 2021 11:46:19 GMT  
		Size: 1.2 MB (1182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e52b69eeaf83816ec98aa96aae9bb33ed20908a01754650540ee8ba90b582d5`  
		Last Modified: Fri, 26 Mar 2021 11:46:20 GMT  
		Size: 16.1 MB (16149240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e10045afbe7512bc161805bacc32cdfd0be64e9d7aee9a0fa4d44fc470dfe`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3610e3637a69677dc3ae103e4fe54747971847227b66f2d8c118916480d82212`  
		Last Modified: Fri, 26 Mar 2021 11:46:14 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e659d5136d24b5d3cdb805ba756fa64ee2ef602407f1d17742040294be9c037`  
		Last Modified: Fri, 26 Mar 2021 11:47:00 GMT  
		Size: 272.7 MB (272713498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676a7e632f063f555d7200c152cc0b0d373a2e87ccc5451d188c3990a94521d`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:be2715320d2acba9cf7b75b22dacfdeb3e40ee7cd98f29fb992159684a29ab24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:e1e2916fbe4647c792e272f3e14a7ea685bc4bda5992872ca120fa0f683bf129
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277721939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb398497f4ae8b1fc76803871d81deff98566e1438aa51bcf4cdb47bfeb790e`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:23:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:23:44 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:23:44 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:23:44 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:23:44 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6ebc61c427d4925078dbcf4c2b7c93e14175703d693cede750bfc68fc6ff20`  
		Last Modified: Fri, 26 Mar 2021 11:44:43 GMT  
		Size: 235.5 MB (235461541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566ccaa06575c0f5b171a3a83887d6b742250d0b8f6e05b3b604fe96552b7a76`  
		Last Modified: Fri, 26 Mar 2021 11:44:01 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11-focal`

```console
$ docker pull gazebo@sha256:a7dd8e363c0cf59b746c7083e42f9244a7cfd3978ca3c7d6446c8ac52403a036
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:7c3abf30f66af91c506c4cf4d94567c6a18ff3dc99a30b6fd6305c20d34eee59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.6 MB (318622773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ff4d5712798a90bfed7b6a7b0977557e3ac9dd7c5b6faa5753350f67a325db`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:26:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:30:30 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:30:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:30:31 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:30:31 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c238a927e44fc68e49f93b318a224102c5d7eed49fc3af359975559e12857`  
		Last Modified: Fri, 26 Mar 2021 11:46:19 GMT  
		Size: 1.2 MB (1182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e52b69eeaf83816ec98aa96aae9bb33ed20908a01754650540ee8ba90b582d5`  
		Last Modified: Fri, 26 Mar 2021 11:46:20 GMT  
		Size: 16.1 MB (16149240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e10045afbe7512bc161805bacc32cdfd0be64e9d7aee9a0fa4d44fc470dfe`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3610e3637a69677dc3ae103e4fe54747971847227b66f2d8c118916480d82212`  
		Last Modified: Fri, 26 Mar 2021 11:46:14 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e659d5136d24b5d3cdb805ba756fa64ee2ef602407f1d17742040294be9c037`  
		Last Modified: Fri, 26 Mar 2021 11:47:00 GMT  
		Size: 272.7 MB (272713498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676a7e632f063f555d7200c152cc0b0d373a2e87ccc5451d188c3990a94521d`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7`

```console
$ docker pull gazebo@sha256:1088f31e45752f1fa8b34bb88cc2d86371e8f59dff0a5fa3841f3df28ae04306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7` - linux; amd64

```console
$ docker pull gazebo@sha256:3fc63df10e2bf8aa93cb838745da94df6baad7feaa2d9ee1a078ae3da8b15794
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243917482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1605e9aa000db75a78c6d2364a8008c928a7cc97ab406f6c6fb7c6ec454e39`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo7=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:02:09 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:02:10 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:02:10 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:02:10 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c47680dc8b02e364694ee47595b0d36d8d43c706e47a39b55c11db8bbfef8d`  
		Last Modified: Fri, 26 Mar 2021 11:37:20 GMT  
		Size: 181.7 MB (181652684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9fa865bc119a9081b48f02c0fc5fd9a5313df471a20dcac45e3dcdfd49ff3d`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7-xenial`

```console
$ docker pull gazebo@sha256:1088f31e45752f1fa8b34bb88cc2d86371e8f59dff0a5fa3841f3df28ae04306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:3fc63df10e2bf8aa93cb838745da94df6baad7feaa2d9ee1a078ae3da8b15794
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243917482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1605e9aa000db75a78c6d2364a8008c928a7cc97ab406f6c6fb7c6ec454e39`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo7=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:02:09 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:02:10 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:02:10 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:02:10 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c47680dc8b02e364694ee47595b0d36d8d43c706e47a39b55c11db8bbfef8d`  
		Last Modified: Fri, 26 Mar 2021 11:37:20 GMT  
		Size: 181.7 MB (181652684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9fa865bc119a9081b48f02c0fc5fd9a5313df471a20dcac45e3dcdfd49ff3d`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:bbd4c56abb17c3425a1e70aad1ef0563b57c49f698050882182b5b36c25f07f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:bb781b7bfefb02c4d926081a074a941a3269151f5839dbbb5ea8f0fe4f9ca00a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268612956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339096b05c6b1435c477bfd7fd7cf59eaf25ccd5a998e83bd1c1dc13538108b8`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:15:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:15:02 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:15:02 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:15:03 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:15:03 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c50b8a944b4fafa408590d27fd289ae1ab0f8664c49e37f226139631e5d5f`  
		Last Modified: Fri, 26 Mar 2021 11:40:49 GMT  
		Size: 226.4 MB (226352557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06b773b343c41a4c57f6315b3c48c0690f3dc702c3df85d5e601222d707a34`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:bbd4c56abb17c3425a1e70aad1ef0563b57c49f698050882182b5b36c25f07f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:bb781b7bfefb02c4d926081a074a941a3269151f5839dbbb5ea8f0fe4f9ca00a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268612956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339096b05c6b1435c477bfd7fd7cf59eaf25ccd5a998e83bd1c1dc13538108b8`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:15:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:15:02 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:15:02 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:15:03 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:15:03 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c50b8a944b4fafa408590d27fd289ae1ab0f8664c49e37f226139631e5d5f`  
		Last Modified: Fri, 26 Mar 2021 11:40:49 GMT  
		Size: 226.4 MB (226352557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06b773b343c41a4c57f6315b3c48c0690f3dc702c3df85d5e601222d707a34`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:4e0ca75dba54817aa8553d8402aee7f003de0551d858ca66398bc40340a885cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:5bb6e82efddfe2df761498ffed90a0b54e5947c71a7c56792c7efa40e1432921
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266182092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:507a77771e14986a2b0a77e3dbcc64e5db0f67e644a5300fd8251aa06e9c0f57`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:50:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:50:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 27 Mar 2021 04:50:36 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 27 Mar 2021 04:51:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:51:48 GMT
EXPOSE 11345
# Sat, 27 Mar 2021 04:51:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 27 Mar 2021 04:51:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 27 Mar 2021 04:51:49 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6991bbdde750310014591f0ea38c3948d0b10b17a4335ca0534cc4b13755be`  
		Last Modified: Sat, 27 Mar 2021 04:54:57 GMT  
		Size: 18.5 MB (18512473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80080bc5a77ef0d0fda04203730723bf5857aba6e596a0eeebccb945c05e396`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53418e5a6f29f8a6095df153332b47554745496dec0c43648bcce335d47323d`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b77d68449be56c1d29621c8af6185c7192ec98f666d953aa28f2d2be823f1f`  
		Last Modified: Sat, 27 Mar 2021 04:55:15 GMT  
		Size: 202.3 MB (202283482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc45f698bf4302981fc5e7c0dce3d519b2b3640f6889bff40622555c32cda954`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-xenial`

```console
$ docker pull gazebo@sha256:28db84f29d2021a91cf8918823c108b869f05bdc9c4d9167639676b1e2916655
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:3ba937b42f89f5795d59fd2662a1aace4e8ad9fc9df9694a4db2743489b6f37c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.6 MB (270612149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b482061366e43ceb585c69b4e04cfadfcdd4bd08e99f229e5987b7aa0411e6`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:07:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:07:48 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:07:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:07:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:07:49 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da28a57518141ed5feae265da6b5a6bbe1bc5b4b37cb8b0c36f1358a30ee4a80`  
		Last Modified: Fri, 26 Mar 2021 11:39:00 GMT  
		Size: 208.3 MB (208347353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4669d26e6877b63a1d29256c0bbe641fccac466e5ab92610495f463240018096`  
		Last Modified: Fri, 26 Mar 2021 11:38:31 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:latest`

```console
$ docker pull gazebo@sha256:e15b662ee784c18ab697ab11d431aab3b489ee37ee449b9fcba38cd68f3d942e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:0c6c96bd240d806ac705282e66ca344053919f5d253a588053067154d0d33b0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **599.1 MB (599082355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b66c3548b11823e073020660aefe62a10daec1807264547709954c4c6b9c93`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:26:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:30:30 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:30:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:30:31 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:30:31 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:36:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c238a927e44fc68e49f93b318a224102c5d7eed49fc3af359975559e12857`  
		Last Modified: Fri, 26 Mar 2021 11:46:19 GMT  
		Size: 1.2 MB (1182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e52b69eeaf83816ec98aa96aae9bb33ed20908a01754650540ee8ba90b582d5`  
		Last Modified: Fri, 26 Mar 2021 11:46:20 GMT  
		Size: 16.1 MB (16149240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e10045afbe7512bc161805bacc32cdfd0be64e9d7aee9a0fa4d44fc470dfe`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3610e3637a69677dc3ae103e4fe54747971847227b66f2d8c118916480d82212`  
		Last Modified: Fri, 26 Mar 2021 11:46:14 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e659d5136d24b5d3cdb805ba756fa64ee2ef602407f1d17742040294be9c037`  
		Last Modified: Fri, 26 Mar 2021 11:47:00 GMT  
		Size: 272.7 MB (272713498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676a7e632f063f555d7200c152cc0b0d373a2e87ccc5451d188c3990a94521d`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f02a85171f18b326be6bf4f565ab1590ed8cfae1d308aedf43389fbe312d6fb`  
		Last Modified: Fri, 26 Mar 2021 11:48:34 GMT  
		Size: 280.5 MB (280459582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10`

```console
$ docker pull gazebo@sha256:b55d451471b4d1fcb9065cb44a1b5bf06482856e21561066e7a329887427ee3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10` - linux; amd64

```console
$ docker pull gazebo@sha256:36c67233e36b568b80879ed6cd732f09a072622bd670b6bc207fb4388af3a14e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.1 MB (522125766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cc696c8b42cb8f8fd2c707ee74f2c36d2e1d8e132427ba414df6599076ad7f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:19:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:20:01 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:20:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:20:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:20:01 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c657cda42b070ca62fc738fcb7ab5cfea8b1f47ac702623cb20614771eef5`  
		Last Modified: Fri, 26 Mar 2021 11:42:26 GMT  
		Size: 226.2 MB (226238115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b9ae36cc6518d0eea17ceb7f889439eba31247373c7ba8cd50f4d05b6c19c5`  
		Last Modified: Fri, 26 Mar 2021 11:41:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3af4f37304e062dcd362f37edaa26d187fafdcd51da60b7b76bf8f8f5dae4e`  
		Last Modified: Fri, 26 Mar 2021 11:43:49 GMT  
		Size: 253.6 MB (253627252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10-bionic`

```console
$ docker pull gazebo@sha256:b55d451471b4d1fcb9065cb44a1b5bf06482856e21561066e7a329887427ee3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:36c67233e36b568b80879ed6cd732f09a072622bd670b6bc207fb4388af3a14e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.1 MB (522125766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cc696c8b42cb8f8fd2c707ee74f2c36d2e1d8e132427ba414df6599076ad7f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:19:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:20:01 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:20:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:20:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:20:01 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1c657cda42b070ca62fc738fcb7ab5cfea8b1f47ac702623cb20614771eef5`  
		Last Modified: Fri, 26 Mar 2021 11:42:26 GMT  
		Size: 226.2 MB (226238115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b9ae36cc6518d0eea17ceb7f889439eba31247373c7ba8cd50f4d05b6c19c5`  
		Last Modified: Fri, 26 Mar 2021 11:41:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3af4f37304e062dcd362f37edaa26d187fafdcd51da60b7b76bf8f8f5dae4e`  
		Last Modified: Fri, 26 Mar 2021 11:43:49 GMT  
		Size: 253.6 MB (253627252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:e15b662ee784c18ab697ab11d431aab3b489ee37ee449b9fcba38cd68f3d942e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:0c6c96bd240d806ac705282e66ca344053919f5d253a588053067154d0d33b0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **599.1 MB (599082355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b66c3548b11823e073020660aefe62a10daec1807264547709954c4c6b9c93`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:26:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:30:30 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:30:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:30:31 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:30:31 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:36:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c238a927e44fc68e49f93b318a224102c5d7eed49fc3af359975559e12857`  
		Last Modified: Fri, 26 Mar 2021 11:46:19 GMT  
		Size: 1.2 MB (1182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e52b69eeaf83816ec98aa96aae9bb33ed20908a01754650540ee8ba90b582d5`  
		Last Modified: Fri, 26 Mar 2021 11:46:20 GMT  
		Size: 16.1 MB (16149240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e10045afbe7512bc161805bacc32cdfd0be64e9d7aee9a0fa4d44fc470dfe`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3610e3637a69677dc3ae103e4fe54747971847227b66f2d8c118916480d82212`  
		Last Modified: Fri, 26 Mar 2021 11:46:14 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e659d5136d24b5d3cdb805ba756fa64ee2ef602407f1d17742040294be9c037`  
		Last Modified: Fri, 26 Mar 2021 11:47:00 GMT  
		Size: 272.7 MB (272713498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676a7e632f063f555d7200c152cc0b0d373a2e87ccc5451d188c3990a94521d`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f02a85171f18b326be6bf4f565ab1590ed8cfae1d308aedf43389fbe312d6fb`  
		Last Modified: Fri, 26 Mar 2021 11:48:34 GMT  
		Size: 280.5 MB (280459582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:b39c87caec02c8517e1750e634e35d95957c5128261db6b9086ccaf2f6c2f584
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:d11b23898e170fe50e9e4642e446ce1562c3b5df56abec1a57e48fab9f8a564f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.1 MB (547138146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98578ea3521d895418afa8f0deb56a2bacfa327e7d9dd877bfcb039bf607a49d`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:23:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:23:44 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:23:44 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:23:44 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:23:44 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:25:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6ebc61c427d4925078dbcf4c2b7c93e14175703d693cede750bfc68fc6ff20`  
		Last Modified: Fri, 26 Mar 2021 11:44:43 GMT  
		Size: 235.5 MB (235461541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566ccaa06575c0f5b171a3a83887d6b742250d0b8f6e05b3b604fe96552b7a76`  
		Last Modified: Fri, 26 Mar 2021 11:44:01 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb625925631ef7f68b1049bc56e13f66cfa465e2c3e429d4ce728a02812bae9`  
		Last Modified: Fri, 26 Mar 2021 11:46:04 GMT  
		Size: 269.4 MB (269416207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:e15b662ee784c18ab697ab11d431aab3b489ee37ee449b9fcba38cd68f3d942e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:0c6c96bd240d806ac705282e66ca344053919f5d253a588053067154d0d33b0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **599.1 MB (599082355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b66c3548b11823e073020660aefe62a10daec1807264547709954c4c6b9c93`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:25:35 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:26:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:26:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:30:30 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:30:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:30:31 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:30:31 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:36:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.3.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c238a927e44fc68e49f93b318a224102c5d7eed49fc3af359975559e12857`  
		Last Modified: Fri, 26 Mar 2021 11:46:19 GMT  
		Size: 1.2 MB (1182444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e52b69eeaf83816ec98aa96aae9bb33ed20908a01754650540ee8ba90b582d5`  
		Last Modified: Fri, 26 Mar 2021 11:46:20 GMT  
		Size: 16.1 MB (16149240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e10045afbe7512bc161805bacc32cdfd0be64e9d7aee9a0fa4d44fc470dfe`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3610e3637a69677dc3ae103e4fe54747971847227b66f2d8c118916480d82212`  
		Last Modified: Fri, 26 Mar 2021 11:46:14 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e659d5136d24b5d3cdb805ba756fa64ee2ef602407f1d17742040294be9c037`  
		Last Modified: Fri, 26 Mar 2021 11:47:00 GMT  
		Size: 272.7 MB (272713498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676a7e632f063f555d7200c152cc0b0d373a2e87ccc5451d188c3990a94521d`  
		Last Modified: Fri, 26 Mar 2021 11:46:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f02a85171f18b326be6bf4f565ab1590ed8cfae1d308aedf43389fbe312d6fb`  
		Last Modified: Fri, 26 Mar 2021 11:48:34 GMT  
		Size: 280.5 MB (280459582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7`

```console
$ docker pull gazebo@sha256:a1376aca1ff3e926afa6ea7035a7568225b5b80d11a258191fdef356a9d84911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7` - linux; amd64

```console
$ docker pull gazebo@sha256:d9091f12fe93cd8131a242be07d9038f60b6b77e52ee36b0821a6840edf6be45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.3 MB (484328524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe8a38cb4ed85c357ea0c626edf1668533ac5b4a0e73d2f50769d728180e145`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo7=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:02:09 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:02:10 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:02:10 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:02:10 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo7-dev=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c47680dc8b02e364694ee47595b0d36d8d43c706e47a39b55c11db8bbfef8d`  
		Last Modified: Fri, 26 Mar 2021 11:37:20 GMT  
		Size: 181.7 MB (181652684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9fa865bc119a9081b48f02c0fc5fd9a5313df471a20dcac45e3dcdfd49ff3d`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839171e0001baf0b7d7b0d473b19233df1807acb176040c1df1db05aae930342`  
		Last Modified: Fri, 26 Mar 2021 11:38:18 GMT  
		Size: 240.4 MB (240411042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7-xenial`

```console
$ docker pull gazebo@sha256:a1376aca1ff3e926afa6ea7035a7568225b5b80d11a258191fdef356a9d84911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:d9091f12fe93cd8131a242be07d9038f60b6b77e52ee36b0821a6840edf6be45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.3 MB (484328524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe8a38cb4ed85c357ea0c626edf1668533ac5b4a0e73d2f50769d728180e145`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:02:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo7=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:02:09 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:02:10 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:02:10 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:02:10 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:05:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo7-dev=7.16.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c47680dc8b02e364694ee47595b0d36d8d43c706e47a39b55c11db8bbfef8d`  
		Last Modified: Fri, 26 Mar 2021 11:37:20 GMT  
		Size: 181.7 MB (181652684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9fa865bc119a9081b48f02c0fc5fd9a5313df471a20dcac45e3dcdfd49ff3d`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839171e0001baf0b7d7b0d473b19233df1807acb176040c1df1db05aae930342`  
		Last Modified: Fri, 26 Mar 2021 11:38:18 GMT  
		Size: 240.4 MB (240411042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:527820622d0405c7aa6d5e7dd481536adbfe8673f6b2505baae2760674d5084f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:482ea1fb8cd848ae9065b13e163c7c7212ee6fcfb6fd0f1ef5710cb27fb68650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.8 MB (413817652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f80b5741bb5e4f6ef185f13026aa8156b3c71cff3d3c3ec283992a4915a6039`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:15:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:15:02 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:15:02 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:15:03 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:15:03 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c50b8a944b4fafa408590d27fd289ae1ab0f8664c49e37f226139631e5d5f`  
		Last Modified: Fri, 26 Mar 2021 11:40:49 GMT  
		Size: 226.4 MB (226352557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06b773b343c41a4c57f6315b3c48c0690f3dc702c3df85d5e601222d707a34`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781f5db599f0ebc01863243f776548ca47e2b104700bee7c6a6cd6b06dd621a1`  
		Last Modified: Fri, 26 Mar 2021 11:41:40 GMT  
		Size: 145.2 MB (145204696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-bionic`

```console
$ docker pull gazebo@sha256:527820622d0405c7aa6d5e7dd481536adbfe8673f6b2505baae2760674d5084f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:482ea1fb8cd848ae9065b13e163c7c7212ee6fcfb6fd0f1ef5710cb27fb68650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.8 MB (413817652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f80b5741bb5e4f6ef185f13026aa8156b3c71cff3d3c3ec283992a4915a6039`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:10:22 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:11:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 11:11:09 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:15:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:15:02 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:15:02 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:15:03 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:15:03 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa0eff1a96d1d945845cab86a8e978cc925e0c70eb0c4c23df2d989f3d08c6`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 840.2 KB (840161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173394d5eef61aa7ce6db53e2c5e13988f1e165ad4d657aff376954078c9f4`  
		Last Modified: Fri, 26 Mar 2021 11:40:20 GMT  
		Size: 14.7 MB (14701328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b584f647c38b5ad3f307fffbabfb06c9038b800f2b5c75942e5b89cf21b9e48`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481f95c2c477adc29785416c7324b97b8b0e96af9722fcc3e186f21da90858`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 5.5 KB (5457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c50b8a944b4fafa408590d27fd289ae1ab0f8664c49e37f226139631e5d5f`  
		Last Modified: Fri, 26 Mar 2021 11:40:49 GMT  
		Size: 226.4 MB (226352557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06b773b343c41a4c57f6315b3c48c0690f3dc702c3df85d5e601222d707a34`  
		Last Modified: Fri, 26 Mar 2021 11:40:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781f5db599f0ebc01863243f776548ca47e2b104700bee7c6a6cd6b06dd621a1`  
		Last Modified: Fri, 26 Mar 2021 11:41:40 GMT  
		Size: 145.2 MB (145204696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:3656199c59f7e03b6eb3b2b1f76079e9a157dab1b9f05ae597af7cf8db512313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:cf7072fca9df25c2f1447098ca4a69285414ad36cabd553e5a216285692ce411
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **570.3 MB (570253015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1946a4e5ab2ce443c2d1d2911c8a0636ed70194d93888de0253dc2299f717140`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:50:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:50:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 27 Mar 2021 04:50:36 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 27 Mar 2021 04:51:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:51:48 GMT
EXPOSE 11345
# Sat, 27 Mar 2021 04:51:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 27 Mar 2021 04:51:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 27 Mar 2021 04:51:49 GMT
CMD ["gzserver"]
# Sat, 27 Mar 2021 04:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6991bbdde750310014591f0ea38c3948d0b10b17a4335ca0534cc4b13755be`  
		Last Modified: Sat, 27 Mar 2021 04:54:57 GMT  
		Size: 18.5 MB (18512473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80080bc5a77ef0d0fda04203730723bf5857aba6e596a0eeebccb945c05e396`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53418e5a6f29f8a6095df153332b47554745496dec0c43648bcce335d47323d`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b77d68449be56c1d29621c8af6185c7192ec98f666d953aa28f2d2be823f1f`  
		Last Modified: Sat, 27 Mar 2021 04:55:15 GMT  
		Size: 202.3 MB (202283482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc45f698bf4302981fc5e7c0dce3d519b2b3640f6889bff40622555c32cda954`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224bc61ac07ce76ff4aeafb7c24d7fd15b4f8f265e164e684b6af38da402c998`  
		Last Modified: Sat, 27 Mar 2021 04:56:29 GMT  
		Size: 304.1 MB (304070923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-xenial`

```console
$ docker pull gazebo@sha256:191c1e5d43023587ffcf97f4458b8aef8a4bf57f5cb975df8b392613805f388f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:65fc197a741abdc10b09208e815daf076dae556183fc36a4c66c660c1a891a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.4 MB (495361056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a5209bf571036c095f230504bef59cc4fa7ac1573653188263a80477945f54f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:59:10 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:59:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 26 Mar 2021 10:59:13 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 26 Mar 2021 11:07:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:07:48 GMT
EXPOSE 11345
# Fri, 26 Mar 2021 11:07:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 26 Mar 2021 11:07:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 26 Mar 2021 11:07:49 GMT
CMD ["gzserver"]
# Fri, 26 Mar 2021 11:09:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d0e8f810db17f0571da3cf2c9bd7417f7d73695388bc1aaed4e210aa54732`  
		Last Modified: Fri, 26 Mar 2021 11:36:58 GMT  
		Size: 16.3 MB (16280405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61e4286aac2a2f27ed2e4067426bf7fffeef043ff4209cda58ce241ffa39e6`  
		Last Modified: Fri, 26 Mar 2021 11:36:54 GMT  
		Size: 14.8 KB (14760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa17012d4ee4708da00c83ca4dbd3c90c182e190cca2dc4ad45b3a40889df44`  
		Last Modified: Fri, 26 Mar 2021 11:36:57 GMT  
		Size: 5.6 KB (5553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da28a57518141ed5feae265da6b5a6bbe1bc5b4b37cb8b0c36f1358a30ee4a80`  
		Last Modified: Fri, 26 Mar 2021 11:39:00 GMT  
		Size: 208.3 MB (208347353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4669d26e6877b63a1d29256c0bbe641fccac466e5ab92610495f463240018096`  
		Last Modified: Fri, 26 Mar 2021 11:38:31 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cf3b6066abc2c4fba4490b161c84b2d58782953adc1f702bd29680112c6257`  
		Last Modified: Fri, 26 Mar 2021 11:40:03 GMT  
		Size: 224.7 MB (224748907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
