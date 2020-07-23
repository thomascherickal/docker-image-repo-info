## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:06578340ee08017404c25331ee78ecc4617d9fff025bf0124d17a553ac85effd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:e730b2a8f93f1e18fc8cc1141f7f5ab33de1faa01aae6114ba69452854638f61
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268363562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6048fb6436fcf3ff26fac3c9ab559634e8c91137c15080098e2d12b198e869`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:42:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:43:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Mon, 06 Jul 2020 23:43:11 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Jul 2020 10:20:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 10:20:32 GMT
EXPOSE 11345
# Thu, 23 Jul 2020 10:20:32 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Jul 2020 10:20:33 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Jul 2020 10:20:33 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5a9a0d3edafb836db5fec8836034836fd3958d7f30865871a5e6bd21ea4f82`  
		Last Modified: Mon, 06 Jul 2020 23:59:55 GMT  
		Size: 837.6 KB (837576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e325120aafa0f4feb33c505b3e557b8e1741e2bdcd40588c58a714be3d0603a`  
		Last Modified: Tue, 07 Jul 2020 00:00:01 GMT  
		Size: 14.7 MB (14694900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62359864d8bd7d9168f4c7ad0b3e7d009f978e52f64a889ed7288aaead75fb93`  
		Last Modified: Mon, 06 Jul 2020 23:59:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd2afc00dbacd927b3bfd10dc166b4e784b5a9896beb2f65dfe97ecd7db8037`  
		Last Modified: Mon, 06 Jul 2020 23:59:53 GMT  
		Size: 5.4 KB (5433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70c2b14b7f258300449b8979370e760c680e44a5b6a80ec3ea797c96288755f`  
		Last Modified: Thu, 23 Jul 2020 10:27:46 GMT  
		Size: 226.1 MB (226091456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c90cca289c4995af686e66360662fde839fd9627c3f2ef584554aace92c56b`  
		Last Modified: Thu, 23 Jul 2020 10:27:14 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
