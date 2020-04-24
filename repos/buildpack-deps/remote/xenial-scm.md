## `buildpack-deps:xenial-scm`

```console
$ docker pull buildpack-deps@sha256:61b97c0783e7543995410610ad1abf2b65badac98a2ab49d825d23a9490c3a02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b70edbfe4a2d02d44d7e6a6a6557e497ce3e8220a29d613fde2237ea2e0e941b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93363301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b023953f4b010e2d43bd532d0d025de5585f8ac9c6c9920cd70c599b62ec5c2e`
-	Default Command: `["\/bin\/bash"]`

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
# Fri, 21 Feb 2020 23:00:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:00:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 21 Feb 2020 23:01:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3331c6158137ed51eddd9309ab74a6fdb1353c9ea3e1c18a8ecd1936ee76cf64`  
		Last Modified: Fri, 21 Feb 2020 23:05:15 GMT  
		Size: 7.3 MB (7324657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a91de9878ceb704d390861b38bd32ed316e7bf4e180f47678d7134c36fc31`  
		Last Modified: Fri, 21 Feb 2020 23:05:29 GMT  
		Size: 41.8 MB (41845373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9fe96af329a7dbc7a6dbd73e7acfbc7bfdcdf9adeda673506c170f6e22ad38c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83219132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5926bafdcc9d5253ebfe24ec9ffbd9925e6cb391cca615134f081b1252b60a00`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:07:55 GMT
ADD file:baa32b9dff77005bab52997f1dcb9df3558abb0e2ef834cc2d09fd2f9b199f75 in / 
# Thu, 23 Apr 2020 22:07:58 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 22:08:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:08:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:08:03 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 12:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:42:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 12:43:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:471714e6acf6feae8152818c3e754b9ca6a0bb98630e01ccc7f3a11b3c167d67`  
		Last Modified: Mon, 30 Mar 2020 15:50:01 GMT  
		Size: 38.9 MB (38921731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452137b54c197f3f182da5f3c8f8464b32e21e6023206fc84f1973bd7b5d6d0e`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba3c36f61e095df847ba29ce216ff56b6cef111df85728fe0dee190fc49193d`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414dfa5050bda9cc1932154a5ad6031f727ff248a9098137827aa48f60e11ceb`  
		Last Modified: Thu, 23 Apr 2020 22:08:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841aa23d6599ae2238137bb7432acda2e1a364e1f074a3ebcf4c48e51a79dd44`  
		Last Modified: Fri, 24 Apr 2020 12:49:40 GMT  
		Size: 6.2 MB (6176586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7c192049bf73793e74b6fc0539de899e0620093be56e21606a6988c7461e07`  
		Last Modified: Fri, 24 Apr 2020 12:50:00 GMT  
		Size: 38.1 MB (38119280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ea4737fad88f1e4ba386e32da1438736226d9f161631a6d4b42a9a46cf151df8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86120752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6e4b46321a05dda460e0bf495285df93ffb15bb57fd1e51f7fec459a3964167`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:20:42 GMT
ADD file:24038b6c5a9bab991785fab56202fc43de85e0749e57fcfc361de8aeff302309 in / 
# Fri, 24 Apr 2020 00:20:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 00:20:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:20:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:20:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:08:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:08:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 16:09:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca96533948cdaf1fc84922a44248fcf915a3f526b46555bb96090bed658b00d7`  
		Last Modified: Mon, 30 Mar 2020 15:49:17 GMT  
		Size: 40.0 MB (39968791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72780e1c95403020a1883a1054d9d48b7a5ad2d940ba2d57ae211369a19685`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d962f0171bca79269769ac242507e3f65f2dcbb86de35ecaf164d37b8a89c9d`  
		Last Modified: Fri, 24 Apr 2020 00:22:16 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f057dc5a95fd6368cf61fa48d9e2d85af21b750813b8dd17b7ad44752c342`  
		Last Modified: Fri, 24 Apr 2020 00:22:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413a3162bc1fc442d4ba8ba4d108eeaa5910895d7693a341c939ada991f6c2e8`  
		Last Modified: Fri, 24 Apr 2020 16:14:59 GMT  
		Size: 6.4 MB (6383097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dcc34af97c322feaf5b84a7dbc3913fa56e943435d1675a0dd78b52027e6d5`  
		Last Modified: Fri, 24 Apr 2020 16:15:17 GMT  
		Size: 39.8 MB (39767368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ee7f55d214309fa7c6bb4064051f523e05ff1788e39cafb760efae90fbe41aa1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94517730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2596d12fa2f1a764fed1fefdf6e7d907511fd245caf0b96069bc239697e938`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 21:17:40 GMT
ADD file:63f010395531a9f80a46467e101e5faaa15a956b549c08a6afd70b8d5d3e945e in / 
# Thu, 23 Apr 2020 21:17:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:17:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 21:17:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 21:17:42 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 09:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 09:09:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 09:10:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67d49c13ed2c9b289158b085c6215fe67ea17345ad7e834ef26e977647696056`  
		Last Modified: Mon, 30 Mar 2020 15:50:14 GMT  
		Size: 44.2 MB (44207533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a69e39cf53088b87506229493af61c0a92bca912a530bf3e25ed7180e134125`  
		Last Modified: Thu, 23 Apr 2020 21:18:16 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf9f29b646ffc24e96fe13309b5425714730ef1ac579a37a818da98bdc13`  
		Last Modified: Thu, 23 Apr 2020 21:18:16 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805827cce86a04c12e994125c6504f76a3f2c41b32658608484bd2a41f1434f1`  
		Last Modified: Thu, 23 Apr 2020 21:18:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f7c0f7edb4ece93eb5fcaf0238b956cfa6d075d880ba97879218e2431bbb83`  
		Last Modified: Fri, 24 Apr 2020 09:15:08 GMT  
		Size: 7.5 MB (7470605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639992f9ebdccb4b88e1d0e0f000f41ae6e0abd5b2cf00097a9e4c84221ea49`  
		Last Modified: Fri, 24 Apr 2020 09:15:23 GMT  
		Size: 42.8 MB (42838059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:79eeb69aa6843df27832bab5303c1ac606b71b8b1ae67f6abd3b2fd494a35e74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.5 MB (98479906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b0216426d4ce6da0fcacbfa9a98a000d2171d16cc95592e8578d264242b535`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 20:48:01 GMT
ADD file:36cf2a50881947cc8930a57622516abb7c57b5f24a66ea99dce0eed8062a6f60 in / 
# Thu, 23 Apr 2020 20:48:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 20:48:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:48:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:48:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 13:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 13:01:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 13:03:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b169ceddcd2a39f266f90393bc1b86eec3b7639eed8f2284fabe5f3402dca04`  
		Last Modified: Mon, 30 Mar 2020 15:50:14 GMT  
		Size: 46.1 MB (46128683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19601b8798de70175c84541058fcdfd77b3ea7f541b65d8b79e509877f5153c`  
		Last Modified: Thu, 23 Apr 2020 20:50:26 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db330d3fb72bb26806c74ea2d3c7dbb9ddfef3ddeb4b7ea1814c457c96433ce1`  
		Last Modified: Thu, 23 Apr 2020 20:50:26 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffd1d80f6cae6e0eb2f96dff6b6ea6d77dc712a10d80aaa539341bffbbee980`  
		Last Modified: Thu, 23 Apr 2020 20:50:26 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b9490ec0ab56616f43ef5d6f7eb246f361225ad148acf76635056d20cbd98`  
		Last Modified: Fri, 24 Apr 2020 13:24:35 GMT  
		Size: 7.2 MB (7233765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05932042d145fdfa66792b3d0ab6914f859a7fe9b693bb3f5f5f4ac3f313464d`  
		Last Modified: Fri, 24 Apr 2020 13:25:10 GMT  
		Size: 45.1 MB (45115966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e1e0670df79d79a08344dfc2bbe4cdaf143bf47436c1383339dc7c296bde5557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92555710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3345d1253c7f1ee83dc2252156077ea74c1046a9de96ce465fce01024704d5c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 17:53:43 GMT
ADD file:ed32a6507ce62172a75daf32a3e745ad7d8e5ec2c72a0dbeb1ad18af3be6cde8 in / 
# Thu, 23 Apr 2020 17:53:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 17:53:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:53:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:53:58 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:52:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 07:53:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68931fb1bceafcc32dd3b6ff5116133bbd2be9aad34c04cc81a270dca82df13`  
		Last Modified: Mon, 30 Mar 2020 15:50:44 GMT  
		Size: 42.8 MB (42840710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febc54d02b58a20f824a7c8503ccc8d35a35482936d8dc59dfe0adc3359e1fb7`  
		Last Modified: Thu, 23 Apr 2020 17:54:52 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aed9cad1309eeb57273b441dc4661e5f3dd6055d9960dad401eebfa93f6178`  
		Last Modified: Thu, 23 Apr 2020 17:54:52 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e342d8c62e47069f917221bdd6d21bf7ccab595f1d2feab7554cb3ae93d86b`  
		Last Modified: Thu, 23 Apr 2020 17:54:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d397414e6f5a0ba42f19b6dcbf646decbe786620da4f8de5865c81eeca24ca4b`  
		Last Modified: Fri, 24 Apr 2020 07:56:57 GMT  
		Size: 7.1 MB (7063576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5489aefbafe20dab3dc54fb7c03c6a1174ca8334be198282921e3e9ec4e7fa`  
		Last Modified: Fri, 24 Apr 2020 07:57:09 GMT  
		Size: 42.6 MB (42649931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
