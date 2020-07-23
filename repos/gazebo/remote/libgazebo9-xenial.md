## `gazebo:libgazebo9-xenial`

```console
$ docker pull gazebo@sha256:df98a45a3a63f463f77ac37f648b9e162f0917d319a86a45522ee1aef10b136d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:371aa3bbac91d0512c1314f3577b4c86de1416fdbae8855dc9b23ce5f1657bba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **498.6 MB (498626474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18e897f86838233fb82697e8799c277f5fd737ffd5187c72e0a92cf5696cd53`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:38:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:38:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Mon, 06 Jul 2020 23:38:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Jul 2020 10:15:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 10:15:17 GMT
EXPOSE 11345
# Thu, 23 Jul 2020 10:15:17 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Jul 2020 10:15:17 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Jul 2020 10:15:17 GMT
CMD ["gzserver"]
# Thu, 23 Jul 2020 10:17:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5cf68a450f23523f4abc320a9589ae21d259e4826cabde9835d9e3c670f708`  
		Last Modified: Mon, 06 Jul 2020 23:58:34 GMT  
		Size: 16.3 MB (16275999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63d4e2fbe4dcacbe3c4c73dd65f8715cba308198c0de49741480263fee63558`  
		Last Modified: Mon, 06 Jul 2020 23:58:26 GMT  
		Size: 14.8 KB (14757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccb1e4b56b217f92ca1a91d15fef5204e35e7c15c5ff00a19b3d7e80d02d352`  
		Last Modified: Mon, 06 Jul 2020 23:58:26 GMT  
		Size: 5.5 KB (5519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc138f296114a2d12d2450f8d62459d6f5be9dac12d52d4172ca8cb9e7b5148f`  
		Last Modified: Thu, 23 Jul 2020 10:26:23 GMT  
		Size: 208.2 MB (208229216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf4c2408ec02811753cb95a00614f759e749ca6476150d2b5edfced63724cb4`  
		Last Modified: Thu, 23 Jul 2020 10:25:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8cb5cb1c6b7bcbdcd242c841bb2e1a1a3e85991ba99acff07e70cbc9bb6364`  
		Last Modified: Thu, 23 Jul 2020 10:27:11 GMT  
		Size: 229.7 MB (229725096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
