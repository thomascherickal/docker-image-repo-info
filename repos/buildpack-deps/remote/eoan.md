## `buildpack-deps:eoan`

```console
$ docker pull buildpack-deps@sha256:59aadbe8e5bc7732979e51b17fbda5a3b1e01032a45367d907d84f5749e4df98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:eoan` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ce4ef9de44e2d8da1cc44c3344adddc9be89f0b1d08ab6331c41d11c8c0b314d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234334353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa03af468a67e5e2abb685fb7df26fe482c23995fef5bf9896f279c5295a40b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:34 GMT
ADD file:537f9883fb90d19383082b8ac20c17b581db9045a48fa28b83cab73fe317047d in / 
# Fri, 20 Mar 2020 19:20:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:36 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:48:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:48:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:49:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:26:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeacba527962683a1b026af611fe162d35281159762b699172caa48c69480f79`  
		Last Modified: Mon, 16 Mar 2020 15:44:17 GMT  
		Size: 28.3 MB (28276050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25405ed4f245fc5627d0b03996d04c11d492c7a9ff937f4562a18e8757c39434`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 30.6 KB (30632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22752cd61bd53e9ac71e22fef539c165b3e11b368c1e54ca947260e317c4870a`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9460de83957c509dd234ede9ea96d4d03b7f9cd252ef1497844f8450dedb6570`  
		Last Modified: Fri, 20 Mar 2020 19:21:27 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42eb88f91904b1b4337337103ab96430c87f3ad2e37d3f822b84a655bd0809e`  
		Last Modified: Fri, 20 Mar 2020 19:57:01 GMT  
		Size: 6.5 MB (6512597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff84c2324c65af66e83971227b34dc08eb47fa329d526af15e72ee7c2243b8`  
		Last Modified: Fri, 20 Mar 2020 19:57:00 GMT  
		Size: 3.5 MB (3517022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e64540e87545fd02991a47180c59c4082383009f57dd967e9be025e7b35265`  
		Last Modified: Fri, 20 Mar 2020 19:57:15 GMT  
		Size: 47.4 MB (47369722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d39ccc51f0e89f50cc6728f95581d93701fc805deddd8b6d140cb546f0d28e`  
		Last Modified: Tue, 21 Apr 2020 01:38:37 GMT  
		Size: 148.6 MB (148627323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:72e66bc190f95db2312b9adac05b5dfcb265755d9060cdd6b29134f4f3b7311f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.8 MB (201780312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f6d5330e5695eb2ccc700096669e2f2ffcf4d5a4c9ba047c4a2288049a5d082`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:06:26 GMT
ADD file:a786d9ae5b3aaa37e3188ec13cba2efb20951cc432a05a3695210ce018439ce0 in / 
# Thu, 23 Apr 2020 22:06:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 22:06:43 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:06:45 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:06:46 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 12:25:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:26:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 12:28:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:35:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8729ee1b2c9c364007cc8f9967331e0464ea4d2ce5998811ea52e890737a4b7c`  
		Last Modified: Mon, 13 Apr 2020 15:44:38 GMT  
		Size: 23.7 MB (23735820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7153a6c4736e5469da08e1b45afdaeb7aa5d7864a7396c35f7799afb2a8c96c6`  
		Last Modified: Thu, 23 Apr 2020 22:08:32 GMT  
		Size: 30.6 KB (30618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2419c576e579e9eefaa1f9e5f5d8db949d4c09a789a577994d0f7237c35d4f9`  
		Last Modified: Thu, 23 Apr 2020 22:08:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f176618d72c6c467923dece921be857a756d30afd87f213c8658361102d14f3`  
		Last Modified: Thu, 23 Apr 2020 22:08:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b30b5dbb14c906a07aad7e49910a2a3bc2e2ce5a1e57c0c37c05fc801283301`  
		Last Modified: Fri, 24 Apr 2020 12:48:16 GMT  
		Size: 5.5 MB (5532892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48e073ec876479cc7eb8ae1cbe14afe25278c91ed319f83848df30560962f12`  
		Last Modified: Fri, 24 Apr 2020 12:48:15 GMT  
		Size: 3.0 MB (2983204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ea264d9f3ca10d420b0aeae6f7ddeb26faa4bdb51c12e83556f973659bcbd2`  
		Last Modified: Fri, 24 Apr 2020 12:48:40 GMT  
		Size: 43.1 MB (43132807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a74209326bb82807d51fc0cb2eb94b7b9ec0ecb92547cca20d5754b1a01e22c`  
		Last Modified: Fri, 24 Apr 2020 12:49:25 GMT  
		Size: 126.4 MB (126363931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2aae99f3cf3e5aabb24e34439ee224b0a94019f2eb01f247b0a3ef62a69613e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.4 MB (229435627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b098dfeb1c1334649b51d1eedf7628a4064cacaf669b00f72877bd6233e0f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:17:30 GMT
ADD file:ee5b532439ae81ec375590ce5538f3157e74936de2065e183983eb1b88a0d9c2 in / 
# Fri, 24 Apr 2020 00:17:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:17:43 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:54 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 16:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:01:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 16:02:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 16:04:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e232f54ba41e1aedbb70a6b06711c2133ee78faf50ec07fa8156e1390ee5c760`  
		Last Modified: Mon, 13 Apr 2020 15:44:34 GMT  
		Size: 26.9 MB (26869648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d7e01a364ea6224bdd8ba50bdc9067661a7586e87107f3e979b3a0a9e4d02`  
		Last Modified: Fri, 24 Apr 2020 00:21:33 GMT  
		Size: 30.5 KB (30457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e642e95286c1d4bcf9515a90456522a3f47ddbe52e5799e80e1d14e7d173ecef`  
		Last Modified: Fri, 24 Apr 2020 00:21:33 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e0b886ba6b67680a5d627be78d99d2db19a91a0c5f02f164d7b3abd3c33592`  
		Last Modified: Fri, 24 Apr 2020 00:21:33 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c585cbe8fa44af3648f22add7e96f48689a8699f0d3b7c0564f409ac08028d`  
		Last Modified: Fri, 24 Apr 2020 16:12:34 GMT  
		Size: 6.4 MB (6371011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037a2612054ab42ac962160699f4d87f82799a99d06bd2a4cf97510b327ac9fa`  
		Last Modified: Fri, 24 Apr 2020 16:12:33 GMT  
		Size: 3.5 MB (3511635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c1d8b3be5d59e8a112ba823b4fcc86c8ac88a6bdd552700bc21078d1ccfa50`  
		Last Modified: Fri, 24 Apr 2020 16:12:54 GMT  
		Size: 47.4 MB (47415975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d14a10bbe9eada266201941fb7bec3f502650ecd0c5407761271a6c9a05cf`  
		Last Modified: Fri, 24 Apr 2020 16:13:37 GMT  
		Size: 145.2 MB (145235867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4ee096d7608fb79b1c60241fc79b965252ab43eee836d7d38c48007273e92c58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.5 MB (238491917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbad7d2586db98b8263d31a5486871a606c01067fe522f74fefb6040ebef5a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 21:17:15 GMT
ADD file:f7ba0a72b1867680590e06dee4957489f61064444c99136216e872289753205b in / 
# Thu, 23 Apr 2020 21:17:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 21:17:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 21:17:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 21:17:18 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 09:05:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 09:05:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 09:06:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 09:08:21 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fcc600edb6cfd0f1f659b23300df5716d9534682f7bb847b2cf3fa623aa90a31`  
		Last Modified: Mon, 13 Apr 2020 15:44:55 GMT  
		Size: 29.0 MB (29044041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d3ca6655399bfe2c1ed6e5a5456d1d666e48dc9ed14da2a0cbb347933ab0ef`  
		Last Modified: Thu, 23 Apr 2020 21:18:04 GMT  
		Size: 30.7 KB (30696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7cdb9cb7ad5cdc2e1cc3e791d3dc33d99ce8079b4924664bc77a8af0dfcf38`  
		Last Modified: Thu, 23 Apr 2020 21:18:04 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec81ba1924129679b6fcec1e55d28a6d71fbcfbe7db715aea9ef144c50ac6d`  
		Last Modified: Thu, 23 Apr 2020 21:18:04 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a766ccdbe901ed5e2ffa8521e25dc52dc93157673fc3e64f66e7770118c4cc`  
		Last Modified: Fri, 24 Apr 2020 09:14:04 GMT  
		Size: 6.8 MB (6841269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48044873d3301355963c44fdfdcaafe8cec317eb1e7d10fb4cc46e4a8d8199e`  
		Last Modified: Fri, 24 Apr 2020 09:14:04 GMT  
		Size: 3.8 MB (3810325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2af3bea39a8764f3dfcc8e98d51f3fe3e006e66e744a3ebf47df8e5ea76177`  
		Last Modified: Fri, 24 Apr 2020 09:14:22 GMT  
		Size: 49.0 MB (49017315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd9e8bbddcf4416c21ad71c1c17cf99150d813b123c3f59a929199a2088c49e`  
		Last Modified: Fri, 24 Apr 2020 09:15:00 GMT  
		Size: 149.7 MB (149747263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c10fb367a16ee6c7eb28ba3c8508e635c7f1e71e644f1baa9bd8c0e81885a7b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260713305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9577552b3783e3b44902b91ebf6983b46e6011fe82172cc539307bd7b8283f90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 20:43:51 GMT
ADD file:3dddd0440bd0461ad738de1cac6d91b3e135f8ced829fe6b4ce68191764cbead in / 
# Thu, 23 Apr 2020 20:43:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 20:44:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:44:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:44:15 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 12:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:37:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 12:38:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:46:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92f1850658c279ede8a91155ce8c3448f24f41b6c34af2f7abc1758aa4b66da4`  
		Last Modified: Mon, 13 Apr 2020 15:45:23 GMT  
		Size: 33.0 MB (32986779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f77e23c3391871551319f5a95d13da7decaa4c5f82a6d8c5b7973466c8c759c`  
		Last Modified: Thu, 23 Apr 2020 20:49:15 GMT  
		Size: 30.5 KB (30496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d25529fd9371ec1a0256e037a3910b37015b517f876f30df0199a34a41c829`  
		Last Modified: Thu, 23 Apr 2020 20:49:15 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b901c3c78abc835c6887d98a6580e4b895cf612c470f317f39e5f46e2dbca0`  
		Last Modified: Thu, 23 Apr 2020 20:49:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02305273ba52f9a855a78ea8cb39ff2c511ec15e644f25c39aa6d0c371a6400`  
		Last Modified: Fri, 24 Apr 2020 13:18:57 GMT  
		Size: 7.4 MB (7420786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00441024500c01b26667ba67bf1ebccafcc416ef344b804c94baa59065a2c354`  
		Last Modified: Fri, 24 Apr 2020 13:18:56 GMT  
		Size: 4.5 MB (4463295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d010ffb83282fd735f60e9ba8ba424e6e9d4385da3156f0d6ff69f0f5aac54`  
		Last Modified: Fri, 24 Apr 2020 13:20:04 GMT  
		Size: 54.8 MB (54848682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e405549dbab2b3dfb5c496b94dbcf178b27aa6e62d7c12aa37ea55816a1a3b`  
		Last Modified: Fri, 24 Apr 2020 13:21:29 GMT  
		Size: 161.0 MB (160962223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b324174887ac6ae7a4969371ebf00917a86b4864f82a50c116b3893ec0481b07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.5 MB (218461067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb07ddfc7b59c4d14ac488ab89033c31d32a335e891f6284eaed06f7a54de17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:44 GMT
ADD file:590238292f6a053ea2bf6e08f583c7d381c15ead1a8a0f1bad600fca48d20648 in / 
# Thu, 23 Apr 2020 17:52:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:56 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:49:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:49:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 07:49:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:50:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4a7e39a0b3f9ba3421a213b5b6ae19b4ee4315b5aff0252496ef8117c7caae2e`  
		Last Modified: Mon, 13 Apr 2020 15:45:44 GMT  
		Size: 26.7 MB (26682562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15519bbe785a81349f4b9318ec98f07fb1d7ed9742eaf004a27806254935f5bf`  
		Last Modified: Thu, 23 Apr 2020 17:54:25 GMT  
		Size: 31.1 KB (31106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39a183d313a7aec756ef4cec9ebed83e7eefb892c64f68a74fb640abde8a647`  
		Last Modified: Thu, 23 Apr 2020 17:54:25 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0914614caf2827873d1d4b1f12426334285b8d984af44e48b64b7db18c3ee4fc`  
		Last Modified: Thu, 23 Apr 2020 17:54:30 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba99f74f403727ed8ce2e6a910248a0a53edf2bff04fe4fe7551ee0acbaaf849`  
		Last Modified: Fri, 24 Apr 2020 07:55:26 GMT  
		Size: 6.1 MB (6139662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7833d62efa3405cf0f7f73e663802e5167b8fe4fc84628bdc4e14a161891379`  
		Last Modified: Fri, 24 Apr 2020 07:55:26 GMT  
		Size: 3.4 MB (3433720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96a5c8eb18e8366958eb8cad11d8615cf9e6d5601789bc53fc94bd6febda994`  
		Last Modified: Fri, 24 Apr 2020 07:55:39 GMT  
		Size: 47.0 MB (47001567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac22e06bd8dbeb8326b1188155ccfe64f6d042e0b268634a74e79c5378a3aaf`  
		Last Modified: Fri, 24 Apr 2020 07:56:02 GMT  
		Size: 135.2 MB (135171413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
