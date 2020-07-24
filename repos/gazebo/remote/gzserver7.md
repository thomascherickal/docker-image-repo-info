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
