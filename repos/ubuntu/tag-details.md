<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:14.04`](#ubuntu1404)
-	[`ubuntu:16.04`](#ubuntu1604)
-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20220829`](#ubuntubionic-20220829)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20220826`](#ubuntufocal-20220826)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20220815`](#ubuntujammy-20220815)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20220830`](#ubuntukinetic-20220830)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:rolling`](#ubunturolling)
-	[`ubuntu:trusty`](#ubuntutrusty)
-	[`ubuntu:trusty-20191217`](#ubuntutrusty-20191217)
-	[`ubuntu:xenial`](#ubuntuxenial)
-	[`ubuntu:xenial-20210804`](#ubuntuxenial-20210804)

## `ubuntu:14.04`

```console
$ docker pull ubuntu@sha256:d7a459ecd77ebb09525584f2c3e1bb7f6a2879d90df8a3523c1b899dfc2a226f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:14.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d34202d0ce9f1a55b9fffa1d69af2821dcf9645cc655e96a5b168c2a9265d5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a7f3400ca032052bf769658a0a6f7562e441504c7da16527defa818a24fcf0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:30 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 02 Aug 2022 01:41:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:41:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430e3e7a1afcac7bf89d27c42804489d76ac8775a945924494e9e5794f0ce6`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 76.8 KB (76779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8c3e99facaf81b42b2e4e24792e7254297607e2273054e5f729712163cafc2`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:209f78eaf05254c51cff7676b913bcb70c1da54e58ae728a592ea58f3b5552b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd23a098588cb567106c63829bf08759e87f4235bbd4c90168e6b065420ac853`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:42 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 02 Aug 2022 01:31:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:31:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:31:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:31:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736dbcbc0bcb73948970c71c59c6fc5662698a0cdca10a232da87ede89aabeef`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 63.4 KB (63436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376b7bbeb4d42e6e9b75e9ad5bd043790235c8963cac05a03bc5400002ae965b`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:16.04`

```console
$ docker pull ubuntu@sha256:91bd29a464fdabfcf44e29e1f2a5f213c6dfa750b6290e40dd6998ac79da3c41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:16.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
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

### `ubuntu:16.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:696252dd941a9a0ca7db7ca8d9fbb91d838cc9bfb27403219953af6750a89111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20832692ca6e913217051aa57084ec76c076987a63cd497100d754b27097fa33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
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

### `ubuntu:16.04` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:4ef33ed6b1af10706727d280de436bced5e9413cba7992d6126c866efd79cacd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fb9d3bc97649795df6522739036df75814819b4b48997a6e05345dcd5e6845`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
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

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:3aa2ccb021969aadb28381fee1b247422e845b176e241cd1540c4b6831e000bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:ee1b6a6b513d6db9a14cf6e6d37895a7c70008d313d08cdf66e07cf617a3b978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26710085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476c64862aa8439ac32236e4dc7b2f35cffa748dd99565fcddd667f4994542e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1a9c90d5d959416422d50c65cd2b24dc8b7d596fd649c4249e814af97e47670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22305684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970ccdd609a88639212f12744557025bdeed28e800b788ea1cd908c252669a4f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:11 GMT
ADD file:93826239c43c79f307094d84d6fc79733e950dc0c0a332320254a2328eb5fff9 in / 
# Fri, 02 Sep 2022 06:08:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7347571ddfc71927a9f2ae03da3d05d7d68457aa24b5e18b6c7545fb65f4d034`  
		Last Modified: Fri, 02 Sep 2022 06:09:59 GMT  
		Size: 22.3 MB (22305684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:661c9525f2db5469c6fcb9e546442e62a1c7283ca0be7b0baa264c2f4b08dd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23734081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:487e1fdc39b6c9bf754e585f705e8e35c7fd30b88344a789010cfeb7919e68fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:919f05157e3a494086924aa02abe04f5fc08e84b41274c6a5549a996ac6ad530
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdc7dbece30f75bd7c19a0d9ec57c1b7724391304ad2db6a6e993a4c2160a3a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0fc175b31379070ddcfffdb1bfdc1f85d1f334ca9b784ab7baf94dcbf6457649
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30441333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6d9a8764c5e4bf91381594004243e6e44647dfc5c283cc002addb85ca8755`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:38 GMT
ADD file:57b462f3139cb98a97a7020f0d1be33f5beb6500115500a9bfd7aaec39854e35 in / 
# Thu, 01 Sep 2022 23:49:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c48fbbfad89e07e20864186f593c37c87089700f93ddb1b88e1912f891bf3ae2`  
		Last Modified: Thu, 01 Sep 2022 23:51:47 GMT  
		Size: 30.4 MB (30441333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:cd3be034605747b64cbb27bbdad719e4e6492ace1126b44c51159fbc59d93edc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25369467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7a99e726b896c91a21fe36c27f2d0a31fbbc34af4e6000c24de5174aa0ef2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:35ab2bf57814e9ff49e365efd5a5935b6915eede5c7f8581e9e1b85e0eecbe16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:a0a45bd8c6c4acd6967396366f01f2a68f73406327285edc5b7b07cb1cf073db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28572685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ce5a295b637a10bc329ded296a0c895e5e56e7c5e674188d423e213b0d213e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d23aa8e657602b0991be01bc98845f0039044e0274be15e0cff1ae330ab013b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24588743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b269006b5b030974e4afebc104e993a4a8078f883a8742194340e25578613b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b18dbe0837fd555c7028af6a1281ffa4fd1b5ffd835968f1009fd4cf9dfeaec3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27191817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe84df0b988965129e5189bae37e09e29d17d090cf4b8c8cb8dabf2443fd77`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:189ed3d4e1b2d68cb23cddd5b25351c45e0cf734f96cfe6faeb7502e5339b617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33295624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07521e3249989394fa16ab464aea52644c9686ee256068007f78dc53f58f8c18`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:e75cfa7ef5d58be253efa7d0fd4e027453d426734953dd39dd0d195705180855
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24243281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e34a031af45e3713cdd05b74ace973a4aac1e8161589c78dd5dbf24bda66cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:09:50 GMT
ADD file:3f3a2d77633db008f6d929f63880dab6bd20eab1e346e715331cc1b32a9d9821 in / 
# Fri, 02 Sep 2022 00:09:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6cbb7395a087ad86b87360ff9e4682ac013d19b01b368e0d658aa360440c9e0f`  
		Last Modified: Fri, 02 Sep 2022 00:26:57 GMT  
		Size: 24.2 MB (24243281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:79b29fd5d282f6fa2b03eb47235ab8aaaf1c360d7ebcfb82ba3af8a6eb52eebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27045282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0c81032f4bacdd27b86eaa7fbd7160e468523d1a14f722e771110b7e0a92d8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:20fa2d7bb4de7723f542be5923b06c4d704370f0390e4ae9e1c833c8785644c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:22.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d7ecc9c5e08953d586a6e50c29b91479a48f69ac1ba1f9dc0420d18a728dfc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc39ba059dcd42ade30aae30147b5692777ba9ff0779a62ad93a74de02e3e1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:7723f8c211cbc089f836e13136b35157ba572b61e0419d8f978917fca049db68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27016783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e636293a78dc5278638b41676f558e19826b82202e8c835021ea682114a4fe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1bc0bc3815bdcfafefa6b3ef1d8fd159564693d0f8fbb37b8151074651a11ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28381340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21735dab04ba60a144c23c491690a46073e06c72fdcc100f61bc610124eaa8c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7ecd20a7c308c281d7695ba41f4cdaa9544cbe118e71765ad48414023fa444a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35721187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9575c96de2157c77e6075c218b127e4d62c51ccbcef51c19a83d78d32212de7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:9c374fef8ababbbb0ec1f3c452de291159e258abb01bea320207fd29ec850c94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27744005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d2f5c3cb5043d8d2c2212aea246ad87e6a4b7fa6d0d6f01b87effa57b8a22`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:be541d4b5a77aad6ee06262f67641213785c2be5aac180f86418455f711f9f06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28643161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0926f9e9010b141cbc4803062e83ebb5da0224914531d45d30ec1db8ff6769e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:3cc2e19d3538681fb614683187329b47520424b80d7b31c97cdeb2403d82cae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:22.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:d1bb7a6d5328489e086a2b058d02155c1579575cc28e88b9715fe177493dc8a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27428015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e34ae906cfa0e790806cd584d563cc08dc6cd94965b82e0ad4f23ef9fd7882`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:c426292092c18964b8af9c6472ec5399fb847e377d215d9627b9ac3bf2a58e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25845683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2117c8d89f9af56983ef82f0ab715da7b4e0e6647e1facd6be46734fbe94c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f1507a8f2db68b552d73480e960e13111de4cb3be1ea570c54b097e2e839d7dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26663798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e3fb76febb675272d397040a109f404bfa6705ec3a45be5376742a2c4ed402`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:dbcb9a96e9f5bc64fb5dcbb3b8eaeebb16546f6b6efa95a96be9c1b72e70f77b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32082633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67d6c0812597fb08ae04598e0986b8c6fced9d4153f4c578b777995b7b690ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; riscv64

```console
$ docker pull ubuntu@sha256:69315ad5551ce29ec8c45aba461b0556bf6fd0d67728afeb996977412e1c5b1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25594334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb93887d22c140df11194c127de073880f244880d2b150d1321190320be848d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:d18c53653ff6feb3052b86e861da92f8a946c2ab9b6e0760314491e77f0ce5d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25995506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b1ab28aaec6e3c3afd74dd63dc16b006c681cd8be2f4806a645e68abf7e2f7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:3aa2ccb021969aadb28381fee1b247422e845b176e241cd1540c4b6831e000bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:ee1b6a6b513d6db9a14cf6e6d37895a7c70008d313d08cdf66e07cf617a3b978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26710085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476c64862aa8439ac32236e4dc7b2f35cffa748dd99565fcddd667f4994542e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1a9c90d5d959416422d50c65cd2b24dc8b7d596fd649c4249e814af97e47670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22305684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970ccdd609a88639212f12744557025bdeed28e800b788ea1cd908c252669a4f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:11 GMT
ADD file:93826239c43c79f307094d84d6fc79733e950dc0c0a332320254a2328eb5fff9 in / 
# Fri, 02 Sep 2022 06:08:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7347571ddfc71927a9f2ae03da3d05d7d68457aa24b5e18b6c7545fb65f4d034`  
		Last Modified: Fri, 02 Sep 2022 06:09:59 GMT  
		Size: 22.3 MB (22305684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:661c9525f2db5469c6fcb9e546442e62a1c7283ca0be7b0baa264c2f4b08dd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23734081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:487e1fdc39b6c9bf754e585f705e8e35c7fd30b88344a789010cfeb7919e68fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:919f05157e3a494086924aa02abe04f5fc08e84b41274c6a5549a996ac6ad530
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdc7dbece30f75bd7c19a0d9ec57c1b7724391304ad2db6a6e993a4c2160a3a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0fc175b31379070ddcfffdb1bfdc1f85d1f334ca9b784ab7baf94dcbf6457649
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30441333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6d9a8764c5e4bf91381594004243e6e44647dfc5c283cc002addb85ca8755`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:38 GMT
ADD file:57b462f3139cb98a97a7020f0d1be33f5beb6500115500a9bfd7aaec39854e35 in / 
# Thu, 01 Sep 2022 23:49:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c48fbbfad89e07e20864186f593c37c87089700f93ddb1b88e1912f891bf3ae2`  
		Last Modified: Thu, 01 Sep 2022 23:51:47 GMT  
		Size: 30.4 MB (30441333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:cd3be034605747b64cbb27bbdad719e4e6492ace1126b44c51159fbc59d93edc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25369467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7a99e726b896c91a21fe36c27f2d0a31fbbc34af4e6000c24de5174aa0ef2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20220829`

```console
$ docker pull ubuntu@sha256:3aa2ccb021969aadb28381fee1b247422e845b176e241cd1540c4b6831e000bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic-20220829` - linux; amd64

```console
$ docker pull ubuntu@sha256:ee1b6a6b513d6db9a14cf6e6d37895a7c70008d313d08cdf66e07cf617a3b978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26710085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476c64862aa8439ac32236e4dc7b2f35cffa748dd99565fcddd667f4994542e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220829` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1a9c90d5d959416422d50c65cd2b24dc8b7d596fd649c4249e814af97e47670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22305684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970ccdd609a88639212f12744557025bdeed28e800b788ea1cd908c252669a4f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:11 GMT
ADD file:93826239c43c79f307094d84d6fc79733e950dc0c0a332320254a2328eb5fff9 in / 
# Fri, 02 Sep 2022 06:08:12 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7347571ddfc71927a9f2ae03da3d05d7d68457aa24b5e18b6c7545fb65f4d034`  
		Last Modified: Fri, 02 Sep 2022 06:09:59 GMT  
		Size: 22.3 MB (22305684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220829` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:661c9525f2db5469c6fcb9e546442e62a1c7283ca0be7b0baa264c2f4b08dd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23734081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:487e1fdc39b6c9bf754e585f705e8e35c7fd30b88344a789010cfeb7919e68fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:32 GMT
ADD file:7a0b62af1ae0ff529abfef9c94385824381baa3a79aaf52940bce9508f9fc3c3 in / 
# Fri, 02 Sep 2022 00:57:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:dfd1fb90fd33185f74ada410bb05d51c40a41dff4883165698330ddc208f0b2d`  
		Last Modified: Fri, 02 Sep 2022 00:59:06 GMT  
		Size: 23.7 MB (23734081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220829` - linux; 386

```console
$ docker pull ubuntu@sha256:919f05157e3a494086924aa02abe04f5fc08e84b41274c6a5549a996ac6ad530
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdc7dbece30f75bd7c19a0d9ec57c1b7724391304ad2db6a6e993a4c2160a3a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220829` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0fc175b31379070ddcfffdb1bfdc1f85d1f334ca9b784ab7baf94dcbf6457649
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30441333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d6d9a8764c5e4bf91381594004243e6e44647dfc5c283cc002addb85ca8755`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:38 GMT
ADD file:57b462f3139cb98a97a7020f0d1be33f5beb6500115500a9bfd7aaec39854e35 in / 
# Thu, 01 Sep 2022 23:49:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c48fbbfad89e07e20864186f593c37c87089700f93ddb1b88e1912f891bf3ae2`  
		Last Modified: Thu, 01 Sep 2022 23:51:47 GMT  
		Size: 30.4 MB (30441333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220829` - linux; s390x

```console
$ docker pull ubuntu@sha256:cd3be034605747b64cbb27bbdad719e4e6492ace1126b44c51159fbc59d93edc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25369467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7a99e726b896c91a21fe36c27f2d0a31fbbc34af4e6000c24de5174aa0ef2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:3cc2e19d3538681fb614683187329b47520424b80d7b31c97cdeb2403d82cae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:d1bb7a6d5328489e086a2b058d02155c1579575cc28e88b9715fe177493dc8a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27428015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e34ae906cfa0e790806cd584d563cc08dc6cd94965b82e0ad4f23ef9fd7882`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:c426292092c18964b8af9c6472ec5399fb847e377d215d9627b9ac3bf2a58e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25845683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2117c8d89f9af56983ef82f0ab715da7b4e0e6647e1facd6be46734fbe94c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f1507a8f2db68b552d73480e960e13111de4cb3be1ea570c54b097e2e839d7dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26663798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e3fb76febb675272d397040a109f404bfa6705ec3a45be5376742a2c4ed402`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:dbcb9a96e9f5bc64fb5dcbb3b8eaeebb16546f6b6efa95a96be9c1b72e70f77b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32082633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67d6c0812597fb08ae04598e0986b8c6fced9d4153f4c578b777995b7b690ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; riscv64

```console
$ docker pull ubuntu@sha256:69315ad5551ce29ec8c45aba461b0556bf6fd0d67728afeb996977412e1c5b1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25594334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb93887d22c140df11194c127de073880f244880d2b150d1321190320be848d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:d18c53653ff6feb3052b86e861da92f8a946c2ab9b6e0760314491e77f0ce5d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25995506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b1ab28aaec6e3c3afd74dd63dc16b006c681cd8be2f4806a645e68abf7e2f7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:35ab2bf57814e9ff49e365efd5a5935b6915eede5c7f8581e9e1b85e0eecbe16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:a0a45bd8c6c4acd6967396366f01f2a68f73406327285edc5b7b07cb1cf073db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28572685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ce5a295b637a10bc329ded296a0c895e5e56e7c5e674188d423e213b0d213e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d23aa8e657602b0991be01bc98845f0039044e0274be15e0cff1ae330ab013b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24588743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b269006b5b030974e4afebc104e993a4a8078f883a8742194340e25578613b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b18dbe0837fd555c7028af6a1281ffa4fd1b5ffd835968f1009fd4cf9dfeaec3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27191817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe84df0b988965129e5189bae37e09e29d17d090cf4b8c8cb8dabf2443fd77`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:189ed3d4e1b2d68cb23cddd5b25351c45e0cf734f96cfe6faeb7502e5339b617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33295624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07521e3249989394fa16ab464aea52644c9686ee256068007f78dc53f58f8c18`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; riscv64

```console
$ docker pull ubuntu@sha256:e75cfa7ef5d58be253efa7d0fd4e027453d426734953dd39dd0d195705180855
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24243281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e34a031af45e3713cdd05b74ace973a4aac1e8161589c78dd5dbf24bda66cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:09:50 GMT
ADD file:3f3a2d77633db008f6d929f63880dab6bd20eab1e346e715331cc1b32a9d9821 in / 
# Fri, 02 Sep 2022 00:09:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6cbb7395a087ad86b87360ff9e4682ac013d19b01b368e0d658aa360440c9e0f`  
		Last Modified: Fri, 02 Sep 2022 00:26:57 GMT  
		Size: 24.2 MB (24243281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:79b29fd5d282f6fa2b03eb47235ab8aaaf1c360d7ebcfb82ba3af8a6eb52eebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27045282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0c81032f4bacdd27b86eaa7fbd7160e468523d1a14f722e771110b7e0a92d8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20220826`

```console
$ docker pull ubuntu@sha256:35ab2bf57814e9ff49e365efd5a5935b6915eede5c7f8581e9e1b85e0eecbe16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:focal-20220826` - linux; amd64

```console
$ docker pull ubuntu@sha256:a0a45bd8c6c4acd6967396366f01f2a68f73406327285edc5b7b07cb1cf073db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28572685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ce5a295b637a10bc329ded296a0c895e5e56e7c5e674188d423e213b0d213e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220826` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d23aa8e657602b0991be01bc98845f0039044e0274be15e0cff1ae330ab013b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24588743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b269006b5b030974e4afebc104e993a4a8078f883a8742194340e25578613b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:22 GMT
ADD file:685f4b5f8c1f11b6389e9f929909e1a667abf29814a7ccfb859aae287dacd7e1 in / 
# Fri, 02 Sep 2022 06:08:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:eff72fca8e1d166ddfda6ac6c409e888c95950da6c47d360a088219c0ad7ba05`  
		Last Modified: Fri, 02 Sep 2022 06:10:16 GMT  
		Size: 24.6 MB (24588743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220826` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b18dbe0837fd555c7028af6a1281ffa4fd1b5ffd835968f1009fd4cf9dfeaec3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27191817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe84df0b988965129e5189bae37e09e29d17d090cf4b8c8cb8dabf2443fd77`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220826` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:189ed3d4e1b2d68cb23cddd5b25351c45e0cf734f96cfe6faeb7502e5339b617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33295624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07521e3249989394fa16ab464aea52644c9686ee256068007f78dc53f58f8c18`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220826` - linux; riscv64

```console
$ docker pull ubuntu@sha256:e75cfa7ef5d58be253efa7d0fd4e027453d426734953dd39dd0d195705180855
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24243281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e34a031af45e3713cdd05b74ace973a4aac1e8161589c78dd5dbf24bda66cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:09:50 GMT
ADD file:3f3a2d77633db008f6d929f63880dab6bd20eab1e346e715331cc1b32a9d9821 in / 
# Fri, 02 Sep 2022 00:09:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6cbb7395a087ad86b87360ff9e4682ac013d19b01b368e0d658aa360440c9e0f`  
		Last Modified: Fri, 02 Sep 2022 00:26:57 GMT  
		Size: 24.2 MB (24243281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220826` - linux; s390x

```console
$ docker pull ubuntu@sha256:79b29fd5d282f6fa2b03eb47235ab8aaaf1c360d7ebcfb82ba3af8a6eb52eebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27045282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0c81032f4bacdd27b86eaa7fbd7160e468523d1a14f722e771110b7e0a92d8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:20fa2d7bb4de7723f542be5923b06c4d704370f0390e4ae9e1c833c8785644c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:jammy` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d7ecc9c5e08953d586a6e50c29b91479a48f69ac1ba1f9dc0420d18a728dfc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc39ba059dcd42ade30aae30147b5692777ba9ff0779a62ad93a74de02e3e1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:7723f8c211cbc089f836e13136b35157ba572b61e0419d8f978917fca049db68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27016783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e636293a78dc5278638b41676f558e19826b82202e8c835021ea682114a4fe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1bc0bc3815bdcfafefa6b3ef1d8fd159564693d0f8fbb37b8151074651a11ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28381340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21735dab04ba60a144c23c491690a46073e06c72fdcc100f61bc610124eaa8c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7ecd20a7c308c281d7695ba41f4cdaa9544cbe118e71765ad48414023fa444a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35721187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9575c96de2157c77e6075c218b127e4d62c51ccbcef51c19a83d78d32212de7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; riscv64

```console
$ docker pull ubuntu@sha256:9c374fef8ababbbb0ec1f3c452de291159e258abb01bea320207fd29ec850c94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27744005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d2f5c3cb5043d8d2c2212aea246ad87e6a4b7fa6d0d6f01b87effa57b8a22`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:be541d4b5a77aad6ee06262f67641213785c2be5aac180f86418455f711f9f06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28643161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0926f9e9010b141cbc4803062e83ebb5da0224914531d45d30ec1db8ff6769e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy-20220815`

```console
$ docker pull ubuntu@sha256:20fa2d7bb4de7723f542be5923b06c4d704370f0390e4ae9e1c833c8785644c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:jammy-20220815` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d7ecc9c5e08953d586a6e50c29b91479a48f69ac1ba1f9dc0420d18a728dfc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc39ba059dcd42ade30aae30147b5692777ba9ff0779a62ad93a74de02e3e1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220815` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:7723f8c211cbc089f836e13136b35157ba572b61e0419d8f978917fca049db68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27016783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e636293a78dc5278638b41676f558e19826b82202e8c835021ea682114a4fe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220815` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1bc0bc3815bdcfafefa6b3ef1d8fd159564693d0f8fbb37b8151074651a11ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28381340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21735dab04ba60a144c23c491690a46073e06c72fdcc100f61bc610124eaa8c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220815` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7ecd20a7c308c281d7695ba41f4cdaa9544cbe118e71765ad48414023fa444a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35721187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9575c96de2157c77e6075c218b127e4d62c51ccbcef51c19a83d78d32212de7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220815` - linux; riscv64

```console
$ docker pull ubuntu@sha256:9c374fef8ababbbb0ec1f3c452de291159e258abb01bea320207fd29ec850c94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27744005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d2f5c3cb5043d8d2c2212aea246ad87e6a4b7fa6d0d6f01b87effa57b8a22`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220815` - linux; s390x

```console
$ docker pull ubuntu@sha256:be541d4b5a77aad6ee06262f67641213785c2be5aac180f86418455f711f9f06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28643161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0926f9e9010b141cbc4803062e83ebb5da0224914531d45d30ec1db8ff6769e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:3cc2e19d3538681fb614683187329b47520424b80d7b31c97cdeb2403d82cae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:kinetic` - linux; amd64

```console
$ docker pull ubuntu@sha256:d1bb7a6d5328489e086a2b058d02155c1579575cc28e88b9715fe177493dc8a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27428015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e34ae906cfa0e790806cd584d563cc08dc6cd94965b82e0ad4f23ef9fd7882`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:c426292092c18964b8af9c6472ec5399fb847e377d215d9627b9ac3bf2a58e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25845683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2117c8d89f9af56983ef82f0ab715da7b4e0e6647e1facd6be46734fbe94c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f1507a8f2db68b552d73480e960e13111de4cb3be1ea570c54b097e2e839d7dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26663798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e3fb76febb675272d397040a109f404bfa6705ec3a45be5376742a2c4ed402`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:dbcb9a96e9f5bc64fb5dcbb3b8eaeebb16546f6b6efa95a96be9c1b72e70f77b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32082633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67d6c0812597fb08ae04598e0986b8c6fced9d4153f4c578b777995b7b690ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; riscv64

```console
$ docker pull ubuntu@sha256:69315ad5551ce29ec8c45aba461b0556bf6fd0d67728afeb996977412e1c5b1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25594334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb93887d22c140df11194c127de073880f244880d2b150d1321190320be848d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:d18c53653ff6feb3052b86e861da92f8a946c2ab9b6e0760314491e77f0ce5d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25995506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b1ab28aaec6e3c3afd74dd63dc16b006c681cd8be2f4806a645e68abf7e2f7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic-20220830`

```console
$ docker pull ubuntu@sha256:3cc2e19d3538681fb614683187329b47520424b80d7b31c97cdeb2403d82cae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:kinetic-20220830` - linux; amd64

```console
$ docker pull ubuntu@sha256:d1bb7a6d5328489e086a2b058d02155c1579575cc28e88b9715fe177493dc8a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27428015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e34ae906cfa0e790806cd584d563cc08dc6cd94965b82e0ad4f23ef9fd7882`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:43 GMT
ADD file:d5de90ac61ee7027aa0900efb669efa73f611463cf73ab2cfdacadf5ab9fee19 in / 
# Thu, 01 Sep 2022 23:46:43 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0b78030514e08aad79cb596ba84b18b9579e90eac0b8e0c2dec483c3da8dbee8`  
		Last Modified: Thu, 01 Sep 2022 23:48:15 GMT  
		Size: 27.4 MB (27428015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220830` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:c426292092c18964b8af9c6472ec5399fb847e377d215d9627b9ac3bf2a58e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25845683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2117c8d89f9af56983ef82f0ab715da7b4e0e6647e1facd6be46734fbe94c14`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:44 GMT
ADD file:6fea481ddc80754c10680e7c291055af82ef815eb0fdaf745c49c4f4cdf2afa1 in / 
# Fri, 02 Sep 2022 06:08:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1f63be4c3b8fca43746377bd8a99dd9b04acdd942d8464feaae1671e6363d920`  
		Last Modified: Fri, 02 Sep 2022 06:10:58 GMT  
		Size: 25.8 MB (25845683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220830` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f1507a8f2db68b552d73480e960e13111de4cb3be1ea570c54b097e2e839d7dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26663798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e3fb76febb675272d397040a109f404bfa6705ec3a45be5376742a2c4ed402`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:58:02 GMT
ADD file:1b9e898b22915c14e3d83959e989e2a653148ff82c8e2a1b3dfa8035256219aa in / 
# Fri, 02 Sep 2022 00:58:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7c0b344a74c2d365a9a57a618f4a544c4e8e70f341f67973d3a22aee52a267b9`  
		Last Modified: Fri, 02 Sep 2022 01:00:04 GMT  
		Size: 26.7 MB (26663798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220830` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:dbcb9a96e9f5bc64fb5dcbb3b8eaeebb16546f6b6efa95a96be9c1b72e70f77b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32082633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67d6c0812597fb08ae04598e0986b8c6fced9d4153f4c578b777995b7b690ce`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220830` - linux; riscv64

```console
$ docker pull ubuntu@sha256:69315ad5551ce29ec8c45aba461b0556bf6fd0d67728afeb996977412e1c5b1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25594334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb93887d22c140df11194c127de073880f244880d2b150d1321190320be848d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220830` - linux; s390x

```console
$ docker pull ubuntu@sha256:d18c53653ff6feb3052b86e861da92f8a946c2ab9b6e0760314491e77f0ce5d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25995506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b1ab28aaec6e3c3afd74dd63dc16b006c681cd8be2f4806a645e68abf7e2f7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:38 GMT
ADD file:61a0b983796cf76453cbc73a44968b8cefb9f90cc922075728432bdbdaaeb854 in / 
# Fri, 02 Sep 2022 01:03:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a51274124ed15147344e4d31d9378a33521faff1de175e551081c34c14db1b9f`  
		Last Modified: Fri, 02 Sep 2022 01:05:17 GMT  
		Size: 26.0 MB (25995506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:20fa2d7bb4de7723f542be5923b06c4d704370f0390e4ae9e1c833c8785644c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d7ecc9c5e08953d586a6e50c29b91479a48f69ac1ba1f9dc0420d18a728dfc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc39ba059dcd42ade30aae30147b5692777ba9ff0779a62ad93a74de02e3e1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:7723f8c211cbc089f836e13136b35157ba572b61e0419d8f978917fca049db68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27016783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e636293a78dc5278638b41676f558e19826b82202e8c835021ea682114a4fe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1bc0bc3815bdcfafefa6b3ef1d8fd159564693d0f8fbb37b8151074651a11ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28381340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21735dab04ba60a144c23c491690a46073e06c72fdcc100f61bc610124eaa8c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7ecd20a7c308c281d7695ba41f4cdaa9544cbe118e71765ad48414023fa444a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35721187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9575c96de2157c77e6075c218b127e4d62c51ccbcef51c19a83d78d32212de7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; riscv64

```console
$ docker pull ubuntu@sha256:9c374fef8ababbbb0ec1f3c452de291159e258abb01bea320207fd29ec850c94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27744005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d2f5c3cb5043d8d2c2212aea246ad87e6a4b7fa6d0d6f01b87effa57b8a22`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:be541d4b5a77aad6ee06262f67641213785c2be5aac180f86418455f711f9f06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28643161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0926f9e9010b141cbc4803062e83ebb5da0224914531d45d30ec1db8ff6769e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:20fa2d7bb4de7723f542be5923b06c4d704370f0390e4ae9e1c833c8785644c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:2d7ecc9c5e08953d586a6e50c29b91479a48f69ac1ba1f9dc0420d18a728dfc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc39ba059dcd42ade30aae30147b5692777ba9ff0779a62ad93a74de02e3e1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:7723f8c211cbc089f836e13136b35157ba572b61e0419d8f978917fca049db68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27016783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e636293a78dc5278638b41676f558e19826b82202e8c835021ea682114a4fe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1bc0bc3815bdcfafefa6b3ef1d8fd159564693d0f8fbb37b8151074651a11ffb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28381340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21735dab04ba60a144c23c491690a46073e06c72fdcc100f61bc610124eaa8c9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7ecd20a7c308c281d7695ba41f4cdaa9544cbe118e71765ad48414023fa444a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35721187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9575c96de2157c77e6075c218b127e4d62c51ccbcef51c19a83d78d32212de7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; riscv64

```console
$ docker pull ubuntu@sha256:9c374fef8ababbbb0ec1f3c452de291159e258abb01bea320207fd29ec850c94
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27744005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d2f5c3cb5043d8d2c2212aea246ad87e6a4b7fa6d0d6f01b87effa57b8a22`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:be541d4b5a77aad6ee06262f67641213785c2be5aac180f86418455f711f9f06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28643161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0926f9e9010b141cbc4803062e83ebb5da0224914531d45d30ec1db8ff6769e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty`

```console
$ docker pull ubuntu@sha256:d7a459ecd77ebb09525584f2c3e1bb7f6a2879d90df8a3523c1b899dfc2a226f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d34202d0ce9f1a55b9fffa1d69af2821dcf9645cc655e96a5b168c2a9265d5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a7f3400ca032052bf769658a0a6f7562e441504c7da16527defa818a24fcf0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:30 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 02 Aug 2022 01:41:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:41:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430e3e7a1afcac7bf89d27c42804489d76ac8775a945924494e9e5794f0ce6`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 76.8 KB (76779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8c3e99facaf81b42b2e4e24792e7254297607e2273054e5f729712163cafc2`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:209f78eaf05254c51cff7676b913bcb70c1da54e58ae728a592ea58f3b5552b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd23a098588cb567106c63829bf08759e87f4235bbd4c90168e6b065420ac853`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:42 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 02 Aug 2022 01:31:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:31:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:31:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:31:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736dbcbc0bcb73948970c71c59c6fc5662698a0cdca10a232da87ede89aabeef`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 63.4 KB (63436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376b7bbeb4d42e6e9b75e9ad5bd043790235c8963cac05a03bc5400002ae965b`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty-20191217`

```console
$ docker pull ubuntu@sha256:d7a459ecd77ebb09525584f2c3e1bb7f6a2879d90df8a3523c1b899dfc2a226f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty-20191217` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d34202d0ce9f1a55b9fffa1d69af2821dcf9645cc655e96a5b168c2a9265d5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a7f3400ca032052bf769658a0a6f7562e441504c7da16527defa818a24fcf0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:30 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 02 Aug 2022 01:41:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:41:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a430e3e7a1afcac7bf89d27c42804489d76ac8775a945924494e9e5794f0ce6`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 76.8 KB (76779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8c3e99facaf81b42b2e4e24792e7254297607e2273054e5f729712163cafc2`  
		Last Modified: Tue, 02 Aug 2022 01:44:15 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:209f78eaf05254c51cff7676b913bcb70c1da54e58ae728a592ea58f3b5552b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd23a098588cb567106c63829bf08759e87f4235bbd4c90168e6b065420ac853`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:42 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 02 Aug 2022 01:31:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:31:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 02 Aug 2022 01:31:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:31:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736dbcbc0bcb73948970c71c59c6fc5662698a0cdca10a232da87ede89aabeef`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 63.4 KB (63436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376b7bbeb4d42e6e9b75e9ad5bd043790235c8963cac05a03bc5400002ae965b`  
		Last Modified: Tue, 02 Aug 2022 01:35:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial`

```console
$ docker pull ubuntu@sha256:91bd29a464fdabfcf44e29e1f2a5f213c6dfa750b6290e40dd6998ac79da3c41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
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

### `ubuntu:xenial` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:696252dd941a9a0ca7db7ca8d9fbb91d838cc9bfb27403219953af6750a89111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20832692ca6e913217051aa57084ec76c076987a63cd497100d754b27097fa33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
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

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:4ef33ed6b1af10706727d280de436bced5e9413cba7992d6126c866efd79cacd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fb9d3bc97649795df6522739036df75814819b4b48997a6e05345dcd5e6845`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
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

## `ubuntu:xenial-20210804`

```console
$ docker pull ubuntu@sha256:91bd29a464fdabfcf44e29e1f2a5f213c6dfa750b6290e40dd6998ac79da3c41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial-20210804` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
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

### `ubuntu:xenial-20210804` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:696252dd941a9a0ca7db7ca8d9fbb91d838cc9bfb27403219953af6750a89111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20832692ca6e913217051aa57084ec76c076987a63cd497100d754b27097fa33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:46 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 02 Aug 2022 01:41:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:41:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:41:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:41:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c9df55506368eeeb59c5f56bf5d6f9ef4476a6b1e43154eebe32e436e60d7a`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60aa30d82c4849b80da22554e0006d9c23c68a807fcb795b2f35ac6c02549eca`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61b5d5a768deb5e021d74947bacf44422a006a3495d70395a7d745e07fab3f3`  
		Last Modified: Tue, 02 Aug 2022 01:44:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
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

### `ubuntu:xenial-20210804` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:4ef33ed6b1af10706727d280de436bced5e9413cba7992d6126c866efd79cacd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fb9d3bc97649795df6522739036df75814819b4b48997a6e05345dcd5e6845`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:32:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 02 Aug 2022 01:32:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 02 Aug 2022 01:32:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:32:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 02 Aug 2022 01:32:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bced789eccb5759f541a5b15b9a3031c06cc54bdbff1a553cc0ef29ddad2bc`  
		Last Modified: Tue, 02 Aug 2022 01:36:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a61259761ffe18601a628413443ccb5dee06a185a81c902220dfc070801c3`  
		Last Modified: Tue, 02 Aug 2022 01:35:56 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272460dff18ff8fd96d33337b0ff5cc5d9d2e7f158c662273e1bb760c7f9722`  
		Last Modified: Tue, 02 Aug 2022 01:36:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
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
