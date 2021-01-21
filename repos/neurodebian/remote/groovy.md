## `neurodebian:groovy`

```console
$ docker pull neurodebian@sha256:0e7e425f9be0e17c91620dd62623f067f93722011d13bf4126245535fb6e0a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:groovy` - linux; amd64

```console
$ docker pull neurodebian@sha256:b2a36f1d9e4730e4e65394f729400d163c2b5ff75e43dbf38304d40b0f788bce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37183031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14932f0788c3c606fb77b942ebcd99d793da2f586a35d9e23e2b742a35384f97`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:40 GMT
ADD file:fbf1e6b04a66bc3f4ff7a5c599fa18604caee5c848328ae120a4a97d3e4636fe in / 
# Thu, 21 Jan 2021 03:38:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:44 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:10:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 10:10:56 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 21 Jan 2021 10:10:57 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian groovy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel groovy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 21 Jan 2021 10:11:01 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a09400eba642b8443b0196d54f94bd75bb9e0ca23fae24e945ce8ef12237f09e`  
		Last Modified: Mon, 18 Jan 2021 17:32:09 GMT  
		Size: 31.3 MB (31348186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcab926b54c7b115b820e2ea38ae0a659bf65a31345459bd404c3780b024a6a`  
		Last Modified: Thu, 21 Jan 2021 03:40:49 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c1d05f510d7751d87a8115e0e927385901b2f17d1838902a51fd902cf855c3`  
		Last Modified: Thu, 21 Jan 2021 03:40:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6a6fc470460bd48cc8bb7cf3e3e388ce4ee11b8dfcdcd8337a389339fe5201`  
		Last Modified: Thu, 21 Jan 2021 10:13:07 GMT  
		Size: 5.6 MB (5577822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da51dc2c12e605333e3578b092cb1f164ff8e12007b0965cce91688aa220f5c1`  
		Last Modified: Thu, 21 Jan 2021 10:13:08 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fc325c585e6ce451d48787873f05a6dbb652dff5df65eb30b821d029c07b9c`  
		Last Modified: Thu, 21 Jan 2021 10:13:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f637eea958ec225d291acaec7c5d734dbb0257943cdf45f906ec0e03c234d9d3`  
		Last Modified: Thu, 21 Jan 2021 10:13:06 GMT  
		Size: 254.0 KB (254006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
