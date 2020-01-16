## `buildpack-deps:disco-curl`

```console
$ docker pull buildpack-deps@sha256:c78736e304b862171e031d77bb8308dd93501299838e31fc3112449f85ef405f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:disco-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:317c7e2b1beda1963905ea3823b01c9db710c5c986a28834bde59724d9e175e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37846658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0e0da11b4ad2bc7ca27d2e745f03716a6d04418908405e986723f306f113b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:22:14 GMT
ADD file:440e68453fcfc383ab4ed0339f77dd56451b14f52cab4ee1e209062af03d5042 in / 
# Thu, 19 Dec 2019 04:22:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:22:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:22:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:22:17 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:25:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:25:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3e6c0c31900e0291814a94e9e8fe953d329b8f9f6a426659a45d7c05e08db089`  
		Last Modified: Thu, 28 Nov 2019 16:25:20 GMT  
		Size: 27.6 MB (27621412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b269ca9077748a3ef472411d5485716d58776f6e0635daa39d51bab4c48ca33`  
		Last Modified: Thu, 19 Dec 2019 04:25:06 GMT  
		Size: 31.0 KB (30991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78aeffdd139d0483a89257110baafbfa91ee684dca0bd8c30a4417cccf92f5b7`  
		Last Modified: Thu, 19 Dec 2019 04:25:05 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f2067539ba72f36bea210a390bcda78f3df29cc30b9e2b0dd69659ad579248`  
		Last Modified: Thu, 19 Dec 2019 04:25:05 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0621f3a9b9391f4bb6ec41d81eb260043bc789af61367922cec85c27c0650cf5`  
		Last Modified: Thu, 19 Dec 2019 07:40:09 GMT  
		Size: 6.7 MB (6678575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f457e320fd24a14498c03b68333f4c74dd616154bbbfe95788524b88db1043f7`  
		Last Modified: Thu, 19 Dec 2019 07:40:09 GMT  
		Size: 3.5 MB (3514654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:disco-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:24b09c2e9e4f9da77d63600b306235388a7c7f4f7735846b20ba0b74b9c4e83d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31776383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7800720b76a8b63aed06a8925211769c2ea368a0cab865c414d57442bc18efe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:00:17 GMT
ADD file:384f8d18a53011ddd03af96b468b0afeedf4c6f6dd2a57bc1ff87368bd8173b5 in / 
# Thu, 16 Jan 2020 01:00:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:00:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:00:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:00:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:55:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:55:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ade5766be18ba630432e0812858bc2eac396e21a5aa9c2409ae19457f8b74f5`  
		Last Modified: Thu, 16 Jan 2020 01:04:42 GMT  
		Size: 23.1 MB (23115380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ecb8600dea0f93648ac363c24a62237479abdf293ca63e212ca6affc4ca88a`  
		Last Modified: Thu, 16 Jan 2020 01:04:36 GMT  
		Size: 31.0 KB (30960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc691d616706ae63c1d5709858ab254ef22e2305f0f850387e0db1ec1c164f6`  
		Last Modified: Thu, 16 Jan 2020 01:04:36 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9e936f9b964d8716ddf35093a4481c7ae7078b4bef9cbb09453d4cc7a9cc78`  
		Last Modified: Thu, 16 Jan 2020 01:04:36 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb07d45d4059ec373cd7de1b7940641b7e6f7111767340218b02474d073469`  
		Last Modified: Thu, 16 Jan 2020 02:23:04 GMT  
		Size: 5.6 MB (5649963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0083f678b36be4c5fb4b7c9ffd3a29a9faef260dcc0c01320cdfd952ceeaf32a`  
		Last Modified: Thu, 16 Jan 2020 02:23:03 GMT  
		Size: 3.0 MB (2979030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:disco-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88f4fa4e98f24d82508171716c738fec5f24ab46762c8a52c21ba1325a68d3b1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36468397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9794c772a83359ce9e1edfff8cba19e964c5b94a8a7fe730183bdbd9748fbcce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:50:57 GMT
ADD file:74f072c21abc354f4180a342a84c4a92bd67887a975e13515af0e727fa871c1e in / 
# Thu, 19 Dec 2019 03:51:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:51:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:51:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:51:44 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:13:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:274e1e3371b9df5253f5129528edfcf609063a8cece74211061e6043da68ae53`  
		Last Modified: Thu, 28 Nov 2019 16:38:51 GMT  
		Size: 26.4 MB (26379071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6467cc73172e25ea7ce12129305cd7fc00af3ccb8176c4345c968d8d449b3b`  
		Last Modified: Thu, 19 Dec 2019 03:55:56 GMT  
		Size: 30.8 KB (30788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac06a88f4c8b446cba8f3dfac10f2a041fb9255d820ada2579734dafef65025`  
		Last Modified: Thu, 19 Dec 2019 03:55:56 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142f8a3358dc0b8523d6d567aa4078b40eb2debe886fd45844831852892cd46`  
		Last Modified: Thu, 19 Dec 2019 03:55:56 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a06dc5e0969290195ec067db1570c19e53225637bd7e23481b08fbbc0ef0d1`  
		Last Modified: Thu, 19 Dec 2019 08:29:58 GMT  
		Size: 6.5 MB (6548494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60ab4e4a03908816c18a914e659ee84b6c541c606505a6c5f803ce479e5e25`  
		Last Modified: Thu, 19 Dec 2019 08:29:58 GMT  
		Size: 3.5 MB (3508992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:disco-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:18f4fa89ea48d658e70bce29e357569feca00484487883f8dbaae134b239992b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39115659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c630d9ef06f0826cb003b4fb1594cd8719f70ca0453c5ab0690bb463f9827976`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:39:10 GMT
ADD file:c477d52ec717cb53e5817b327d0308d11c50bd5e7c2d81a31ee8916297b8442d in / 
# Thu, 16 Jan 2020 00:39:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:39:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:12 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:18:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:18:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2f9ab4800e0e314af7bfd3082450ef368771f164be61312bd04b6a007e47a2ed`  
		Last Modified: Thu, 16 Jan 2020 00:40:11 GMT  
		Size: 28.3 MB (28286786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2110375b0402410b62b24fbfc139e36da1c7eebade43b03f7a3c23907760cfea`  
		Last Modified: Thu, 16 Jan 2020 00:40:05 GMT  
		Size: 30.3 KB (30260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b87094fc5dfbfe60312bbbf356e25dff047c175174b037688a798b853b0db`  
		Last Modified: Thu, 16 Jan 2020 00:40:04 GMT  
		Size: 861.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df8c2e468085c82c9275f927f628a53bf7fc6157c52fc83d3577f17dac70bfd`  
		Last Modified: Thu, 16 Jan 2020 00:40:04 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf25c7f825165dce685fb554f10c7aca6745ce7f66070bce8cf5a58b12b377e`  
		Last Modified: Thu, 16 Jan 2020 01:31:32 GMT  
		Size: 7.0 MB (6990089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6822f5aff5bc8a3e047662a6c751f9d9992ce3dc38cdf64a00b23ab6ba934988`  
		Last Modified: Thu, 16 Jan 2020 01:31:31 GMT  
		Size: 3.8 MB (3807500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:disco-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:53507c7334f37fec4f492629db8199e9ee346ade66c3a5831378edfbcf7a8152
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45130383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b29935cbf5cfbdc1e63cc2aafdde3c8175382e40e4d589ff8000c3893b8f92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:18:33 GMT
ADD file:394daf793a5d7b5cb7fb572a5960a047efe20520c7a6787d9c8a9ea4f5cb6633 in / 
# Thu, 19 Dec 2019 04:18:39 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:18:43 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:18:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:18:50 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:26:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:27:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:702059b0e247216c6cf93ba4e221653678d273c975b436ebbaf4e874780b5805`  
		Last Modified: Mon, 02 Dec 2019 15:34:52 GMT  
		Size: 32.9 MB (32882734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637d574b844b44bfdc0d027d4c106b5541f75ff7dfb8890da44e5114680fa221`  
		Last Modified: Thu, 19 Dec 2019 04:24:43 GMT  
		Size: 30.8 KB (30815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4faa5981401c21195d49efdad19db21fbba891b4ad656483c01fe8c00b903`  
		Last Modified: Thu, 19 Dec 2019 04:24:43 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0556b5a5491e17a90ae90a4ee7ca32bd2c534fe22bb18f976180903fb465150`  
		Last Modified: Thu, 19 Dec 2019 04:24:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7822585ca804e3bb00abee5c0cc643b63e0aa3cc6e1575b01717f90d5d6e4d`  
		Last Modified: Thu, 19 Dec 2019 10:23:47 GMT  
		Size: 7.8 MB (7751290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22855e63c51a6b38ca023d5854f27975123671a456e96fc708b96955cebd7531`  
		Last Modified: Thu, 19 Dec 2019 10:23:43 GMT  
		Size: 4.5 MB (4464490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:disco-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:12d085486eb0890e097e0444b1439d40d48c880fd307b1c9a6cfdfe15052aa73
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35895165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa09e2a06df92deb776df258ba48ef26877d1f366c6dd5ee52a3981e1f78232`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:31 GMT
ADD file:318eee6ba2057b7f702cb9bbaad6258b63af005a971647afecaf3636246a0eb1 in / 
# Thu, 16 Jan 2020 00:45:31 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:33 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:25:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:002612794f82ebf4c1a9b95cc7fe6024e1c1165d606648edcedc16d65abb5337`  
		Last Modified: Thu, 16 Jan 2020 00:46:22 GMT  
		Size: 26.2 MB (26203510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df7a13961251867fdd28020f62a0e93cb02d9aecef3a10cc2a7481492188f4`  
		Last Modified: Thu, 16 Jan 2020 00:46:19 GMT  
		Size: 31.6 KB (31563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9afe8f91575638f4170c173cb7bd22f1cdf196f60eb5e4a8f2f952d57649e`  
		Last Modified: Thu, 16 Jan 2020 00:46:19 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002d7159090deb3d8525e65c7eab5849df26058d8929292b984bfc05564faff`  
		Last Modified: Thu, 16 Jan 2020 00:46:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b29a3acfad729b7dcfc690d753b0d5e8f5621bc08d80aaac5976965d9cbff86`  
		Last Modified: Thu, 16 Jan 2020 01:33:32 GMT  
		Size: 6.2 MB (6227101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeca26b2f8c2e15ea07ae9f7be34ad16aca5bc163898f47db32548186adad35d`  
		Last Modified: Thu, 16 Jan 2020 01:33:32 GMT  
		Size: 3.4 MB (3431970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
