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
