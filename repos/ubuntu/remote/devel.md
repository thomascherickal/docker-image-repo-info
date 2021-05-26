## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:4ead8f09d62038c60b69735e2ea80c6c9899ea2fc53302f8a8e741a0b0bca27c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d84cd5125ae611dc2c445d749dc66ebbcc8c1fc408a99cb86dc13798029cd94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29271688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3596f8231cb89fba11aeb2bbe100377741eedbe4e9c419cf288e3c59569d91b3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 May 2021 00:28:33 GMT
ADD file:d5bc80eba81f060df9f2dd1be5869c7a127a53c9b0dd1337429e5db64db2e21d in / 
# Wed, 26 May 2021 00:28:34 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:100df5f9ba4279983d5c0cf4e2af5c0cef347051ab124e7b8e5805986643be23`  
		Last Modified: Wed, 26 May 2021 00:29:58 GMT  
		Size: 29.3 MB (29271688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:73db11d76e9ec989301b0a5d801909bed3fc168eaec634f89609664b5373c8d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24751699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74080974911b33e7e514368c235c0e57d33c307c38289e8141700abbfd4b666`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:38:07 GMT
ADD file:95ba77e2e7d741cac32dfa843883123f6eb0ace2efcca42e737b837aa9e160e3 in / 
# Fri, 23 Apr 2021 22:38:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:38:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:38:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:38:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da3133366dbfe427412019fd1c881b3fe2a3b4f03a1a2be5c70eca2f0940e834`  
		Last Modified: Fri, 23 Apr 2021 22:40:47 GMT  
		Size: 24.8 MB (24750666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f53ef87823f7bf6f891f2f35f47a790b111f5723d2516ee832c89c4aa6c059`  
		Last Modified: Fri, 23 Apr 2021 22:40:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac517c3e752982cb73e75be840b5b1e5a56552655605b87986a66e287634641e`  
		Last Modified: Fri, 23 Apr 2021 22:40:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0fb0d395bd896ff4670143d0515fb431c638cf9accc7f543114e33b392700eb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27838449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ad5fe250d1b6d5ee7a6937868f72a4b5c385e983a2832f871091bd25e914dd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:48:37 GMT
ADD file:f6b776f11ca04a349ede73efde878cb528ec444a3a342a12ab4942dc9120a8d8 in / 
# Fri, 23 Apr 2021 22:48:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:48:44 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:48:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:48:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:30e34916c3b1ae71b2d4f4c80992d996fb7d9ed8857fa9da152f558e07ae5354`  
		Last Modified: Fri, 23 Apr 2021 22:50:42 GMT  
		Size: 27.8 MB (27837418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da710502d22348ee6d27834480cf8855c4332056fd5baafd5f8b6d4c91ab97e`  
		Last Modified: Fri, 23 Apr 2021 22:50:35 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c334551e118c3954ba6910ef0cf5783351985654b6102f50ec31460e7c0f671`  
		Last Modified: Fri, 23 Apr 2021 22:50:35 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:e0ef2d4838fd0db43ed79d7c45eb387617fec0f51dce6b265c35000d1e290081
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34455386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60293d749dce65c35d79d1a08a870dc2dc035e791a2cdab1abca28f04f3bd90e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 May 2021 00:52:49 GMT
ADD file:c5d7e177bf362b61dd9187e583d5d0aa642c875c2fb2492f079673fb28b3fbb5 in / 
# Wed, 26 May 2021 00:52:58 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1a4d25865ecd202be01ca270a8cd842c61f8f6810b7f4a1d189240ef71daf3e2`  
		Last Modified: Wed, 26 May 2021 00:54:50 GMT  
		Size: 34.5 MB (34455386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:7b3537b30ade96a1a6eb27221a5b59f551ade25c951eaabe944e0d0a6068cc96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30135000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65567937907f8ce293b6c8100d8aa15bad287b94b3331345001d6e2ece165742`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 May 2021 00:51:28 GMT
ADD file:446504b7aa924755689c59ea26a4da9eb765b2829b89dff4420b5e555cf07bd4 in / 
# Wed, 26 May 2021 00:51:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2e1f4a163d47bb20bf367360ebae18d87226492930220a94f44e4faf8d82557c`  
		Last Modified: Wed, 26 May 2021 00:52:40 GMT  
		Size: 30.1 MB (30135000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
