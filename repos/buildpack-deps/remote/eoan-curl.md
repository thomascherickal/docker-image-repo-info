## `buildpack-deps:eoan-curl`

```console
$ docker pull buildpack-deps@sha256:ab372b0dfe50aee18b9050306c393a9cfb3e7558ff7b5f705d841452e050e664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:eoan-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5ad44c8392491696d6e3fa16ecb308c14bdc3201ed2574bf89e58a11dfa69199
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38338393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe6177a1712075021ac46916b6c75989eb92721e9ff3ec5db690af123f96c1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:21:11 GMT
ADD file:49bd1c0bfe89a93a193774bfd334bc1151f0dca95849f81d1ac353673399585c in / 
# Fri, 21 Feb 2020 22:21:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:21:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:21:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:21:16 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a9c68053c4b2379a9ad5b7306236a13f469cfd18e727dd4e76470af366445b45`  
		Last Modified: Mon, 10 Feb 2020 15:41:51 GMT  
		Size: 28.3 MB (28276663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9c43fe7e5dcfee42adb18336072154126bc052cc1c578e64d27a8aeaabc97`  
		Last Modified: Fri, 21 Feb 2020 22:23:01 GMT  
		Size: 30.6 KB (30633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90491034717d4c1d1e0b37a4bde4f3a0e26630af7d360b7c0248660ccbef59d5`  
		Last Modified: Fri, 21 Feb 2020 22:23:01 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781c6270286751c77c20928c68fa3edd532f0d3d11108db32020c8840f0ea6cb`  
		Last Modified: Fri, 21 Feb 2020 22:23:01 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73542a256b5ee66b5f38af9d7c37a2d5d03c3ed228335a54f0b9c4c556f2c45b`  
		Last Modified: Fri, 21 Feb 2020 23:04:21 GMT  
		Size: 6.5 MB (6512504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf9e73f3647faef689dc3183ba6ffe693631be3039058b42f3b7c177b97962`  
		Last Modified: Fri, 21 Feb 2020 23:04:21 GMT  
		Size: 3.5 MB (3517579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f4b8aeb1e14f0bc8d94eeacc2be67df5f3b35ef40d35050c0c0f38ea73903422
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32282216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df2d679bbab74f9d6b430cf0791abbb863ebcf1f44b2a7140dc486220152e12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:05:21 GMT
ADD file:cd4de1fcdceb95824a887d3d27d3c110261a719ded9d99031dd00e1568494c4a in / 
# Fri, 21 Feb 2020 22:05:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:05:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:05:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:05:31 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:16:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:16:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bd94fa49cb09c9859edca1e49f6f1cbac0fd492ae56f34b62332a783ad7b68d7`  
		Last Modified: Mon, 10 Feb 2020 15:42:56 GMT  
		Size: 23.7 MB (23736258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1ca8c199cca8211202b60f587659b529101b98194226cb6735febcac6db3f9`  
		Last Modified: Fri, 21 Feb 2020 22:07:02 GMT  
		Size: 30.6 KB (30612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefecf0dd0df3e68f7f80336d560e65ce665036fe83576e4f801047dfd4a9d9f`  
		Last Modified: Fri, 21 Feb 2020 22:07:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017e57ad339bf8ddfdfd30a79d5096b13c3886781f1078e0303a89cb818f539`  
		Last Modified: Fri, 21 Feb 2020 22:07:02 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6ffc1b31e2df48f8fc4f545708210e564b027a7d98fc57ad046444eeae6bdc`  
		Last Modified: Fri, 21 Feb 2020 23:25:53 GMT  
		Size: 5.5 MB (5531419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d3f5ffdbd8ee19bb0acc962cb7c670533b3f80522e35251e34c82611024402`  
		Last Modified: Fri, 21 Feb 2020 23:25:53 GMT  
		Size: 3.0 MB (2982887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88f3fe5a70760de24b63202120d9a60881a1814e2618643f380b2841a5cafc34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36782385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08ad2c258549f523516246c4af4bbd9b30d3abf918cbb51a0557972cfe08e46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:42 GMT
ADD file:29003dce8015529919e9efa92862cda5f1c4a394bebe00e7d9bca8894f23bad2 in / 
# Fri, 21 Feb 2020 21:54:45 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:29:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:29:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79693b41cb22c8dae6603b2bf443392e179fff02152f5b8fb25e9ebc2f36ca37`  
		Last Modified: Mon, 10 Feb 2020 15:42:23 GMT  
		Size: 26.9 MB (26869627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085004cd2eaec5c5d7d85da739c356d4035b607ff5d3fa3de249827468ac04e4`  
		Last Modified: Fri, 21 Feb 2020 21:56:23 GMT  
		Size: 30.5 KB (30457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9727781305391dcb29dd0f8d61651a751c07d2a32abd0c1ce145117a9416eca`  
		Last Modified: Fri, 21 Feb 2020 21:56:23 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a75366ff852d9cfecac92c78537e6ac39629896a81c09dd9051a924c9363573`  
		Last Modified: Fri, 21 Feb 2020 21:56:23 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3378312c72f98443e87d4051ec0db1f3d85aa111bba210b2f15b1e10d701bb77`  
		Last Modified: Fri, 21 Feb 2020 22:38:50 GMT  
		Size: 6.4 MB (6369837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5141314bdd69c63c2fd6a3262a3bac36c37848ec9fd9f9f76305d5269ce7b`  
		Last Modified: Fri, 21 Feb 2020 22:38:50 GMT  
		Size: 3.5 MB (3511427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8b3c4187f1a2b09dfee75beb27dc95215c36b80cd5b9947f3e6c1f237d6837b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39727193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9ac26f02cacb7e57fd2fdc3cb9017300b31af4bd48889da7fb596d8831a840`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:17 GMT
ADD file:8712d700c1cc817afa2abe23b077498c4ec2332067a7d38e5d3425454373e193 in / 
# Fri, 21 Feb 2020 21:39:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:20 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:03:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:03:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:df36fe298056793eae27d9efb7b1d54a4d69b16ad6a7d62fc186a8e7727db39f`  
		Last Modified: Mon, 10 Feb 2020 15:43:00 GMT  
		Size: 29.0 MB (29044887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b3578b2a446d70c838e7144c5d77d423461b43e78e2e75107f2764511bed0e`  
		Last Modified: Fri, 21 Feb 2020 21:40:03 GMT  
		Size: 30.7 KB (30699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb0394aa2bb495dd3bef1779832e0d27d6d292aaf3f2740c17564759aa47ef2`  
		Last Modified: Fri, 21 Feb 2020 21:40:04 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e86bd657e678ce69ee3e2c2e502097c3353cd8484841245225e4d598489c3`  
		Last Modified: Fri, 21 Feb 2020 21:40:04 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b3c4a9b0c5109888bf628b4611fceac5c22405d7191997b2878481e6738a42`  
		Last Modified: Fri, 21 Feb 2020 22:11:55 GMT  
		Size: 6.8 MB (6840425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c27386cdeb7336876d79f1601770fcc1d4e95c170201adb4411c5b89012e`  
		Last Modified: Fri, 21 Feb 2020 22:11:54 GMT  
		Size: 3.8 MB (3810172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c03e944f856f61687fca0e5c163fd5756286da2b63016e5ea2f912061881e12e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44901138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10290a63f561b52fde0cc7c8d4624115bb72f1124f752fc8f7de921e0f7f5bdc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:31:25 GMT
ADD file:d3168601bc3d213abcd3bb57ad2824d9099de51d8775c8d356460e12d15a26a1 in / 
# Fri, 21 Feb 2020 22:31:31 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:31:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:31:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:31:43 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:02:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:03:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:051dbc8b8e4ed99bbd1a698a7e4bd348c280e0ddaf417786fbedd99ca22cb144`  
		Last Modified: Mon, 10 Feb 2020 15:43:20 GMT  
		Size: 33.0 MB (32986499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f53f3c55500976229df5bc71ead0d2723cda57b2c606b6e906de3b7b5c2ad80`  
		Last Modified: Fri, 21 Feb 2020 22:33:32 GMT  
		Size: 30.5 KB (30477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8143f400347b6df364214d634dbcd1db12d526040a868183289501481e13f05`  
		Last Modified: Fri, 21 Feb 2020 22:33:32 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd6e204830d0f5b1439e36d1a6af90c8b04d96fb8b4bcacdd6f611706a97881`  
		Last Modified: Fri, 21 Feb 2020 22:33:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd064f9cfd83a46d8aefd85c1839261286088ce49c7ed0b6a49bc9f488ba789`  
		Last Modified: Fri, 21 Feb 2020 23:30:53 GMT  
		Size: 7.4 MB (7419981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74726e386bdfae67f0944edb98035484c91063bc63699525f6091848d0f79495`  
		Last Modified: Fri, 21 Feb 2020 23:30:52 GMT  
		Size: 4.5 MB (4463145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60a3d39a01cda1fd891934038b11ff33d21fc196eb62a07cfc5e20fb75b3cd58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36287097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5f0a1ebd163e824af3e0a19a32eb6c02e2ac9aa10ee64ccc0279b7cd77c689`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:58:06 GMT
ADD file:14df51909823644041c1e18fdd62b5c5598c3f037712b7a3db85d68d65c12f9a in / 
# Fri, 21 Feb 2020 21:58:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:58:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:58:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:58:15 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:20:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cb19e5b8123e1f3303c72ff2231d83a7282d4d798635f63093ee0c6329d5bf4b`  
		Last Modified: Mon, 10 Feb 2020 15:44:30 GMT  
		Size: 26.7 MB (26682544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ad82f1f4a65553adb6d26ef9b25aebaacb039124b98ba6867d7a27d8dc25f9`  
		Last Modified: Fri, 21 Feb 2020 21:59:28 GMT  
		Size: 31.1 KB (31106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a7e86bc0f07353acc2cc206b74b5d9825041b4fbd0c0b8de71419ec7b661b`  
		Last Modified: Fri, 21 Feb 2020 21:59:33 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7cae483f07e12cbe0fc9a0bc8dceaecbe7ec0fa3ed9215d663ec3ac10210ab`  
		Last Modified: Fri, 21 Feb 2020 21:59:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e533675a7fe83acca2c0df5bb786e6cc3b72c9c74135ad38dc79b9dadc4890`  
		Last Modified: Fri, 21 Feb 2020 22:29:07 GMT  
		Size: 6.1 MB (6138768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438f3eeb739190fa225248b54833867634881c0b1717f8feaa406b843d65aa4d`  
		Last Modified: Fri, 21 Feb 2020 22:29:07 GMT  
		Size: 3.4 MB (3433644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
