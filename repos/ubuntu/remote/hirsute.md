## `ubuntu:hirsute`

```console
$ docker pull ubuntu@sha256:414bafe37ddfc22fe0f0ceac1c89d563ee3570afbd2e7aa09ad8939ca6fdfa98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:hirsute` - linux; amd64

```console
$ docker pull ubuntu@sha256:72b52c13d7462c156eb0ce608d7b3cc11ab1e0def275f4ea5ee0cbfd73202164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29265746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:478aa0080b6031764323f8d008dcd464f2c245b25a0afa280ed6939cf50a7162`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:28:22 GMT
ADD file:d6b6ba642344138dc401cd05c31eb2c55db70b91adba5f1bf9c4957a1f3caa64 in / 
# Wed, 26 May 2021 00:28:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:28:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:28:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:28:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c1f3479a03a77c31a1fcea35586db9f477549808f1ddb67b7959de75acdcf1c`  
		Last Modified: Sat, 22 May 2021 22:09:18 GMT  
		Size: 29.3 MB (29264710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb3aea4da4440192e04f2fa4312068162c04670b12df1e5e78903117a38e83`  
		Last Modified: Wed, 26 May 2021 00:29:35 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfcfbcbcd594e06620ea6ce7ec8437e406eeae995e9733d18c9fcfc43c46f32`  
		Last Modified: Wed, 26 May 2021 00:29:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2581c675b3727523ea723a0d9a99361a547d03743bd2820cbe58eb48355eac2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.8 MB (24752518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0d7dd9f74332a1c61c6832ec49514acadb6838d0d8033d4e13496c52db4a4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:22:48 GMT
ADD file:e5870ac6e64d788a9ed34c217ecc70648386b8ffc1fb0bbba393155bb7f93437 in / 
# Wed, 19 May 2021 20:22:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:22:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bdd4355f13aa64cacc203ae21d7f6b50c13e90d4ddce9ce1e27ae5aa46cbdd31`  
		Last Modified: Wed, 19 May 2021 20:24:29 GMT  
		Size: 24.8 MB (24751484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8651e11b134edeb4fc951dd121afc6fedf7810f5b2cd90819169fe4abe4d7f`  
		Last Modified: Wed, 19 May 2021 20:24:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6614e7e3c4bd3c9c88b4b28c2ec82a93cf94d5d20cb70a3c944b0f0b2827234c`  
		Last Modified: Wed, 19 May 2021 20:24:23 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; arm64 variant v8

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

### `ubuntu:hirsute` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:518c4deb62bb24f16ef27092d722f211dfe5cbb51f7161f7e1deb3b570dc3b91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34381785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49de090b308a0045bb0804ead12592145ea26bfa2e69bd782524473f3c706658`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:51:50 GMT
ADD file:e80f8df1e69f3cc62d297d2337050d46d08274bd08383e6b1cfec16b925db697 in / 
# Wed, 26 May 2021 00:52:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:52:17 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:52:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:52:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:252891cebe08be4f0264d55f9ed858c2f005caf8d57d258d3c85a7d668387e21`  
		Last Modified: Wed, 26 May 2021 00:54:28 GMT  
		Size: 34.4 MB (34380745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6148b678f2af4b9a14130b1d455bb78e63b7a5fc976ae4e17b8e6fc393fa7a`  
		Last Modified: Wed, 26 May 2021 00:54:21 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485fb0831782def43c7530718335d921b98ebdd3a2ad70d5b453fbb10740ce1b`  
		Last Modified: Wed, 26 May 2021 00:54:21 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; s390x

```console
$ docker pull ubuntu@sha256:20325bd173273e78e8232c6cac753ce46dee387e1330c13127a1c429cedd1bdb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30109413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33d726f342bbc2baa179d4632c3d13e5cbd9a2d5a1e86430c4c0cf2795c7cc6b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:51:07 GMT
ADD file:795bcdfce02a31d768bd13e27acd7326ee51b012ec456686a18bdfca3f4ca610 in / 
# Wed, 26 May 2021 00:51:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:51:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:51:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:51:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d3e7812f2b888ad62db31dfece570fa7b8cc2d413aa236dec496f283510d6ce`  
		Last Modified: Wed, 26 May 2021 00:52:27 GMT  
		Size: 30.1 MB (30108378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fce8a5ccf078c1d3b79ccee8bd06e5b39c0cda50aded87d3b48574cfa72b6e`  
		Last Modified: Wed, 26 May 2021 00:52:23 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282417fb7eb197857a0dd6886c03a59029db8f5f4ed6bbc213203ff92082decb`  
		Last Modified: Wed, 26 May 2021 00:52:23 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
