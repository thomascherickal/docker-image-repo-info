## `gazebo:gzserver9-xenial`

```console
$ docker pull gazebo@sha256:1c7c2b5ab2203835c7cca577b673498461508751f37958c3b2d980174192ca87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-xenial` - linux; amd64

```console
$ docker pull gazebo@sha256:dad0d5186fc06dc096fd821fe260ef1e692dd3a240c2b85b05a555ac7346a67d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269052831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca4cfd5cce31c6468303030c090792db43e54a148666a1e7097a46dc3a18db45`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 25 Sep 2020 22:36:27 GMT
ADD file:23a55d7e93b396e490b6d0893137e5c13e3e0a234e0feaea8b1cfd4079fb1882 in / 
# Fri, 25 Sep 2020 22:36:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:36:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:36:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:36:29 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:57:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:57:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 25 Sep 2020 23:57:04 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 26 Sep 2020 00:01:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:01:47 GMT
EXPOSE 11345
# Sat, 26 Sep 2020 00:01:47 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 26 Sep 2020 00:01:47 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 26 Sep 2020 00:01:47 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:4f53fa4d2cf0e29c6a522433e0ac71a7ce0fdab158481052b2198b5518b83248`  
		Last Modified: Thu, 17 Sep 2020 13:19:58 GMT  
		Size: 44.5 MB (44517215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af7c939e38e8e3160fbbdcc26a32669529b962c79f7337df0a26bf0e9a76d59`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903d0ffd64f6ca1355d2b2df702fc674f5663981dfd100fe4588fb390dd3382c`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04feeed388b71fdca5cc3bce619d65a34f8a1a3e5b0ef03f8392d499970818eb`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b70b5a1be5191bcbbabc32361baec01217ac50735cc38ae44bb25f2f09d84fa`  
		Last Modified: Sat, 26 Sep 2020 00:23:20 GMT  
		Size: 16.3 MB (16275082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19428414bb03aa2f943ff6877240a2d568fbf131c40a5a849b9227d329ba61ff`  
		Last Modified: Sat, 26 Sep 2020 00:23:16 GMT  
		Size: 14.8 KB (14758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee4e38c9c19dd15bb438f3d405e6f5cdf9b34a239a33f9c504fc17c1a521b91`  
		Last Modified: Sat, 26 Sep 2020 00:23:16 GMT  
		Size: 5.5 KB (5522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1c4ee0aa71b7ff23fed34e3c62c04661b46ec38ab4e163196a1f8d9c8460d4`  
		Last Modified: Sat, 26 Sep 2020 00:25:43 GMT  
		Size: 208.2 MB (208238519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeafcc363355e6d13d5b078df374354c63d6ffa82abf2b122eaefd282db6dea`  
		Last Modified: Sat, 26 Sep 2020 00:24:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
