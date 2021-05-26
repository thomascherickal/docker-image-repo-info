<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:14.04`](#ubuntu1404)
-	[`ubuntu:16.04`](#ubuntu1604)
-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:20.10`](#ubuntu2010)
-	[`ubuntu:21.04`](#ubuntu2104)
-	[`ubuntu:21.10`](#ubuntu2110)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20210512`](#ubuntubionic-20210512)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20210416`](#ubuntufocal-20210416)
-	[`ubuntu:groovy`](#ubuntugroovy)
-	[`ubuntu:groovy-20210524`](#ubuntugroovy-20210524)
-	[`ubuntu:hirsute`](#ubuntuhirsute)
-	[`ubuntu:hirsute-20210522`](#ubuntuhirsute-20210522)
-	[`ubuntu:impish`](#ubuntuimpish)
-	[`ubuntu:impish-20210519`](#ubuntuimpish-20210519)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:rolling`](#ubunturolling)
-	[`ubuntu:trusty`](#ubuntutrusty)
-	[`ubuntu:trusty-20191217`](#ubuntutrusty-20191217)
-	[`ubuntu:xenial`](#ubuntuxenial)
-	[`ubuntu:xenial-20210429`](#ubuntuxenial-20210429)

## `ubuntu:14.04`

```console
$ docker pull ubuntu@sha256:4a8a6fa8810a3e01352981b35165b0b28403fe2a4e2535e315b23b4a69cd130a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull ubuntu@sha256:3c395cb9747f1d1513c3fa8a53b19c425e4fc43917c9c9204b69bf9001bf3c48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9ccf3968dbe6dfa7c2ee2f4b9fa9873977ea42634d6af78d255f76568f440d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Wed, 16 Sep 2020 22:29:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:29:45 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:29:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:29:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f0252367c5101cf7b90111c68054763b033350a90f2a18cc130ba9105769`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 76.8 KB (76772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4df6dcc20e58a34495cbea3866f25407b84dc9b253bf94d90de4d1fb20a8c5`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e0c3b6ef57e7710699c96f5b628199cc79f52feaddc96a8349ec2fa8ac1f9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e151b73d5f6446106434be4373ec707411667f1a313d00b983377c8f146de2fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Wed, 16 Sep 2020 23:17:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331949be49492d155af0307a821055a15f39e00916fd82acc0bc1aef242ed7e4`  
		Last Modified: Wed, 16 Sep 2020 23:19:11 GMT  
		Size: 59.1 KB (59097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9870c957ca40dbafea6c69c3cf4c8258e4114da0caa202e59f2268991aae7cd3`  
		Last Modified: Wed, 16 Sep 2020 23:19:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a664cf8519ac301fb0ef545c3b3e53dfdffcf9a0235ddaa51eca299948cc568f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3482d381e047de7cfaed92b88a16e086f36bb5c76d75b266bf2f14490b673e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Wed, 16 Sep 2020 23:58:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:58:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:58:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:58:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1599d04814b0dacc320abd16ec9e1d0d3d344ca7656ed5504d1c529489feb6ca`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef37a9325c7a10b2959384fb20a3c89ddc6c3374693c7d50248ed1eae25653`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:16.04`

```console
$ docker pull ubuntu@sha256:98afb2808ee1ec6aa4d7c8f8b82c6347b9ae156932f7186182b997f3d5616ebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:16.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:d7bb0589725587f2f67d0340edb81fd1fcba6c5f38166639cf2a252c939aa30c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff95a467e458bb9e8653b1df439e02e07fc0be5b362cc3d9aeb0d04039d5925`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5eb7810e4e9f5a336b6ab2fdecb4b467ad1ceae5a352d3fed5680d9c43170771
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b1e9393d1b4c129d2146619ad07abe90537f2e395ce7394c4c42404821d90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:23:21 GMT
ADD file:7e5c1f0262200ed290a61913d7f2c3b2b064c9b02aa1a55a818e38ab1316bbda in / 
# Wed, 19 May 2021 20:23:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:23:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 20:23:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:23:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ae1370da0037e05eb3f24cd486c49ee3a450840763c7d31deef8274cb9abfd86`  
		Last Modified: Wed, 19 May 2021 20:24:51 GMT  
		Size: 40.3 MB (40292258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452bc1820a9d9923cac2a73df110a9ad72318825a2ff4807ed5e89708052cea5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1217aa77f4015a99b17bec638b9f07cdf319ff342015b6c42800a588797d54a7`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84e209d76ee2a0ef7c673bb433398f6e5765eed483d8f68f8015126a1d3ce5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e8eb681cb9e01f339e1d68a47bf6d08a876f875ecf68f263891770bdc3400485
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41028247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f93e87bc68fc5d68ec7c669587d37ea34dc8143de2d4f43386d90a1b6ebab78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; 386

```console
$ docker pull ubuntu@sha256:c33ba65d993289a57df23ed7bcf5a63ea337c56371102aff819c2434e04a59ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45786471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e39c4a62166c3ae7764aaa06b78b1340dfd6e9839813aa82229352f36960c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:41:16 GMT
ADD file:082ca60ab0fd6043fa0b84148070e08bd36e575f3d8970eed54fe4c23aecf44a in / 
# Wed, 19 May 2021 19:41:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:41:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:41:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:41:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b0e5cfe962be5da09713a785360c5afe671f77a12ab690cfff78d4dc4f7bb372`  
		Last Modified: Wed, 19 May 2021 19:42:19 GMT  
		Size: 45.8 MB (45784935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706307f7bb6b836ba10c2f2df595c44e8de7262991f317c23ef61a99660e00a9`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49163eca4e92d67eeb1efa9eeb705eef784becadff03a085232ec7d7061adb37`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d37544d5536a00ff5bc2e023bd9b65a71266f4dd32a8b9ac616adeaef86833`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f42387920067dfe092a27337e281548d68888e93b7ea710e452f012a859caed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47494580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426a54dd9a773d28f88ecc1445838d67e4e4c4143b2ee37e399eb8216a191cc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:32:17 GMT
ADD file:639591e81174c559325b9d1d20efd2f26714b2b054be088252ac55afb93858ed in / 
# Wed, 19 May 2021 21:32:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:32:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:33:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6bb4d8d9255ba68d96734382b8a7bd6608fff0a888c7c6b0aa52d9eb7fc8f11`  
		Last Modified: Wed, 19 May 2021 21:35:17 GMT  
		Size: 47.5 MB (47493078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8718cfe093a36e16721650cedbb150a6e4dd982dd642e6af508af7f2a9baa8`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425fa8f42a78e60d1c406959f5f6629a972fc542248c750f3b05d925a957c2e7`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973b2a3c74625a11480006478adbc31fb4b9522720386b3f19aa8c732a8f8cb`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:85f0e3c6e17efd884f4925859d3b771819e2d4618f92feabb047e5e3a77ec1d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44062586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a5278b1b1fc11837808e9bf7e7e3831a53c47ac3b2c61f82bbc1dfb5065bc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:29:52 GMT
ADD file:d6162b58b24c8842e7bc7d3f9c318c9c914ea2f8d18de8081ee87ffda0c9bc23 in / 
# Wed, 19 May 2021 23:30:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:30:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 23:30:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:30:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5483b215c78221b499b39a57c60379b545a5ab9f9c2c206f8509236f72d6ec90`  
		Last Modified: Wed, 19 May 2021 23:31:17 GMT  
		Size: 44.1 MB (44061095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb39f9943e9829ed5fd8deaeddfad18f6f37dad3399c89d93b6a7fa7c2232f3`  
		Last Modified: Wed, 19 May 2021 23:31:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f68e1710512337a2a8cbf88f1e50225470073f9f58616d4241ea2b65b4616`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab0373bf4c06812031cf4deaf1959122cfd5fef7462f8e59e41dd4974563a8`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:04919776d30640ce4ed24442d5f7c1a8e4bd0e4793ed9469843cedaecb0d72fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:ceed028aae0eac7db9dd33bd89c14d5a9991d73443b0de24ba0db250f47491d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81bcf752ac3dc8a12d54908ecdfe98a857c84285e5d50bed1d10f9812377abd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b399f5db27b50ba1db41a19f97b2ce73b470d90fc70e18bf3b96fd863c9dc9c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22293049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff8caddb242004ff1f5c45a30db06f13e3040f4aad2c3c8964d3e5774b36a49`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:21:52 GMT
ADD file:c990710d70105be91eebcea7dfdf28e2212d37ea9279eb2dfd0071e9ed2fd4f1 in / 
# Wed, 19 May 2021 20:21:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:21:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c61ae1d5a3957b8a0838e053004a2ddf56e395d58ee3b63baa7b1c865a6383b9`  
		Last Modified: Wed, 19 May 2021 20:23:59 GMT  
		Size: 22.3 MB (22292007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ceff6e604f05b8d76ca10ab8fd06e21e9edb719c243d7a204cd6fd6321a0aa`  
		Last Modified: Wed, 19 May 2021 20:23:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5399193bfffbb95297aa486ca4b2fa0207207d9a9e4c53f6bfbbcb85c76a678`  
		Last Modified: Wed, 19 May 2021 20:23:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:26d3b518d930e4e00dbd38f003792a0dddf6c1c7788c095b99c8b0845dcf107c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23704736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193e297a4ffd5e818585ef5f8b0c219f3c5b939a2eec41017489e771e45e71b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:860b09eebc2fb2a622f4b51e5ea2c35cc1596e4075d5cbe3aef7c84f86e66b9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a7cb63ac1b3cf8bd450757e5ed69a1a0d3b95b87e2d550a02ef7e191df6174`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:40:52 GMT
ADD file:e0284f44e9a104546ff12ccb0b485d12a45fef6c2035358fc5620e7a702b358e in / 
# Wed, 19 May 2021 19:40:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:40:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:40:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:40:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da97bc6b7e988f4f13b3e5091db2330133381a463cb607de469e04742900f5f4`  
		Last Modified: Wed, 19 May 2021 19:41:52 GMT  
		Size: 27.1 MB (27131287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652d638a400430b9b485097830ca789323f97806c727fdace35095c1314272a5`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449e958dde8dd03ed487ed6b0df2995490dab77191cdb761ceeda156fd24689`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:add50dcbe8d28e3d499ff6468fbbeb619e2accf42e3de6dd48561c30f7fd76d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30408205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5bc8205a89b4531107d3ff92acb6c883121ceb42f52e025f3213c0bb78033a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:c5598bdf2533dab480dd217d2469bfcc0b797c934f8a43fbfa6a2cd19d438648
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25353592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb59094ec08dd44dbf938102b747c7a64eda1b182e42be293ecdaa1099eeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:28:29 GMT
ADD file:718406af36d25bc30b425ddad4eaa810e4f8cfe92388955edc07fd5ec9816dcc in / 
# Wed, 19 May 2021 23:28:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:28:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 23:28:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d5e421eb08da6bcb06173fcdd4e739a0fc77d7b26f72680342d8db9aedebf05`  
		Last Modified: Wed, 19 May 2021 23:30:36 GMT  
		Size: 25.4 MB (25352550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b74c33ee4c205747bbbc098fc12afc14cab69dd5b2186b8bf7ee58f516631b`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb318177ecfab6a1f7a7c8290c83d4d680cf1110f5b4d80fd059793e3b64708`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:cf31af331f38d1d7158470e095b132acd126a7180a54f263d386da88eb681d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:86ac87f73641c920fb42cc9612d4fb57b5626b56ea2a19b894d0673fd5b4f2e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28540664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0aa2d69a153215c790488ed1fcec162015e973e49962d438e18249d16fa9bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a3e1155cd215efd134f7c70085a2674be897c9b6f7f421b8f19e46673ded3b87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24039589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd9976bcd84a12cfd82950c227f2b17e4033630e569ebc431a0c37409d3a072`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:44 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Fri, 23 Apr 2021 22:36:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3438cfd01915ec245a55dd1047748b26e29a31f4e630766126666c6bc9953a71`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc3cbbc3a3f69a5c07b934f21be14f7006510ff7a327d2f05f94ff680084d5`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1de4c5e2d8954bf5fa9855f8b4c9d3c3b97d1d380efe19f60f3e4107a66f5cae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a98cbe39225dadebcaa04e21dbe5900ad604739b07a9fa351dd10a6ebad4c1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:42d5c74d24685935e6167271ebb74c5898c5adf273dae80a82f9e39e8ae0dab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33256424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81ddd5d688c701fcfd0bf047bd4b9e3ee13f2801a76f37b4512761d369008a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:bdf7ff77dcb36ea18b53d7f2d340d8eea7bbb70e4a2609e959fe1162fd3a46ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27137388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230e5e1e3def457ce7266d68691dc4fc52ab00d071b7401d66d876d95745b65d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.10`

```console
$ docker pull ubuntu@sha256:0971c3fba4ea1ba7012aff4c5ff2a02a1d9fe71f85bd6a2f6ff59939431c7484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:870bba7433f601825f13b95a70b7df32f3ca5bb7ef0a865e8efc0a79e03e0c6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69040ea16df09b627e155acc7762b65b4474f341a3b09fee9b9f7e003224b8ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:28:11 GMT
ADD file:5582a76cd73639bd7b5f941762801034fe6d3297d63d8333085c79c31b5e777a in / 
# Wed, 26 May 2021 00:28:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:28:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:28:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:28:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0dfa4d6d32846900cdf518b31b7420c8e3bee78df56f061347f079b085e55eed`  
		Last Modified: Wed, 26 May 2021 00:29:22 GMT  
		Size: 31.3 MB (31339605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325ba66a34e9b2cf96e7958749a4fdd29a90699b6cd7eb67976c266a8277a26b`  
		Last Modified: Wed, 26 May 2021 00:29:18 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6382425bb0d013b4122cc28ffc63f8bce680a6562260cb6fa715f6f16a59db`  
		Last Modified: Wed, 26 May 2021 00:29:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6c6739fc427893da3110e2f2c631f34e1146dc28f99b08ef8de367ba6c389159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.3 MB (26302837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80239021fb9fa8a4c61c6e01eddbd4be06026a0545fff726543d44f18fbda922`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:22:24 GMT
ADD file:acda6861dee730077731d36484af6c3fa51a7ea2bcdbab39a88f53cb3276509e in / 
# Wed, 19 May 2021 20:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:22:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec376efdd72c4146827ffa866153a4452541beae9106def5a3afb4e858023939`  
		Last Modified: Wed, 19 May 2021 20:24:15 GMT  
		Size: 26.3 MB (26301801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065457da20bed844ec32f63c2c352d39da0d9cf58fd9fcdd710a8c2fe01e0ec`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffea83b1b3aaf9f535176139002bf18809b84cc711fddf2a83206c09194c8c`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:15507ed695229e52b84dbf79ab052b9c738917442244376d136ab0d99478c1c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29859198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae42a2f69b62859661cbea2a3c44cf7523fb015a05e5d3501223c3f767baf585`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:48:13 GMT
ADD file:3b909e405de304d3529a43650aa6812b726dbfe24e2f2a9c163818ab5c206cf1 in / 
# Fri, 23 Apr 2021 22:48:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:48:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:48:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:48:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0312c280f333ebad21d92c6554a1f0b81a5d7de275f2f1fe29c960721e40cb28`  
		Last Modified: Fri, 23 Apr 2021 22:50:26 GMT  
		Size: 29.9 MB (29858157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fedfba085a0c1226682c17f7966295deb654a557860da25aedabd09c96edf6`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d5a4de4889c6c2db1938b8170a1a427483a6b6ab113ceeae3e4b02819d54cf`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:39f41dfb4f2896402a9bf9e2b18b023bc5c01105ef74533f7822965f47ceb54f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36546459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6bfb84c7c6913211df3cfd6124ac66d4b4217cd9f27c173afcbb6d7383d6da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:59 GMT
ADD file:417e85e230e48984b1cc0db245a092e51901fd8cf010070a82fd06ccaec211df in / 
# Wed, 26 May 2021 00:51:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:51:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:51:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:51:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f7501b08507a493babfe9a7a361950a90febd51f598365c8c72a27438e176910`  
		Last Modified: Wed, 26 May 2021 00:54:09 GMT  
		Size: 36.5 MB (36545421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b1bdfb29d855647202d2d86b6473a9b637d7edaafa7d199fe951071b946c0`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63192a9aec9ad98562f0c79212fe107a71c90d1b3f55488cb16ca414d1d6853f`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:b383d0b95879b99225bb648cf95a1869d18c272d021e447900a66c0ccbdcf1b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31564581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e08195772cd6a7e5593d472700d9fcd9744019b04ffe13cfece3135bfa4419e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:49 GMT
ADD file:953040401ce401194c7939af20d4b65872f29c9f1c9e9411f5b04fbd299161d6 in / 
# Wed, 26 May 2021 00:50:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:50:55 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:50:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:50:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a86f368f271868bec872a3e420550decf4fa2f153ca0ebcec9ab48b642f129b1`  
		Last Modified: Wed, 26 May 2021 00:52:15 GMT  
		Size: 31.6 MB (31563545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf527448b6952fd5c7da27d42ed151c11bafb569d579a96ce879307419f0970`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d46e2e6002b01a57ea745988830c3950a2aa33250abe3ebcd67891351feba1f`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:21.04`

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

### `ubuntu:21.04` - linux; amd64

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

### `ubuntu:21.04` - linux; arm variant v7

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

### `ubuntu:21.04` - linux; arm64 variant v8

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

### `ubuntu:21.04` - linux; ppc64le

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

### `ubuntu:21.04` - linux; s390x

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

## `ubuntu:21.10`

```console
$ docker pull ubuntu@sha256:d2ca9636434345840b6dae327fbe2d000d5289739987fa1410c76c2a9d774833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:21.10` - linux; amd64

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

### `ubuntu:21.10` - linux; ppc64le

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

### `ubuntu:21.10` - linux; s390x

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

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:04919776d30640ce4ed24442d5f7c1a8e4bd0e4793ed9469843cedaecb0d72fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:ceed028aae0eac7db9dd33bd89c14d5a9991d73443b0de24ba0db250f47491d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81bcf752ac3dc8a12d54908ecdfe98a857c84285e5d50bed1d10f9812377abd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b399f5db27b50ba1db41a19f97b2ce73b470d90fc70e18bf3b96fd863c9dc9c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22293049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff8caddb242004ff1f5c45a30db06f13e3040f4aad2c3c8964d3e5774b36a49`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:21:52 GMT
ADD file:c990710d70105be91eebcea7dfdf28e2212d37ea9279eb2dfd0071e9ed2fd4f1 in / 
# Wed, 19 May 2021 20:21:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:21:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c61ae1d5a3957b8a0838e053004a2ddf56e395d58ee3b63baa7b1c865a6383b9`  
		Last Modified: Wed, 19 May 2021 20:23:59 GMT  
		Size: 22.3 MB (22292007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ceff6e604f05b8d76ca10ab8fd06e21e9edb719c243d7a204cd6fd6321a0aa`  
		Last Modified: Wed, 19 May 2021 20:23:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5399193bfffbb95297aa486ca4b2fa0207207d9a9e4c53f6bfbbcb85c76a678`  
		Last Modified: Wed, 19 May 2021 20:23:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:26d3b518d930e4e00dbd38f003792a0dddf6c1c7788c095b99c8b0845dcf107c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23704736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193e297a4ffd5e818585ef5f8b0c219f3c5b939a2eec41017489e771e45e71b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:860b09eebc2fb2a622f4b51e5ea2c35cc1596e4075d5cbe3aef7c84f86e66b9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a7cb63ac1b3cf8bd450757e5ed69a1a0d3b95b87e2d550a02ef7e191df6174`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:40:52 GMT
ADD file:e0284f44e9a104546ff12ccb0b485d12a45fef6c2035358fc5620e7a702b358e in / 
# Wed, 19 May 2021 19:40:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:40:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:40:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:40:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da97bc6b7e988f4f13b3e5091db2330133381a463cb607de469e04742900f5f4`  
		Last Modified: Wed, 19 May 2021 19:41:52 GMT  
		Size: 27.1 MB (27131287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652d638a400430b9b485097830ca789323f97806c727fdace35095c1314272a5`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449e958dde8dd03ed487ed6b0df2995490dab77191cdb761ceeda156fd24689`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:add50dcbe8d28e3d499ff6468fbbeb619e2accf42e3de6dd48561c30f7fd76d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30408205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5bc8205a89b4531107d3ff92acb6c883121ceb42f52e025f3213c0bb78033a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:c5598bdf2533dab480dd217d2469bfcc0b797c934f8a43fbfa6a2cd19d438648
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25353592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb59094ec08dd44dbf938102b747c7a64eda1b182e42be293ecdaa1099eeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:28:29 GMT
ADD file:718406af36d25bc30b425ddad4eaa810e4f8cfe92388955edc07fd5ec9816dcc in / 
# Wed, 19 May 2021 23:28:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:28:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 23:28:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d5e421eb08da6bcb06173fcdd4e739a0fc77d7b26f72680342d8db9aedebf05`  
		Last Modified: Wed, 19 May 2021 23:30:36 GMT  
		Size: 25.4 MB (25352550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b74c33ee4c205747bbbc098fc12afc14cab69dd5b2186b8bf7ee58f516631b`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb318177ecfab6a1f7a7c8290c83d4d680cf1110f5b4d80fd059793e3b64708`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20210512`

```console
$ docker pull ubuntu@sha256:cf1df6bbe3c75502945a4f2d7709b55014e5372e7d2e1e1457b3dd89e626a508
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic-20210512` - linux; amd64

```console
$ docker pull ubuntu@sha256:ceed028aae0eac7db9dd33bd89c14d5a9991d73443b0de24ba0db250f47491d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26697350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81bcf752ac3dc8a12d54908ecdfe98a857c84285e5d50bed1d10f9812377abd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210512` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b399f5db27b50ba1db41a19f97b2ce73b470d90fc70e18bf3b96fd863c9dc9c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22293049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff8caddb242004ff1f5c45a30db06f13e3040f4aad2c3c8964d3e5774b36a49`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:21:52 GMT
ADD file:c990710d70105be91eebcea7dfdf28e2212d37ea9279eb2dfd0071e9ed2fd4f1 in / 
# Wed, 19 May 2021 20:21:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:21:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c61ae1d5a3957b8a0838e053004a2ddf56e395d58ee3b63baa7b1c865a6383b9`  
		Last Modified: Wed, 19 May 2021 20:23:59 GMT  
		Size: 22.3 MB (22292007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ceff6e604f05b8d76ca10ab8fd06e21e9edb719c243d7a204cd6fd6321a0aa`  
		Last Modified: Wed, 19 May 2021 20:23:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5399193bfffbb95297aa486ca4b2fa0207207d9a9e4c53f6bfbbcb85c76a678`  
		Last Modified: Wed, 19 May 2021 20:23:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210512` - linux; 386

```console
$ docker pull ubuntu@sha256:860b09eebc2fb2a622f4b51e5ea2c35cc1596e4075d5cbe3aef7c84f86e66b9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a7cb63ac1b3cf8bd450757e5ed69a1a0d3b95b87e2d550a02ef7e191df6174`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:40:52 GMT
ADD file:e0284f44e9a104546ff12ccb0b485d12a45fef6c2035358fc5620e7a702b358e in / 
# Wed, 19 May 2021 19:40:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:40:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:40:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:40:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da97bc6b7e988f4f13b3e5091db2330133381a463cb607de469e04742900f5f4`  
		Last Modified: Wed, 19 May 2021 19:41:52 GMT  
		Size: 27.1 MB (27131287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652d638a400430b9b485097830ca789323f97806c727fdace35095c1314272a5`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449e958dde8dd03ed487ed6b0df2995490dab77191cdb761ceeda156fd24689`  
		Last Modified: Wed, 19 May 2021 19:41:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210512` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:add50dcbe8d28e3d499ff6468fbbeb619e2accf42e3de6dd48561c30f7fd76d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30408205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5bc8205a89b4531107d3ff92acb6c883121ceb42f52e025f3213c0bb78033a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210512` - linux; s390x

```console
$ docker pull ubuntu@sha256:c5598bdf2533dab480dd217d2469bfcc0b797c934f8a43fbfa6a2cd19d438648
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25353592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550bb59094ec08dd44dbf938102b747c7a64eda1b182e42be293ecdaa1099eeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:28:29 GMT
ADD file:718406af36d25bc30b425ddad4eaa810e4f8cfe92388955edc07fd5ec9816dcc in / 
# Wed, 19 May 2021 23:28:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:28:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 23:28:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d5e421eb08da6bcb06173fcdd4e739a0fc77d7b26f72680342d8db9aedebf05`  
		Last Modified: Wed, 19 May 2021 23:30:36 GMT  
		Size: 25.4 MB (25352550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b74c33ee4c205747bbbc098fc12afc14cab69dd5b2186b8bf7ee58f516631b`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb318177ecfab6a1f7a7c8290c83d4d680cf1110f5b4d80fd059793e3b64708`  
		Last Modified: Wed, 19 May 2021 23:30:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:cf31af331f38d1d7158470e095b132acd126a7180a54f263d386da88eb681d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:86ac87f73641c920fb42cc9612d4fb57b5626b56ea2a19b894d0673fd5b4f2e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28540664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0aa2d69a153215c790488ed1fcec162015e973e49962d438e18249d16fa9bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a3e1155cd215efd134f7c70085a2674be897c9b6f7f421b8f19e46673ded3b87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24039589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd9976bcd84a12cfd82950c227f2b17e4033630e569ebc431a0c37409d3a072`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:44 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Fri, 23 Apr 2021 22:36:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3438cfd01915ec245a55dd1047748b26e29a31f4e630766126666c6bc9953a71`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc3cbbc3a3f69a5c07b934f21be14f7006510ff7a327d2f05f94ff680084d5`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1de4c5e2d8954bf5fa9855f8b4c9d3c3b97d1d380efe19f60f3e4107a66f5cae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a98cbe39225dadebcaa04e21dbe5900ad604739b07a9fa351dd10a6ebad4c1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:42d5c74d24685935e6167271ebb74c5898c5adf273dae80a82f9e39e8ae0dab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33256424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81ddd5d688c701fcfd0bf047bd4b9e3ee13f2801a76f37b4512761d369008a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:bdf7ff77dcb36ea18b53d7f2d340d8eea7bbb70e4a2609e959fe1162fd3a46ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27137388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230e5e1e3def457ce7266d68691dc4fc52ab00d071b7401d66d876d95745b65d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20210416`

```console
$ docker pull ubuntu@sha256:cf31af331f38d1d7158470e095b132acd126a7180a54f263d386da88eb681d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20210416` - linux; amd64

```console
$ docker pull ubuntu@sha256:86ac87f73641c920fb42cc9612d4fb57b5626b56ea2a19b894d0673fd5b4f2e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28540664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0aa2d69a153215c790488ed1fcec162015e973e49962d438e18249d16fa9bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210416` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a3e1155cd215efd134f7c70085a2674be897c9b6f7f421b8f19e46673ded3b87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24039589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd9976bcd84a12cfd82950c227f2b17e4033630e569ebc431a0c37409d3a072`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:44 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Fri, 23 Apr 2021 22:36:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3438cfd01915ec245a55dd1047748b26e29a31f4e630766126666c6bc9953a71`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc3cbbc3a3f69a5c07b934f21be14f7006510ff7a327d2f05f94ff680084d5`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210416` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1de4c5e2d8954bf5fa9855f8b4c9d3c3b97d1d380efe19f60f3e4107a66f5cae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a98cbe39225dadebcaa04e21dbe5900ad604739b07a9fa351dd10a6ebad4c1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210416` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:42d5c74d24685935e6167271ebb74c5898c5adf273dae80a82f9e39e8ae0dab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33256424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81ddd5d688c701fcfd0bf047bd4b9e3ee13f2801a76f37b4512761d369008a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210416` - linux; s390x

```console
$ docker pull ubuntu@sha256:bdf7ff77dcb36ea18b53d7f2d340d8eea7bbb70e4a2609e959fe1162fd3a46ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27137388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230e5e1e3def457ce7266d68691dc4fc52ab00d071b7401d66d876d95745b65d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:groovy`

```console
$ docker pull ubuntu@sha256:0971c3fba4ea1ba7012aff4c5ff2a02a1d9fe71f85bd6a2f6ff59939431c7484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:groovy` - linux; amd64

```console
$ docker pull ubuntu@sha256:870bba7433f601825f13b95a70b7df32f3ca5bb7ef0a865e8efc0a79e03e0c6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69040ea16df09b627e155acc7762b65b4474f341a3b09fee9b9f7e003224b8ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:28:11 GMT
ADD file:5582a76cd73639bd7b5f941762801034fe6d3297d63d8333085c79c31b5e777a in / 
# Wed, 26 May 2021 00:28:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:28:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:28:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:28:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0dfa4d6d32846900cdf518b31b7420c8e3bee78df56f061347f079b085e55eed`  
		Last Modified: Wed, 26 May 2021 00:29:22 GMT  
		Size: 31.3 MB (31339605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325ba66a34e9b2cf96e7958749a4fdd29a90699b6cd7eb67976c266a8277a26b`  
		Last Modified: Wed, 26 May 2021 00:29:18 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6382425bb0d013b4122cc28ffc63f8bce680a6562260cb6fa715f6f16a59db`  
		Last Modified: Wed, 26 May 2021 00:29:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6c6739fc427893da3110e2f2c631f34e1146dc28f99b08ef8de367ba6c389159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.3 MB (26302837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80239021fb9fa8a4c61c6e01eddbd4be06026a0545fff726543d44f18fbda922`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:22:24 GMT
ADD file:acda6861dee730077731d36484af6c3fa51a7ea2bcdbab39a88f53cb3276509e in / 
# Wed, 19 May 2021 20:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:22:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec376efdd72c4146827ffa866153a4452541beae9106def5a3afb4e858023939`  
		Last Modified: Wed, 19 May 2021 20:24:15 GMT  
		Size: 26.3 MB (26301801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065457da20bed844ec32f63c2c352d39da0d9cf58fd9fcdd710a8c2fe01e0ec`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffea83b1b3aaf9f535176139002bf18809b84cc711fddf2a83206c09194c8c`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:15507ed695229e52b84dbf79ab052b9c738917442244376d136ab0d99478c1c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29859198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae42a2f69b62859661cbea2a3c44cf7523fb015a05e5d3501223c3f767baf585`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:48:13 GMT
ADD file:3b909e405de304d3529a43650aa6812b726dbfe24e2f2a9c163818ab5c206cf1 in / 
# Fri, 23 Apr 2021 22:48:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:48:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:48:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:48:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0312c280f333ebad21d92c6554a1f0b81a5d7de275f2f1fe29c960721e40cb28`  
		Last Modified: Fri, 23 Apr 2021 22:50:26 GMT  
		Size: 29.9 MB (29858157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fedfba085a0c1226682c17f7966295deb654a557860da25aedabd09c96edf6`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d5a4de4889c6c2db1938b8170a1a427483a6b6ab113ceeae3e4b02819d54cf`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:39f41dfb4f2896402a9bf9e2b18b023bc5c01105ef74533f7822965f47ceb54f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36546459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6bfb84c7c6913211df3cfd6124ac66d4b4217cd9f27c173afcbb6d7383d6da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:59 GMT
ADD file:417e85e230e48984b1cc0db245a092e51901fd8cf010070a82fd06ccaec211df in / 
# Wed, 26 May 2021 00:51:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:51:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:51:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:51:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f7501b08507a493babfe9a7a361950a90febd51f598365c8c72a27438e176910`  
		Last Modified: Wed, 26 May 2021 00:54:09 GMT  
		Size: 36.5 MB (36545421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b1bdfb29d855647202d2d86b6473a9b637d7edaafa7d199fe951071b946c0`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63192a9aec9ad98562f0c79212fe107a71c90d1b3f55488cb16ca414d1d6853f`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; s390x

```console
$ docker pull ubuntu@sha256:b383d0b95879b99225bb648cf95a1869d18c272d021e447900a66c0ccbdcf1b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31564581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e08195772cd6a7e5593d472700d9fcd9744019b04ffe13cfece3135bfa4419e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:49 GMT
ADD file:953040401ce401194c7939af20d4b65872f29c9f1c9e9411f5b04fbd299161d6 in / 
# Wed, 26 May 2021 00:50:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:50:55 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:50:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:50:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a86f368f271868bec872a3e420550decf4fa2f153ca0ebcec9ab48b642f129b1`  
		Last Modified: Wed, 26 May 2021 00:52:15 GMT  
		Size: 31.6 MB (31563545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf527448b6952fd5c7da27d42ed151c11bafb569d579a96ce879307419f0970`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d46e2e6002b01a57ea745988830c3950a2aa33250abe3ebcd67891351feba1f`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:groovy-20210524`

```console
$ docker pull ubuntu@sha256:f712bd0d154a9eaca98f2e6ad98f59c59498c7487d7a53e217546046f1f3eec0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:groovy-20210524` - linux; amd64

```console
$ docker pull ubuntu@sha256:870bba7433f601825f13b95a70b7df32f3ca5bb7ef0a865e8efc0a79e03e0c6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69040ea16df09b627e155acc7762b65b4474f341a3b09fee9b9f7e003224b8ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:28:11 GMT
ADD file:5582a76cd73639bd7b5f941762801034fe6d3297d63d8333085c79c31b5e777a in / 
# Wed, 26 May 2021 00:28:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:28:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:28:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:28:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0dfa4d6d32846900cdf518b31b7420c8e3bee78df56f061347f079b085e55eed`  
		Last Modified: Wed, 26 May 2021 00:29:22 GMT  
		Size: 31.3 MB (31339605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325ba66a34e9b2cf96e7958749a4fdd29a90699b6cd7eb67976c266a8277a26b`  
		Last Modified: Wed, 26 May 2021 00:29:18 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6382425bb0d013b4122cc28ffc63f8bce680a6562260cb6fa715f6f16a59db`  
		Last Modified: Wed, 26 May 2021 00:29:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy-20210524` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:39f41dfb4f2896402a9bf9e2b18b023bc5c01105ef74533f7822965f47ceb54f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36546459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6bfb84c7c6913211df3cfd6124ac66d4b4217cd9f27c173afcbb6d7383d6da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:59 GMT
ADD file:417e85e230e48984b1cc0db245a092e51901fd8cf010070a82fd06ccaec211df in / 
# Wed, 26 May 2021 00:51:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:51:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:51:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:51:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f7501b08507a493babfe9a7a361950a90febd51f598365c8c72a27438e176910`  
		Last Modified: Wed, 26 May 2021 00:54:09 GMT  
		Size: 36.5 MB (36545421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b1bdfb29d855647202d2d86b6473a9b637d7edaafa7d199fe951071b946c0`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63192a9aec9ad98562f0c79212fe107a71c90d1b3f55488cb16ca414d1d6853f`  
		Last Modified: Wed, 26 May 2021 00:54:01 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy-20210524` - linux; s390x

```console
$ docker pull ubuntu@sha256:b383d0b95879b99225bb648cf95a1869d18c272d021e447900a66c0ccbdcf1b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31564581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e08195772cd6a7e5593d472700d9fcd9744019b04ffe13cfece3135bfa4419e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 May 2021 00:50:49 GMT
ADD file:953040401ce401194c7939af20d4b65872f29c9f1c9e9411f5b04fbd299161d6 in / 
# Wed, 26 May 2021 00:50:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 26 May 2021 00:50:55 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 26 May 2021 00:50:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 26 May 2021 00:50:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a86f368f271868bec872a3e420550decf4fa2f153ca0ebcec9ab48b642f129b1`  
		Last Modified: Wed, 26 May 2021 00:52:15 GMT  
		Size: 31.6 MB (31563545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf527448b6952fd5c7da27d42ed151c11bafb569d579a96ce879307419f0970`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d46e2e6002b01a57ea745988830c3950a2aa33250abe3ebcd67891351feba1f`  
		Last Modified: Wed, 26 May 2021 00:52:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `ubuntu:hirsute-20210522`

```console
$ docker pull ubuntu@sha256:e52b50d2b3237dfc0051f2b64f9427e79028dd0623598f6fa4b5327dae18bb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:hirsute-20210522` - linux; amd64

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

### `ubuntu:hirsute-20210522` - linux; ppc64le

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

### `ubuntu:hirsute-20210522` - linux; s390x

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

## `ubuntu:impish`

```console
$ docker pull ubuntu@sha256:d2ca9636434345840b6dae327fbe2d000d5289739987fa1410c76c2a9d774833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:impish` - linux; amd64

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

### `ubuntu:impish` - linux; ppc64le

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

### `ubuntu:impish` - linux; s390x

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

## `ubuntu:impish-20210519`

```console
$ docker pull ubuntu@sha256:d2ca9636434345840b6dae327fbe2d000d5289739987fa1410c76c2a9d774833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:impish-20210519` - linux; amd64

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

### `ubuntu:impish-20210519` - linux; ppc64le

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

### `ubuntu:impish-20210519` - linux; s390x

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

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:cf31af331f38d1d7158470e095b132acd126a7180a54f263d386da88eb681d93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:86ac87f73641c920fb42cc9612d4fb57b5626b56ea2a19b894d0673fd5b4f2e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28540664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0aa2d69a153215c790488ed1fcec162015e973e49962d438e18249d16fa9bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a3e1155cd215efd134f7c70085a2674be897c9b6f7f421b8f19e46673ded3b87
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24039589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd9976bcd84a12cfd82950c227f2b17e4033630e569ebc431a0c37409d3a072`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:36:44 GMT
ADD file:928fc93f670d53bf065ee8446f4af7f103050e96939dfae34f986b5332254115 in / 
# Fri, 23 Apr 2021 22:36:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:36:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:36:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:36:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd0d4853c44dd92753bc49779ae8c6f5bd76ba358989832b5afa42e3a341b4eb`  
		Last Modified: Fri, 23 Apr 2021 22:40:15 GMT  
		Size: 24.0 MB (24038553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3438cfd01915ec245a55dd1047748b26e29a31f4e630766126666c6bc9953a71`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc3cbbc3a3f69a5c07b934f21be14f7006510ff7a327d2f05f94ff680084d5`  
		Last Modified: Fri, 23 Apr 2021 22:40:09 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:1de4c5e2d8954bf5fa9855f8b4c9d3c3b97d1d380efe19f60f3e4107a66f5cae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27145456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a98cbe39225dadebcaa04e21dbe5900ad604739b07a9fa351dd10a6ebad4c1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:42d5c74d24685935e6167271ebb74c5898c5adf273dae80a82f9e39e8ae0dab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33256424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81ddd5d688c701fcfd0bf047bd4b9e3ee13f2801a76f37b4512761d369008a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:bdf7ff77dcb36ea18b53d7f2d340d8eea7bbb70e4a2609e959fe1162fd3a46ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27137388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230e5e1e3def457ce7266d68691dc4fc52ab00d071b7401d66d876d95745b65d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

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

### `ubuntu:rolling` - linux; amd64

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

### `ubuntu:rolling` - linux; arm variant v7

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

### `ubuntu:rolling` - linux; arm64 variant v8

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

### `ubuntu:rolling` - linux; ppc64le

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

### `ubuntu:rolling` - linux; s390x

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

## `ubuntu:trusty`

```console
$ docker pull ubuntu@sha256:4a8a6fa8810a3e01352981b35165b0b28403fe2a4e2535e315b23b4a69cd130a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull ubuntu@sha256:3c395cb9747f1d1513c3fa8a53b19c425e4fc43917c9c9204b69bf9001bf3c48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9ccf3968dbe6dfa7c2ee2f4b9fa9873977ea42634d6af78d255f76568f440d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Wed, 16 Sep 2020 22:29:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:29:45 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:29:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:29:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f0252367c5101cf7b90111c68054763b033350a90f2a18cc130ba9105769`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 76.8 KB (76772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4df6dcc20e58a34495cbea3866f25407b84dc9b253bf94d90de4d1fb20a8c5`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e0c3b6ef57e7710699c96f5b628199cc79f52feaddc96a8349ec2fa8ac1f9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e151b73d5f6446106434be4373ec707411667f1a313d00b983377c8f146de2fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Wed, 16 Sep 2020 23:17:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331949be49492d155af0307a821055a15f39e00916fd82acc0bc1aef242ed7e4`  
		Last Modified: Wed, 16 Sep 2020 23:19:11 GMT  
		Size: 59.1 KB (59097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9870c957ca40dbafea6c69c3cf4c8258e4114da0caa202e59f2268991aae7cd3`  
		Last Modified: Wed, 16 Sep 2020 23:19:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a664cf8519ac301fb0ef545c3b3e53dfdffcf9a0235ddaa51eca299948cc568f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3482d381e047de7cfaed92b88a16e086f36bb5c76d75b266bf2f14490b673e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Wed, 16 Sep 2020 23:58:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:58:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:58:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:58:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1599d04814b0dacc320abd16ec9e1d0d3d344ca7656ed5504d1c529489feb6ca`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef37a9325c7a10b2959384fb20a3c89ddc6c3374693c7d50248ed1eae25653`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty-20191217`

```console
$ docker pull ubuntu@sha256:4a8a6fa8810a3e01352981b35165b0b28403fe2a4e2535e315b23b4a69cd130a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull ubuntu@sha256:3c395cb9747f1d1513c3fa8a53b19c425e4fc43917c9c9204b69bf9001bf3c48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b9ccf3968dbe6dfa7c2ee2f4b9fa9873977ea42634d6af78d255f76568f440d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Wed, 16 Sep 2020 22:29:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:29:45 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:29:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:29:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810f0252367c5101cf7b90111c68054763b033350a90f2a18cc130ba9105769`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 76.8 KB (76772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4df6dcc20e58a34495cbea3866f25407b84dc9b253bf94d90de4d1fb20a8c5`  
		Last Modified: Wed, 16 Sep 2020 22:31:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e0c3b6ef57e7710699c96f5b628199cc79f52feaddc96a8349ec2fa8ac1f9c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e151b73d5f6446106434be4373ec707411667f1a313d00b983377c8f146de2fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Wed, 16 Sep 2020 23:17:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331949be49492d155af0307a821055a15f39e00916fd82acc0bc1aef242ed7e4`  
		Last Modified: Wed, 16 Sep 2020 23:19:11 GMT  
		Size: 59.1 KB (59097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9870c957ca40dbafea6c69c3cf4c8258e4114da0caa202e59f2268991aae7cd3`  
		Last Modified: Wed, 16 Sep 2020 23:19:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a664cf8519ac301fb0ef545c3b3e53dfdffcf9a0235ddaa51eca299948cc568f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3482d381e047de7cfaed92b88a16e086f36bb5c76d75b266bf2f14490b673e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Wed, 16 Sep 2020 23:58:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:58:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:58:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:58:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1599d04814b0dacc320abd16ec9e1d0d3d344ca7656ed5504d1c529489feb6ca`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef37a9325c7a10b2959384fb20a3c89ddc6c3374693c7d50248ed1eae25653`  
		Last Modified: Thu, 17 Sep 2020 00:02:32 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial`

```console
$ docker pull ubuntu@sha256:98afb2808ee1ec6aa4d7c8f8b82c6347b9ae156932f7186182b997f3d5616ebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial` - linux; amd64

```console
$ docker pull ubuntu@sha256:d7bb0589725587f2f67d0340edb81fd1fcba6c5f38166639cf2a252c939aa30c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff95a467e458bb9e8653b1df439e02e07fc0be5b362cc3d9aeb0d04039d5925`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5eb7810e4e9f5a336b6ab2fdecb4b467ad1ceae5a352d3fed5680d9c43170771
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b1e9393d1b4c129d2146619ad07abe90537f2e395ce7394c4c42404821d90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:23:21 GMT
ADD file:7e5c1f0262200ed290a61913d7f2c3b2b064c9b02aa1a55a818e38ab1316bbda in / 
# Wed, 19 May 2021 20:23:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:23:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 20:23:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:23:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ae1370da0037e05eb3f24cd486c49ee3a450840763c7d31deef8274cb9abfd86`  
		Last Modified: Wed, 19 May 2021 20:24:51 GMT  
		Size: 40.3 MB (40292258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452bc1820a9d9923cac2a73df110a9ad72318825a2ff4807ed5e89708052cea5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1217aa77f4015a99b17bec638b9f07cdf319ff342015b6c42800a588797d54a7`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84e209d76ee2a0ef7c673bb433398f6e5765eed483d8f68f8015126a1d3ce5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e8eb681cb9e01f339e1d68a47bf6d08a876f875ecf68f263891770bdc3400485
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41028247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f93e87bc68fc5d68ec7c669587d37ea34dc8143de2d4f43386d90a1b6ebab78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:49:13 GMT
ADD file:f7933af6e4e3a52794ae852310c5fd423b1afeb32576f8e3c3bc695db17d34e4 in / 
# Fri, 23 Apr 2021 22:49:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:49:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:49:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:49:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ea68ed57e24afe569fc149143e2b3c46c597abcbb61449c3652998e4bb1b5440`  
		Last Modified: Sat, 17 Apr 2021 00:25:08 GMT  
		Size: 41.0 MB (41026756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12a5b59372be005e03800813e52c56f42f21410e07162424afb9662a5620f7c`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a820d46388e3f6c8bd0bdd7d2079370426b00565c4fffac3f138c26af2408de2`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af45b45bb6a5e3119ffb671a33eb4a934675de944eee38f1aba43f3967c533`  
		Last Modified: Fri, 23 Apr 2021 22:50:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:c33ba65d993289a57df23ed7bcf5a63ea337c56371102aff819c2434e04a59ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45786471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e39c4a62166c3ae7764aaa06b78b1340dfd6e9839813aa82229352f36960c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:41:16 GMT
ADD file:082ca60ab0fd6043fa0b84148070e08bd36e575f3d8970eed54fe4c23aecf44a in / 
# Wed, 19 May 2021 19:41:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:41:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:41:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:41:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b0e5cfe962be5da09713a785360c5afe671f77a12ab690cfff78d4dc4f7bb372`  
		Last Modified: Wed, 19 May 2021 19:42:19 GMT  
		Size: 45.8 MB (45784935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706307f7bb6b836ba10c2f2df595c44e8de7262991f317c23ef61a99660e00a9`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49163eca4e92d67eeb1efa9eeb705eef784becadff03a085232ec7d7061adb37`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d37544d5536a00ff5bc2e023bd9b65a71266f4dd32a8b9ac616adeaef86833`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f42387920067dfe092a27337e281548d68888e93b7ea710e452f012a859caed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47494580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426a54dd9a773d28f88ecc1445838d67e4e4c4143b2ee37e399eb8216a191cc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:32:17 GMT
ADD file:639591e81174c559325b9d1d20efd2f26714b2b054be088252ac55afb93858ed in / 
# Wed, 19 May 2021 21:32:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:32:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:33:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6bb4d8d9255ba68d96734382b8a7bd6608fff0a888c7c6b0aa52d9eb7fc8f11`  
		Last Modified: Wed, 19 May 2021 21:35:17 GMT  
		Size: 47.5 MB (47493078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8718cfe093a36e16721650cedbb150a6e4dd982dd642e6af508af7f2a9baa8`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425fa8f42a78e60d1c406959f5f6629a972fc542248c750f3b05d925a957c2e7`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973b2a3c74625a11480006478adbc31fb4b9522720386b3f19aa8c732a8f8cb`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; s390x

```console
$ docker pull ubuntu@sha256:85f0e3c6e17efd884f4925859d3b771819e2d4618f92feabb047e5e3a77ec1d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44062586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a5278b1b1fc11837808e9bf7e7e3831a53c47ac3b2c61f82bbc1dfb5065bc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:29:52 GMT
ADD file:d6162b58b24c8842e7bc7d3f9c318c9c914ea2f8d18de8081ee87ffda0c9bc23 in / 
# Wed, 19 May 2021 23:30:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:30:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 23:30:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:30:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5483b215c78221b499b39a57c60379b545a5ab9f9c2c206f8509236f72d6ec90`  
		Last Modified: Wed, 19 May 2021 23:31:17 GMT  
		Size: 44.1 MB (44061095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb39f9943e9829ed5fd8deaeddfad18f6f37dad3399c89d93b6a7fa7c2232f3`  
		Last Modified: Wed, 19 May 2021 23:31:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f68e1710512337a2a8cbf88f1e50225470073f9f58616d4241ea2b65b4616`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab0373bf4c06812031cf4deaf1959122cfd5fef7462f8e59e41dd4974563a8`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial-20210429`

```console
$ docker pull ubuntu@sha256:6a9db6e8f83e15979561199d3a1cefb6308c11b915c66f77f9078d2341e05914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial-20210429` - linux; amd64

```console
$ docker pull ubuntu@sha256:d7bb0589725587f2f67d0340edb81fd1fcba6c5f38166639cf2a252c939aa30c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff95a467e458bb9e8653b1df439e02e07fc0be5b362cc3d9aeb0d04039d5925`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210429` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5eb7810e4e9f5a336b6ab2fdecb4b467ad1ceae5a352d3fed5680d9c43170771
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8b1e9393d1b4c129d2146619ad07abe90537f2e395ce7394c4c42404821d90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:23:21 GMT
ADD file:7e5c1f0262200ed290a61913d7f2c3b2b064c9b02aa1a55a818e38ab1316bbda in / 
# Wed, 19 May 2021 20:23:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:23:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 20:23:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:23:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ae1370da0037e05eb3f24cd486c49ee3a450840763c7d31deef8274cb9abfd86`  
		Last Modified: Wed, 19 May 2021 20:24:51 GMT  
		Size: 40.3 MB (40292258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452bc1820a9d9923cac2a73df110a9ad72318825a2ff4807ed5e89708052cea5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1217aa77f4015a99b17bec638b9f07cdf319ff342015b6c42800a588797d54a7`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84e209d76ee2a0ef7c673bb433398f6e5765eed483d8f68f8015126a1d3ce5`  
		Last Modified: Wed, 19 May 2021 20:24:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210429` - linux; 386

```console
$ docker pull ubuntu@sha256:c33ba65d993289a57df23ed7bcf5a63ea337c56371102aff819c2434e04a59ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45786471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e39c4a62166c3ae7764aaa06b78b1340dfd6e9839813aa82229352f36960c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:41:16 GMT
ADD file:082ca60ab0fd6043fa0b84148070e08bd36e575f3d8970eed54fe4c23aecf44a in / 
# Wed, 19 May 2021 19:41:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:41:18 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:41:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:41:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b0e5cfe962be5da09713a785360c5afe671f77a12ab690cfff78d4dc4f7bb372`  
		Last Modified: Wed, 19 May 2021 19:42:19 GMT  
		Size: 45.8 MB (45784935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706307f7bb6b836ba10c2f2df595c44e8de7262991f317c23ef61a99660e00a9`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49163eca4e92d67eeb1efa9eeb705eef784becadff03a085232ec7d7061adb37`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d37544d5536a00ff5bc2e023bd9b65a71266f4dd32a8b9ac616adeaef86833`  
		Last Modified: Wed, 19 May 2021 19:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210429` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f42387920067dfe092a27337e281548d68888e93b7ea710e452f012a859caed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47494580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426a54dd9a773d28f88ecc1445838d67e4e4c4143b2ee37e399eb8216a191cc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 21:32:17 GMT
ADD file:639591e81174c559325b9d1d20efd2f26714b2b054be088252ac55afb93858ed in / 
# Wed, 19 May 2021 21:32:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:32:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:33:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6bb4d8d9255ba68d96734382b8a7bd6608fff0a888c7c6b0aa52d9eb7fc8f11`  
		Last Modified: Wed, 19 May 2021 21:35:17 GMT  
		Size: 47.5 MB (47493078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8718cfe093a36e16721650cedbb150a6e4dd982dd642e6af508af7f2a9baa8`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425fa8f42a78e60d1c406959f5f6629a972fc542248c750f3b05d925a957c2e7`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973b2a3c74625a11480006478adbc31fb4b9522720386b3f19aa8c732a8f8cb`  
		Last Modified: Wed, 19 May 2021 21:35:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210429` - linux; s390x

```console
$ docker pull ubuntu@sha256:85f0e3c6e17efd884f4925859d3b771819e2d4618f92feabb047e5e3a77ec1d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44062586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a5278b1b1fc11837808e9bf7e7e3831a53c47ac3b2c61f82bbc1dfb5065bc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 23:29:52 GMT
ADD file:d6162b58b24c8842e7bc7d3f9c318c9c914ea2f8d18de8081ee87ffda0c9bc23 in / 
# Wed, 19 May 2021 23:30:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 23:30:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 23:30:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 23:30:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5483b215c78221b499b39a57c60379b545a5ab9f9c2c206f8509236f72d6ec90`  
		Last Modified: Wed, 19 May 2021 23:31:17 GMT  
		Size: 44.1 MB (44061095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb39f9943e9829ed5fd8deaeddfad18f6f37dad3399c89d93b6a7fa7c2232f3`  
		Last Modified: Wed, 19 May 2021 23:31:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f68e1710512337a2a8cbf88f1e50225470073f9f58616d4241ea2b65b4616`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ab0373bf4c06812031cf4deaf1959122cfd5fef7462f8e59e41dd4974563a8`  
		Last Modified: Wed, 19 May 2021 23:31:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
