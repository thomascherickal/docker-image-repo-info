## `buildpack-deps:xenial-scm`

```console
$ docker pull buildpack-deps@sha256:dfea081d2c9badedad7501874275c71fa449d3802c770f0c7d8a32401952c3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bdffd3de9058b91bf7ca86dc5d7b9e0028b9d0d894e630f23ef3c283e9e254b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96195328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433417de2a1ffff8b6c87633942faa9c8645ec88f7cb7a47c9a1d5f56b7e96dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:06:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:07:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42950b703a06b97a939a480237f84b19002bdea7a18b13134adc765328699d4d`  
		Last Modified: Tue, 31 Aug 2021 03:16:13 GMT  
		Size: 7.8 MB (7790543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2a7ae66eff85a2438aa0ea3586e8d8d638e66d1b32fe7d59a510cde54c2813`  
		Last Modified: Tue, 31 Aug 2021 03:16:30 GMT  
		Size: 41.9 MB (41905682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ca27f899fcaf5240abf6e29d84601c0c2def08b179b0441443c49d7d14f1f7a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85107802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49140e977ceeba1edff0140500feec7c945c1838c132e0dc78f30e976313320`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:25:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0c65fb267d23c5dd58ee3a818a8932a3fd565b8db9f6536fe98737a4e08f7`  
		Last Modified: Tue, 31 Aug 2021 03:44:48 GMT  
		Size: 6.6 MB (6631655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ffada20ea8521b2262a77a6239d4fc025f8f59d675a86c60923a075fb73d9d`  
		Last Modified: Tue, 31 Aug 2021 03:45:29 GMT  
		Size: 38.2 MB (38162364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:676194f83bf0884b02998c5e5783ba66882579a02a3da41de3a8180280f8f5d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87893278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a849f28400387145666eead1018792c030ac71ad4445140201f4e6395aee9178`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
# Sat, 16 Oct 2021 03:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77011f0e629af6f1792d3ccf59b89e6c06bb7f9a0f9ff78fee1d59ca55eda175`  
		Last Modified: Sat, 16 Oct 2021 03:24:02 GMT  
		Size: 6.8 MB (6837244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef3e23489d0258d8ea0afeec7d0eac6009020741bdee47ed1cae3fd5a9004fb`  
		Last Modified: Sat, 16 Oct 2021 03:24:19 GMT  
		Size: 39.8 MB (39815288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0bf6ac725a866c81afc2d4dbbdf5b3f90d502ea487f04992245dfbec7e4bc476
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96648619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a280aa8d673d47002a23857941e0d96ad26e57d7741b582565bd6378ef19f8c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:09:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc22e1425a6b0e2770426d0c67679ef683e74ee1abfa9a681dcfe10e1f0b6f5`  
		Last Modified: Tue, 29 Mar 2022 18:20:57 GMT  
		Size: 7.9 MB (7932472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12616572c59d50bf4880ffcf32efa0d4a77445cc92312e76d09815af78a7c88c`  
		Last Modified: Tue, 29 Mar 2022 18:21:17 GMT  
		Size: 42.9 MB (42898428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b14a5fb51b5d1ab5613940dea0f744f8a26a25e8961fea9dba6e27f06fb42984
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d669cab791289e0af0fcec78a739743372399e8bea4102312cd5ca1d5f4af1af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 04:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6ecbb79c70d45fca469278bf60d5e429f108594e71179f4a564aa3531b2d5`  
		Last Modified: Tue, 31 Aug 2021 05:34:20 GMT  
		Size: 7.7 MB (7693285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba12653da3d4e66d89f4d0e6e7f60832cda0b7b78d6a428c517d0479e4b892`  
		Last Modified: Tue, 31 Aug 2021 05:36:50 GMT  
		Size: 45.1 MB (45147268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a203418fa9ce17ec959479c3f6715d9ecc75466fd0aa528075e0cc9f94ec900a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94299319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c60d1962866a26c61283292dd8fbc87d1d75e3fb6c73d5f60070a001b7d67f40`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 02:41:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:41:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:41:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd8a6861a80aa4b11ce96ec3537844aec4b713e8074deacba0614cd64afaf6f`  
		Last Modified: Tue, 31 Aug 2021 02:48:46 GMT  
		Size: 7.5 MB (7522004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f08394215864198c62652fc16666081e5739d70caea25d4324e60bcab889`  
		Last Modified: Tue, 31 Aug 2021 02:49:00 GMT  
		Size: 42.7 MB (42688096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
