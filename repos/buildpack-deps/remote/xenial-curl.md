## `buildpack-deps:xenial-curl`

```console
$ docker pull buildpack-deps@sha256:a7bb8952cdc5f76df5e52935ca541fd1a7275ebbd8006359935446c427b0e27e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4bafd979210b581f9ea1ecc2380cc56fd41d9c7e3c24fcea45b9d1dff9919bfb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51517928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0befc51610f7ca77bc4f1e0df71d03b10eead4ad9f0edd0507f276f229610a`
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

### `buildpack-deps:xenial-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8b289b271c48cccf2ce016598ecadf379d67692dc55f49d66827862740975b21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45099852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7657817910bbedbc6404ed4a68261ff967f40916d3fbf60fcf1b01b837aa866f`
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

### `buildpack-deps:xenial-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:570f47d8b0b22111b9fc849c3fa6f215fc1e7c8bf6cb963a06cd5c12f1e33677
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46353384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f357bc6c93c6540d717812aa18780d5704348df6c5690dc4f777f08288efb16a`
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

### `buildpack-deps:xenial-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5149bdd71f4a0b6c7eea285e8a126a02ddf28f304a14c179a2b1fb7ba65f64cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51679671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c09ce4203ab2e99d38eb6f480c7ed6bbe109bb9f14fc81b74878c87502d5f990`
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

### `buildpack-deps:xenial-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:62f42f17e00078735c1f3974e48b1e279990554c42fafaf9b03c10d7778b8b36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53363940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d721f1dc3deadd4b408ac2aaa5867c158286700fe444595a1a6a19927544575`
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

### `buildpack-deps:xenial-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:31b194f325b83e3a7fcf8296d6d737b1e261253c92cef01bf2e32bc8c81f61a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49905779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2feead81f9fea37b3a9c0f6aff585b2f518b1c3239e3f237687e48f3d6a892`
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
