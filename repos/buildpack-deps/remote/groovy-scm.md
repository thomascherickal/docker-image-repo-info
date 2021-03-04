## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:a9fb4439aff5a37d2fe8d7a114a0a284e0abc0783a5cde99e2540fd46f96e1b5
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
$ docker pull buildpack-deps@sha256:75b612ee4b46004f2773f5c634db0a011f8d069073c854f9b22445aa2b9769d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.5 MB (95546374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34412ad9527cb51aeb6b8c9bcc9ad1477b370584505c91ad48dc182ce9bceeeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:54 GMT
ADD file:040f5377eee4911128a2a905c24395f01f851e15b48eb119590403ccc061b848 in / 
# Thu, 04 Mar 2021 02:24:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:57 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:48:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Mar 2021 03:48:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de21e52cfb21f634ab48959716b6f989328d5324043d6a259ca15df8a04e7f8d`  
		Last Modified: Mon, 01 Mar 2021 16:34:23 GMT  
		Size: 31.3 MB (31348436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e557bdec7d1561d0553244d6aa08a4f152c6d6656c780009e85e8591d81a1af`  
		Last Modified: Thu, 04 Mar 2021 02:26:00 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f57cefb68887255bfffe7e6ddee55ac93c131dc9ceedf6bbf1dfec7836abe75`  
		Last Modified: Thu, 04 Mar 2021 02:26:00 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb869a239d5c5443b40ed649a95e7c62a882e7a712061ec5cd3761e45436a864`  
		Last Modified: Thu, 04 Mar 2021 03:53:54 GMT  
		Size: 5.4 MB (5402586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2aeda38c88bc817a684421cda9198d3b6d2b43685793c7f64b23dea700aad6`  
		Last Modified: Thu, 04 Mar 2021 03:53:54 GMT  
		Size: 3.7 MB (3662143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f19a369d5fd9a7ffd46c7fd658914b75bd0bed9331bf1aeac4fe19dc75cf09`  
		Last Modified: Thu, 04 Mar 2021 03:54:10 GMT  
		Size: 55.1 MB (55132197 bytes)  
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
$ docker pull buildpack-deps@sha256:96e70f911c89c56605da12838dace297cea4045227885e6e55541afec71686b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110640647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1af535f8a6075dabcab528c5cbaf9ce9fc065de0b9e537bde3191a47d188357d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:a10e8e48da10ced8afe769f787ff5a4ca06f4fbd9fa540fc352cb1532f5cf79a in / 
# Thu, 21 Jan 2021 03:51:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:39 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:51:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:51 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 07:15:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:16:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 07:19:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef02a96d03691b901f9aaecbda4044e0a465bb09a96ec254a558f21aaa99d87d`  
		Last Modified: Mon, 18 Jan 2021 18:06:47 GMT  
		Size: 36.5 MB (36546462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86170ee335cc78e8dba1ebc6578dda027cebcf94e0c218542c7bd56823df23`  
		Last Modified: Thu, 21 Jan 2021 03:55:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa602367c34b7783eccd2b06110907f4ee35f7da6815511505d55c6a4ec4b4`  
		Last Modified: Thu, 21 Jan 2021 03:55:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699d439101b23a806560cdb986474df97e830feb91146f947cbec099e7eafdbb`  
		Last Modified: Thu, 21 Jan 2021 08:09:24 GMT  
		Size: 6.0 MB (6035868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98634b432b61959bbc5fbfa90c2bff853805200b53df947d94a0a421453a20e3`  
		Last Modified: Thu, 21 Jan 2021 08:09:23 GMT  
		Size: 4.5 MB (4506849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52624b6e57f5f99c4e395157e0deda953759dad356f5e26a73a5cf06488c8605`  
		Last Modified: Thu, 21 Jan 2021 08:09:51 GMT  
		Size: 63.6 MB (63550427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3618f046bedec0dd90ae2ba5246b97b1afe5c4af6372834341c784b016666588
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96668377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f440d5c1ddbc4477495fd679836d7433cdb9ec8e9ec9277d93216cb97d65d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:52 GMT
ADD file:9eaef80dfffe586684f11d475b678ca4ee498248fc71bad3946b676aa7293195 in / 
# Thu, 04 Mar 2021 02:47:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:55 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:56 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:30:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:30:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 04 Mar 2021 03:31:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2fece171627877339747c54fc8f877e712ab2d95c4f25e504b086dbce816637`  
		Last Modified: Mon, 01 Mar 2021 16:53:14 GMT  
		Size: 31.6 MB (31554858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed262f8a209a0550d194452d736a32fdf876fdfdb91b18e967192cb6e8d11238`  
		Last Modified: Thu, 04 Mar 2021 02:48:52 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46966d0c6ef65d3bfc7dc58455b472f85be1b5612d62a280e0cccc497d4c0517`  
		Last Modified: Thu, 04 Mar 2021 02:48:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e29518e6ad3684bd866ec5492fed181b4230d4ec1d03808249819b8f38cf`  
		Last Modified: Thu, 04 Mar 2021 03:34:48 GMT  
		Size: 5.6 MB (5628493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02572f10a16abbdb68a46afbb4e59a21b8961610adff357bcccb80584160fa79`  
		Last Modified: Thu, 04 Mar 2021 03:34:43 GMT  
		Size: 4.2 MB (4155727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1694eb963695359e3a226b5368986d652693c9369effddb066d6959139387b8`  
		Last Modified: Thu, 04 Mar 2021 03:35:03 GMT  
		Size: 55.3 MB (55328270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
