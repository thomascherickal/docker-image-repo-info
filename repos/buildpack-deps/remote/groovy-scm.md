## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:6bdf3f626d49166d86cd4a998ed8cf38ad533cfd15da18cd2ecdb0da28ebe741
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d21b88f1ce5c970ea5e4f55bd42cbe322f8220a8126ca4804979129203a5f6e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95889836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939842f68ab8ac08c409b4989fbdb1382d799cf7a8fb472729860a7ff8d964dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:18 GMT
ADD file:4aba1ec4c6317039d27ed2f8cdda90160c834d979269ba6253f4b8839e6a8c06 in / 
# Thu, 25 Mar 2021 22:33:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:21 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:43:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 10:43:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67b8b51191f1c23048b4af7390755377b07b7033f43a5bc7a5bcf37f863f7adb`  
		Last Modified: Thu, 25 Mar 2021 22:35:06 GMT  
		Size: 31.3 MB (31348493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bee746ea8f946b8bb5dee1458e4bf97293706926511644fdfd4411b9bac5710`  
		Last Modified: Thu, 25 Mar 2021 22:35:01 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014d36ded12e82e314bb890faf3e15c110c39688e938f9c8c8ba8ebda5cbcbb7`  
		Last Modified: Thu, 25 Mar 2021 22:35:01 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9c37b96171571dc75418fdaead51ffde0478f656e8a8abba474da5f34e9982`  
		Last Modified: Fri, 26 Mar 2021 10:55:55 GMT  
		Size: 5.4 MB (5403819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126959169ae74465bee143ab20f409ffdbd10f26684b2284611d1380fda4ac47`  
		Last Modified: Fri, 26 Mar 2021 10:55:55 GMT  
		Size: 3.7 MB (3663037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f9f417ebd6fceb2f41c071071eb8113cbed20124275713383d643a00e3b3c4`  
		Last Modified: Fri, 26 Mar 2021 10:56:20 GMT  
		Size: 55.5 MB (55473449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3c14cb7a68ff47f918bf1b70ca646f37a6852a6e7c6b32ffd85da12f2f15efc2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84290439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f696830d0720f521c7ee98967e028e79e73b359c81bb5205ae6bbcc4eb06bc74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Mar 2021 03:12:15 GMT
ADD file:913cd61077b4364d8b370a1b3ec56fa4903b0514d25dbbd6f6935b3e6b7012c3 in / 
# Thu, 04 Mar 2021 03:12:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 03:12:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 03:12:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 03:12:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:53:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:53:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Mar 2021 03:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd497b823aefe08737b0ccec226c389310ebaa8dba94b4fee2b4670b873a1fd6`  
		Last Modified: Mon, 01 Mar 2021 16:53:02 GMT  
		Size: 26.3 MB (26305325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51bc255c8f40b519a7c9fdbdc13ff51d16d644e43283e0890887ff8c86770db`  
		Last Modified: Thu, 04 Mar 2021 03:13:45 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c588f540621d72d5d6aef336044cc3c14bcf9cfe6bd1f537d1764bdb451264`  
		Last Modified: Thu, 04 Mar 2021 03:13:45 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d865f1b57da14202590be5592605defc2bc452d162eab64c9e8e2d8f00b348b`  
		Last Modified: Thu, 04 Mar 2021 04:01:12 GMT  
		Size: 4.8 MB (4839197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e14a3851a41ecad0e0d14c5d8fcd5b43c7135ed603d19e54cce446eae706aa7`  
		Last Modified: Thu, 04 Mar 2021 04:01:11 GMT  
		Size: 3.1 MB (3139666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dbe51baa0c8548167474561a33e83a7976d86d224baccc584c5cc0830bda7b`  
		Last Modified: Thu, 04 Mar 2021 04:01:42 GMT  
		Size: 50.0 MB (50005214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:256e98e9baf5e75c170675fc2ba92662311710f86d1e7ee9a3be062e913dc445
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94047850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5ce995481c1946f96d4ecf3f2270cea797098a774cda834beb0c560ebe1265`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:53:13 GMT
ADD file:76ef7445bf6a89dcd1b3a65d97d32984cf5e9ba5a873b583685c90db6787cc9c in / 
# Thu, 04 Mar 2021 02:53:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:53:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:53:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:53:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:24:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:24:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Mar 2021 04:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:340a8d75d14b672cf98aa422c5d640a84745e6a9db9b4991bb86c41328cffb2f`  
		Last Modified: Mon, 01 Mar 2021 16:34:39 GMT  
		Size: 29.9 MB (29879299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9803d9cfbfa3fcf4921c891a5db6b6a87eb76984cdfe33dc73c9d1f9903752f`  
		Last Modified: Thu, 04 Mar 2021 02:54:53 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2d2226c7bce101efc57e60a1a525b17e7751b8368a2dd66adf2b8a17adad07`  
		Last Modified: Thu, 04 Mar 2021 02:54:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96aaec3dd6357a12ec08c1afa94f07abb8fbb6438710a36427edcb707214d27`  
		Last Modified: Thu, 04 Mar 2021 04:31:22 GMT  
		Size: 5.4 MB (5371448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd925d7b22821622b0e08b3be3632abf80f4242975b8d9482296818d1ae28b41`  
		Last Modified: Thu, 04 Mar 2021 04:31:21 GMT  
		Size: 3.6 MB (3634218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da9e0caef19e565ddaf2452ef676b5998b5e7a5d8b6a4da4ce7bce902ca2ee`  
		Last Modified: Thu, 04 Mar 2021 04:31:43 GMT  
		Size: 55.2 MB (55161850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:406adee29753caa4452768da58410b9639be66b5777e9d1e79fcc6bd14c96023
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110655750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8143182380dc8174d314167ab6f8ee67554b78a3223422a5d73c3567b26d11c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:59:07 GMT
ADD file:1f744d16a4497af1b967f7e85a48d8b8d93c5763bd87609256c052d413dd4aac in / 
# Thu, 04 Mar 2021 02:59:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:59:44 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 03:00:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 03:00:15 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:05:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:06:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Mar 2021 05:11:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ead43cfb2a3680f0bb194f098c2f47e89cc9988b239241b56c5e1ba8ef515f9b`  
		Last Modified: Mon, 01 Mar 2021 16:53:07 GMT  
		Size: 36.5 MB (36543595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991cee7a279cce929fff46b3b1a038186778e26296e3d7eb8b2abb051d4ec22`  
		Last Modified: Thu, 04 Mar 2021 03:02:32 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e119b0298590334832001ba977b4f1e488abbd58211c98bcfdd22a80cdb89bd`  
		Last Modified: Thu, 04 Mar 2021 03:02:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b6a4b3b63acbb1d916cddc10761e25d5ce43d58fa19bc7d32e1ca08c878d99`  
		Last Modified: Thu, 04 Mar 2021 05:31:12 GMT  
		Size: 6.0 MB (6039518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540394e214e7c285bdc14566b48f599570be95e17e7a51458d9bc80bc89edf6e`  
		Last Modified: Thu, 04 Mar 2021 05:31:11 GMT  
		Size: 4.5 MB (4520706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3112ca1e590c84348b5f4faa5bb8b29b7886cd4cb57e876babfd3ef9e4afe1ff`  
		Last Modified: Thu, 04 Mar 2021 05:31:39 GMT  
		Size: 63.6 MB (63550887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b496a6e62b75d870f2209e4918e19977b951c449787c2a4629e3dcca71f777e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101989889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6698f12e4f5221890b939962a47f6e96f7cbbe22246526becbb5a327291f7d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:51 GMT
ADD file:7945beb7b5ef4c133bdf7d9985c8bf01597f8529054f63bdd3248cc6f62898c6 in / 
# Thu, 25 Mar 2021 22:53:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:07:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:07:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 09:08:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff47e30c1aabcb1fb50a92bbf25aeb65010daab236491e40a6328f0d0837aedf`  
		Last Modified: Thu, 25 Mar 2021 22:54:56 GMT  
		Size: 31.6 MB (31555142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8d4f437f8df3327d0adb39cc03bee0f02236b2424230a1eb77593ae575e437`  
		Last Modified: Thu, 25 Mar 2021 22:54:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5ccf215f963aacb49a819b61b1f7658ff0d670b47ece9b0e8a8fa3ec074053`  
		Last Modified: Thu, 25 Mar 2021 22:54:51 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc20992cecbdf0269278df2147cd1afc47ee8194684c62516fb04e04cde2b94`  
		Last Modified: Fri, 26 Mar 2021 09:13:02 GMT  
		Size: 5.6 MB (5628850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83638988ee96c06d9bb6f2f756488c8f0c384f773c0f55bc6bf167d15486e8bf`  
		Last Modified: Fri, 26 Mar 2021 09:13:01 GMT  
		Size: 4.2 MB (4155848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e35596bd825564822fdd62bad760f3d970c85b41e25d6de3acb4e37cd3bcf1`  
		Last Modified: Fri, 26 Mar 2021 09:13:21 GMT  
		Size: 60.6 MB (60649009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
