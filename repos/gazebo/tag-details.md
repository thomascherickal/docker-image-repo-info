<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `gazebo`

-	[`gazebo:gzserver10`](#gazebogzserver10)
-	[`gazebo:gzserver10-bionic`](#gazebogzserver10-bionic)
-	[`gazebo:gzserver11`](#gazebogzserver11)
-	[`gazebo:gzserver11-bionic`](#gazebogzserver11-bionic)
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
-	[`gazebo:libgazebo7`](#gazebolibgazebo7)
-	[`gazebo:libgazebo7-xenial`](#gazebolibgazebo7-xenial)
-	[`gazebo:libgazebo9`](#gazebolibgazebo9)
-	[`gazebo:libgazebo9-bionic`](#gazebolibgazebo9-bionic)
-	[`gazebo:libgazebo9-stretch`](#gazebolibgazebo9-stretch)
-	[`gazebo:libgazebo9-xenial`](#gazebolibgazebo9-xenial)

## `gazebo:gzserver10`

```console
$ docker pull gazebo@sha256:b358ba63452e6fe3617a8b2f5248a5bdf6546730b95b547a57e544f57820b0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10` - linux; amd64

```console
$ docker pull gazebo@sha256:6e6d52fe4d4cf44ed4c0a286f0ca196ec892b2e4bd047a1f35fd0c9d60296760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298798475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb030aed8429ecf0018d92851e7aa753c4dcbdd16367ee7b6d9746ee94b8b4b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:00:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:00:01 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:00:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:00:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:00:01 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd71ac7c348f9d95d42969693ed4b5a1e886462ceae402767c93faf5553cc08f`  
		Last Modified: Fri, 20 Mar 2020 21:06:49 GMT  
		Size: 256.1 MB (256075614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef35106135279ca751e3f4019135b4b61594dbdf671174666773cf007022613`  
		Last Modified: Fri, 20 Mar 2020 21:06:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver10-bionic`

```console
$ docker pull gazebo@sha256:b358ba63452e6fe3617a8b2f5248a5bdf6546730b95b547a57e544f57820b0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:6e6d52fe4d4cf44ed4c0a286f0ca196ec892b2e4bd047a1f35fd0c9d60296760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298798475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb030aed8429ecf0018d92851e7aa753c4dcbdd16367ee7b6d9746ee94b8b4b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:00:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:00:01 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:00:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:00:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:00:01 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd71ac7c348f9d95d42969693ed4b5a1e886462ceae402767c93faf5553cc08f`  
		Last Modified: Fri, 20 Mar 2020 21:06:49 GMT  
		Size: 256.1 MB (256075614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef35106135279ca751e3f4019135b4b61594dbdf671174666773cf007022613`  
		Last Modified: Fri, 20 Mar 2020 21:06:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:99d0a6be935f601cb3e274c50ced99f76ef001be01fc707b6bd4051849d54d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:14e94b30f1aab6bbb7c02577d77db667cbb1790b104ad05c9d5e7cec2fbc9d11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301472383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c4917ccb156fe3d7badf132bb0c0109eb5d6c69ad34b7f159ed413557786a8`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:99d0a6be935f601cb3e274c50ced99f76ef001be01fc707b6bd4051849d54d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:14e94b30f1aab6bbb7c02577d77db667cbb1790b104ad05c9d5e7cec2fbc9d11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.5 MB (301472383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c4917ccb156fe3d7badf132bb0c0109eb5d6c69ad34b7f159ed413557786a8`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7`

```console
$ docker pull gazebo@sha256:f714616dbfa59c4e236724b010c86608d5fdb746a5733fbe18e3cce4a8344255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7` - linux; amd64

```console
$ docker pull gazebo@sha256:c30a62097dd2e7bff5de5ea218599c3c5ad37b332601e731f8da2bc22c2e5663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250649377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e45bbeaf390d1cdf6b0d3b83dda2bb63ebc645a654c032ca55a68b754496c93`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 21 Feb 2020 23:28:07 GMT
RUN apt-get update && apt-get install -q -y     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:28:07 GMT
EXPOSE 11345
# Fri, 21 Feb 2020 23:28:07 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 21 Feb 2020 23:28:07 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 21 Feb 2020 23:28:08 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025559e6749872e63f778f6dfef89765e7e18f4bc508633153df0ecc5cb2438`  
		Last Modified: Fri, 21 Feb 2020 23:45:05 GMT  
		Size: 189.8 MB (189780833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75958b52b14f1654a39d50fb5b8f5680e6d54f2d8869a75564d1b41f3ebc7467`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver7-xenial`

```console
$ docker pull gazebo@sha256:f714616dbfa59c4e236724b010c86608d5fdb746a5733fbe18e3cce4a8344255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:c30a62097dd2e7bff5de5ea218599c3c5ad37b332601e731f8da2bc22c2e5663
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250649377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e45bbeaf390d1cdf6b0d3b83dda2bb63ebc645a654c032ca55a68b754496c93`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 21 Feb 2020 23:28:07 GMT
RUN apt-get update && apt-get install -q -y     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:28:07 GMT
EXPOSE 11345
# Fri, 21 Feb 2020 23:28:07 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 21 Feb 2020 23:28:07 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 21 Feb 2020 23:28:08 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025559e6749872e63f778f6dfef89765e7e18f4bc508633153df0ecc5cb2438`  
		Last Modified: Fri, 21 Feb 2020 23:45:05 GMT  
		Size: 189.8 MB (189780833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75958b52b14f1654a39d50fb5b8f5680e6d54f2d8869a75564d1b41f3ebc7467`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:d89c5e33fc8db49cf284d5b145e9868aca3de18a5af6404ea7c308f9939602f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:6b907ff56faba94e10bbeb7a9302fa935e9db7050a02d7b4021230eb4ae4300e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.5 MB (299529870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c4117f86b100e1e0ed2b202705dccdf14e9e19aa59f151a9e3cbafb9a127e9`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:31:53 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:31:54 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:31:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:31:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:31:54 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b836fe682f0969c73def0da1bfb0bc95d93a4c443a8d20995c34b62ddc37887d`  
		Last Modified: Mon, 06 Apr 2020 20:44:29 GMT  
		Size: 256.8 MB (256807009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec66b5fcbea9ead3b7939a947c9e38c41172c5457b313acc94b530916a55a6c1`  
		Last Modified: Mon, 06 Apr 2020 20:40:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:d89c5e33fc8db49cf284d5b145e9868aca3de18a5af6404ea7c308f9939602f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:6b907ff56faba94e10bbeb7a9302fa935e9db7050a02d7b4021230eb4ae4300e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.5 MB (299529870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c4117f86b100e1e0ed2b202705dccdf14e9e19aa59f151a9e3cbafb9a127e9`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:31:53 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:31:54 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:31:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:31:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:31:54 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b836fe682f0969c73def0da1bfb0bc95d93a4c443a8d20995c34b62ddc37887d`  
		Last Modified: Mon, 06 Apr 2020 20:44:29 GMT  
		Size: 256.8 MB (256807009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec66b5fcbea9ead3b7939a947c9e38c41172c5457b313acc94b530916a55a6c1`  
		Last Modified: Mon, 06 Apr 2020 20:40:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:4a1329b2442382ade2673c2ebb2a6d5cb2b48541a490401c4b49a0eb94722e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:9b1e77d96d0134e6ac8b7cf00b73668d25444c94749164bcd0cf2e553045f112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.3 MB (346348740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94346110a6c3c013e03f5462f48c74107a18d5ba76fe5f2c27bd27b4c99f3be0`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:42:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 23 Apr 2020 01:42:42 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Apr 2020 01:44:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:44:01 GMT
EXPOSE 11345
# Thu, 23 Apr 2020 01:44:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Apr 2020 01:44:02 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Apr 2020 01:44:02 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34502294a02bc4b5c87766699f13475a1f7403335fd2821ab6fc1b3ec5ba3d7c`  
		Last Modified: Thu, 23 Apr 2020 01:46:15 GMT  
		Size: 21.1 MB (21095000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f91f9850ce1646beddf2640422d469d00b3bf4e412306a90fcd63331adfb41c`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983d13ecad407e0bb4bd2e197bbc7afa28e75467becfbd82e5e917e6c3b4793e`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5406926b69455e0c8280ca6a3673804030a8979279d8200b701c8bab92089e`  
		Last Modified: Thu, 23 Apr 2020 01:46:53 GMT  
		Size: 279.9 MB (279871200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e5b376e643b770370ae9291c4bd1cab32b385fccfa0b5406f1cdcc13c82f8d`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:gzserver9-xenial`

```console
$ docker pull gazebo@sha256:a456c82f33c0995c7878adf9956a8f73444877130b92d48a0bae624b5151fd94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:041646d7820ac53073aef7f69305087e9eec008f893091fc37ea29d1ff397ff1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280340551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3dee2898fff424f2f64fbb486fba4e06f0107ece907800d6e98a1485013b297`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:25:38 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:25:38 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:25:38 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:25:38 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:25:39 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081b870b09d1ee2bba60ec0d26856497e8bf1ca97e5a2e8824b944f6906369b6`  
		Last Modified: Mon, 06 Apr 2020 20:38:45 GMT  
		Size: 219.5 MB (219472008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfec6c8e27760dd30b27063bafa5b33eaefa5f25789b72041d8916f474dafffe`  
		Last Modified: Mon, 06 Apr 2020 20:34:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:latest`

```console
$ docker pull gazebo@sha256:a1abd8a01749e82d1cb3e5c869c4cd9c2ff080735f0d898f96827712be323e14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:d86413a7d3ab3a24c69fd53aaaa6620b9c2001a6d21a42fb0a4dc2728c8f720d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **602.3 MB (602344811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba056cb9fc3f3fc838667a488c807a19941c021ac13dac55c551a556eb6ced86`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
# Fri, 20 Mar 2020 21:04:20 GMT
RUN apt-get update && apt-get install -q -y     libgazebo11-dev=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa19d07d2818382a61b0f2603886fee78bfa84887b5a437d2e45d45dfc06053`  
		Last Modified: Fri, 20 Mar 2020 21:09:15 GMT  
		Size: 300.9 MB (300872428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10`

```console
$ docker pull gazebo@sha256:defbc13eef1ef10c572264ca1480b77433a8403c53efd4d50e1b4075b0e4ff98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10` - linux; amd64

```console
$ docker pull gazebo@sha256:cd1afa1b5e9c6171e95066667080d063ebddb4f4692895b85991a63045bfc265
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.3 MB (587314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de00dfe9b40b286a6646b2831b736e8caee241576df62069bf2708ab37d5fcce`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:00:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:00:01 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:00:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:00:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:00:01 GMT
CMD ["gzserver"]
# Fri, 20 Mar 2020 21:01:22 GMT
RUN apt-get update && apt-get install -q -y     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd71ac7c348f9d95d42969693ed4b5a1e886462ceae402767c93faf5553cc08f`  
		Last Modified: Fri, 20 Mar 2020 21:06:49 GMT  
		Size: 256.1 MB (256075614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef35106135279ca751e3f4019135b4b61594dbdf671174666773cf007022613`  
		Last Modified: Fri, 20 Mar 2020 21:06:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219f22304588077f49a6940612fa53bcd2e34f1b82fdee2cb4d37b1090844dc4`  
		Last Modified: Fri, 20 Mar 2020 21:07:39 GMT  
		Size: 288.5 MB (288515559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo10-bionic`

```console
$ docker pull gazebo@sha256:defbc13eef1ef10c572264ca1480b77433a8403c53efd4d50e1b4075b0e4ff98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo10-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:cd1afa1b5e9c6171e95066667080d063ebddb4f4692895b85991a63045bfc265
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.3 MB (587314034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de00dfe9b40b286a6646b2831b736e8caee241576df62069bf2708ab37d5fcce`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:00:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo10=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:00:01 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:00:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:00:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:00:01 GMT
CMD ["gzserver"]
# Fri, 20 Mar 2020 21:01:22 GMT
RUN apt-get update && apt-get install -q -y     libgazebo10-dev=10.2.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd71ac7c348f9d95d42969693ed4b5a1e886462ceae402767c93faf5553cc08f`  
		Last Modified: Fri, 20 Mar 2020 21:06:49 GMT  
		Size: 256.1 MB (256075614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef35106135279ca751e3f4019135b4b61594dbdf671174666773cf007022613`  
		Last Modified: Fri, 20 Mar 2020 21:06:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219f22304588077f49a6940612fa53bcd2e34f1b82fdee2cb4d37b1090844dc4`  
		Last Modified: Fri, 20 Mar 2020 21:07:39 GMT  
		Size: 288.5 MB (288515559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:a1abd8a01749e82d1cb3e5c869c4cd9c2ff080735f0d898f96827712be323e14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:d86413a7d3ab3a24c69fd53aaaa6620b9c2001a6d21a42fb0a4dc2728c8f720d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **602.3 MB (602344811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba056cb9fc3f3fc838667a488c807a19941c021ac13dac55c551a556eb6ced86`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
# Fri, 20 Mar 2020 21:04:20 GMT
RUN apt-get update && apt-get install -q -y     libgazebo11-dev=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa19d07d2818382a61b0f2603886fee78bfa84887b5a437d2e45d45dfc06053`  
		Last Modified: Fri, 20 Mar 2020 21:09:15 GMT  
		Size: 300.9 MB (300872428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo11-bionic`

```console
$ docker pull gazebo@sha256:a1abd8a01749e82d1cb3e5c869c4cd9c2ff080735f0d898f96827712be323e14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:d86413a7d3ab3a24c69fd53aaaa6620b9c2001a6d21a42fb0a4dc2728c8f720d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **602.3 MB (602344811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba056cb9fc3f3fc838667a488c807a19941c021ac13dac55c551a556eb6ced86`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 20 Mar 2020 21:02:45 GMT
RUN apt-get update && apt-get install -q -y     gazebo11=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 21:02:46 GMT
EXPOSE 11345
# Fri, 20 Mar 2020 21:02:46 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 20 Mar 2020 21:02:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 20 Mar 2020 21:02:47 GMT
CMD ["gzserver"]
# Fri, 20 Mar 2020 21:04:20 GMT
RUN apt-get update && apt-get install -q -y     libgazebo11-dev=11.0.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998f7e37ef010e3138493d5604da592ef98e7e5758a0111e1a4645212a099e6`  
		Last Modified: Fri, 20 Mar 2020 21:08:22 GMT  
		Size: 258.7 MB (258749521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db145bf1e587e0089f1dc4d6f46a371c077701f8506db0f75025db663e118f6c`  
		Last Modified: Fri, 20 Mar 2020 21:07:44 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa19d07d2818382a61b0f2603886fee78bfa84887b5a437d2e45d45dfc06053`  
		Last Modified: Fri, 20 Mar 2020 21:09:15 GMT  
		Size: 300.9 MB (300872428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7`

```console
$ docker pull gazebo@sha256:3a1adde4b4ccecc028dcafb83182b37a14f765cd23014bc3e5b9163ee102f9e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7` - linux; amd64

```console
$ docker pull gazebo@sha256:b3c67851b05829766cfd8f8607d120ac67db38e6146b4ab442621c6c1759cc11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.9 MB (509912806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b6e8df29fe27d44b599d047052e07e232966162be9676875a04a158b33d7a1`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 21 Feb 2020 23:28:07 GMT
RUN apt-get update && apt-get install -q -y     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:28:07 GMT
EXPOSE 11345
# Fri, 21 Feb 2020 23:28:07 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 21 Feb 2020 23:28:07 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 21 Feb 2020 23:28:08 GMT
CMD ["gzserver"]
# Fri, 21 Feb 2020 23:30:30 GMT
RUN apt-get update && apt-get install -q -y     libgazebo7-dev=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025559e6749872e63f778f6dfef89765e7e18f4bc508633153df0ecc5cb2438`  
		Last Modified: Fri, 21 Feb 2020 23:45:05 GMT  
		Size: 189.8 MB (189780833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75958b52b14f1654a39d50fb5b8f5680e6d54f2d8869a75564d1b41f3ebc7467`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e74814905efa94a834e042cf439bcfa5d708ce3b5c62e9d31f74721ab8678f`  
		Last Modified: Fri, 21 Feb 2020 23:46:05 GMT  
		Size: 259.3 MB (259263429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo7-xenial`

```console
$ docker pull gazebo@sha256:3a1adde4b4ccecc028dcafb83182b37a14f765cd23014bc3e5b9163ee102f9e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo7-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:b3c67851b05829766cfd8f8607d120ac67db38e6146b4ab442621c6c1759cc11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.9 MB (509912806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b6e8df29fe27d44b599d047052e07e232966162be9676875a04a158b33d7a1`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 21 Feb 2020 23:28:07 GMT
RUN apt-get update && apt-get install -q -y     gazebo7=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:28:07 GMT
EXPOSE 11345
# Fri, 21 Feb 2020 23:28:07 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 21 Feb 2020 23:28:07 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 21 Feb 2020 23:28:08 GMT
CMD ["gzserver"]
# Fri, 21 Feb 2020 23:30:30 GMT
RUN apt-get update && apt-get install -q -y     libgazebo7-dev=7.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7025559e6749872e63f778f6dfef89765e7e18f4bc508633153df0ecc5cb2438`  
		Last Modified: Fri, 21 Feb 2020 23:45:05 GMT  
		Size: 189.8 MB (189780833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75958b52b14f1654a39d50fb5b8f5680e6d54f2d8869a75564d1b41f3ebc7467`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e74814905efa94a834e042cf439bcfa5d708ce3b5c62e9d31f74721ab8678f`  
		Last Modified: Fri, 21 Feb 2020 23:46:05 GMT  
		Size: 259.3 MB (259263429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:d0642e5f473c09ce8f9a5770ad49b7dbee2bdea86b3f8f1b288ca583dacb80ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:61cacaaeec40453a86a22d79ca7369b0b51a6ef6bf68dc9d9f55eece82d36382
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.6 MB (479608718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870680ebe55e4471c7480f09c3b2d14ef87e9581c27627513914c2fd6951581e`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:31:53 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:31:54 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:31:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:31:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:31:54 GMT
CMD ["gzserver"]
# Mon, 06 Apr 2020 20:34:18 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b836fe682f0969c73def0da1bfb0bc95d93a4c443a8d20995c34b62ddc37887d`  
		Last Modified: Mon, 06 Apr 2020 20:44:29 GMT  
		Size: 256.8 MB (256807009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec66b5fcbea9ead3b7939a947c9e38c41172c5457b313acc94b530916a55a6c1`  
		Last Modified: Mon, 06 Apr 2020 20:40:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d349fb23c6a09c5e136c8f9bec8b8dbf7689bbae0af550b46a33a196bf2aba0a`  
		Last Modified: Mon, 06 Apr 2020 20:45:28 GMT  
		Size: 180.1 MB (180078848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-bionic`

```console
$ docker pull gazebo@sha256:d0642e5f473c09ce8f9a5770ad49b7dbee2bdea86b3f8f1b288ca583dacb80ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:61cacaaeec40453a86a22d79ca7369b0b51a6ef6bf68dc9d9f55eece82d36382
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.6 MB (479608718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870680ebe55e4471c7480f09c3b2d14ef87e9581c27627513914c2fd6951581e`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:17:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:58 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:55:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 20 Mar 2020 20:56:00 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:31:53 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:31:54 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:31:54 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:31:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:31:54 GMT
CMD ["gzserver"]
# Mon, 06 Apr 2020 20:34:18 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97510123400e649cc5a98136827c7d21af815d5d349e28a7ab4aa81822936de7`  
		Last Modified: Fri, 20 Mar 2020 20:33:10 GMT  
		Size: 838.2 KB (838197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbf03a431c81899103bea322503020e82fbab7691a18c3218832abc44c6ed`  
		Last Modified: Fri, 20 Mar 2020 21:04:43 GMT  
		Size: 15.2 MB (15150645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e9be754f0ddc5b56c06184b996e3dbceeec7ac5bd0550b54ed5c7ee217da1`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fb356a3b3f242e4d29a37ab838b473444f24bf293953d022d1e3df14f4265`  
		Last Modified: Fri, 20 Mar 2020 21:04:40 GMT  
		Size: 5.4 KB (5429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b836fe682f0969c73def0da1bfb0bc95d93a4c443a8d20995c34b62ddc37887d`  
		Last Modified: Mon, 06 Apr 2020 20:44:29 GMT  
		Size: 256.8 MB (256807009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec66b5fcbea9ead3b7939a947c9e38c41172c5457b313acc94b530916a55a6c1`  
		Last Modified: Mon, 06 Apr 2020 20:40:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d349fb23c6a09c5e136c8f9bec8b8dbf7689bbae0af550b46a33a196bf2aba0a`  
		Last Modified: Mon, 06 Apr 2020 20:45:28 GMT  
		Size: 180.1 MB (180078848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:403a8229790daa8c46e6ec925875a4c5ad7210f1d49b5aca69ebd4d13c7d6af7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:4d37d3d51460de5711c218290bc8ec70552d7027148c47db72e5ebe15ffbbaef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **651.0 MB (650966527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9553c75eebdb5347cc8550f000e9bf3629783fd4b432c2eaed870e9b8d9b86`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:42:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 23 Apr 2020 01:42:42 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Apr 2020 01:44:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:44:01 GMT
EXPOSE 11345
# Thu, 23 Apr 2020 01:44:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Apr 2020 01:44:02 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Apr 2020 01:44:02 GMT
CMD ["gzserver"]
# Thu, 23 Apr 2020 01:45:32 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34502294a02bc4b5c87766699f13475a1f7403335fd2821ab6fc1b3ec5ba3d7c`  
		Last Modified: Thu, 23 Apr 2020 01:46:15 GMT  
		Size: 21.1 MB (21095000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f91f9850ce1646beddf2640422d469d00b3bf4e412306a90fcd63331adfb41c`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983d13ecad407e0bb4bd2e197bbc7afa28e75467becfbd82e5e917e6c3b4793e`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5406926b69455e0c8280ca6a3673804030a8979279d8200b701c8bab92089e`  
		Last Modified: Thu, 23 Apr 2020 01:46:53 GMT  
		Size: 279.9 MB (279871200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e5b376e643b770370ae9291c4bd1cab32b385fccfa0b5406f1cdcc13c82f8d`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401a6bfd471f0a3ddfb51025e7934b97e9ca1a68e5a0c06b93341af1b5cb5c89`  
		Last Modified: Thu, 23 Apr 2020 01:47:55 GMT  
		Size: 304.6 MB (304617787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `gazebo:libgazebo9-xenial`

```console
$ docker pull gazebo@sha256:c194cf2db187949c1d4629cf15c09ffbf19dbce1be1f9f505b71749bfa323f08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:813a06d67ee9f9d2c738ec77bd755e9d6636d9788d09f67163ec826252fe0ff8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **522.7 MB (522697949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0502ea6a44d78044d74de0601c5d46dcc4830bd311d1757c5bb7160191870fca`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:26:29 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:26:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 21 Feb 2020 23:26:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 06 Apr 2020 20:25:38 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 20:25:38 GMT
EXPOSE 11345
# Mon, 06 Apr 2020 20:25:38 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 06 Apr 2020 20:25:38 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 06 Apr 2020 20:25:39 GMT
CMD ["gzserver"]
# Mon, 06 Apr 2020 20:28:46 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.13.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800fbbcfa76fef22becb19160c1bc6ff902d29e48da7cbbf10dc139f88399424`  
		Last Modified: Fri, 21 Feb 2020 23:44:38 GMT  
		Size: 16.7 MB (16656445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d1ccb8bcca00d55e3e0cbaa6ebc7de8c4b3c2cddda85f8ce41d1bc5f365e8b`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 13.1 KB (13119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6138c22d01789aa9d9feb0ccfacf5f26d9a6e0f27b80d8a49470a5b605853e`  
		Last Modified: Fri, 21 Feb 2020 23:44:34 GMT  
		Size: 5.5 KB (5520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081b870b09d1ee2bba60ec0d26856497e8bf1ca97e5a2e8824b944f6906369b6`  
		Last Modified: Mon, 06 Apr 2020 20:38:45 GMT  
		Size: 219.5 MB (219472008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfec6c8e27760dd30b27063bafa5b33eaefa5f25789b72041d8916f474dafffe`  
		Last Modified: Mon, 06 Apr 2020 20:34:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e489b247d5c7bf8cfc9a9ffc3aa0f6d0cfb75166b21f766951e988f6ee9ee0`  
		Last Modified: Mon, 06 Apr 2020 20:39:57 GMT  
		Size: 242.4 MB (242357398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
