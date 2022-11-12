<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `registry`

-	[`registry:2`](#registry2)
-	[`registry:2.8`](#registry28)
-	[`registry:2.8.1`](#registry281)
-	[`registry:latest`](#registrylatest)

## `registry:2`

```console
$ docker pull registry@sha256:3e7b956e2ed16cd83121f285efce86f7f99579d9582b09edf9a2e1f7cbfbcc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:2` - linux; amd64

```console
$ docker pull registry@sha256:11bb1b1a54493dc3626f4bd3cdd74f83e4e5157239ea607a70cbe634f50bb89c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9197217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb3d42c17449436b2b75ef51b7ab9df91c403294c9b97da504cb56917af2842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 03:36:10 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 03:36:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 03:36:10 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 03:36:10 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 03:36:11 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 03:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 03:36:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6a6c5733af45e9529485356193e527ccb28fd2617c9bfc98e7e237b4840752`  
		Last Modified: Fri, 07 Oct 2022 03:36:23 GMT  
		Size: 6.1 MB (6105818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136d5c19b1da0f0d701b57e37bc8bedc173bcdc314255ec8274d3aa7399911d`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4a5435f342c8bab6154a6d584a1c2d5d38e612db1fe26eb258fc0da1ebbcc9`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v6

```console
$ docker pull registry@sha256:1aed93dd3bbcfa6cb7c2b34d72b3c7cda7a4ac2c5514e1bb07f9e65c2347ff02
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8571014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484ee5e0ac9884efb0df4890fb12fc7c5d1f53db956e049a1e3a60613ef75844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:12:13 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 08:12:15 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 08:12:15 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 08:12:15 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 08:12:16 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 08:12:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 08:12:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 08:12:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0748778b12033c88c7e03677ee64967de1101113fa637901277bce9624bf55`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 284.6 KB (284637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e52eb5f5e6317d293f5b3c7f4791f1d11e6216233264b6ea1ce9c68518bd2`  
		Last Modified: Sat, 12 Nov 2022 08:12:37 GMT  
		Size: 5.7 MB (5670688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc870a8c59287200d56b4dff441512feefe9a3e26357d8f93767127fe1b7b9e`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65572f819874d25d88df345faf5a1d9c8f90bddd85eef22d1faf5ca7fb78b8d6`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v7

```console
$ docker pull registry@sha256:b3256abf52ddc180bf6ade033d36db87584535fbb4dde979bb7887dbc9b06b82
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8368814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552d9229824aa8e9d3b7767a164ae8b87b96e407c6e6654d0eab5d552a1fcfc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:48:22 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 07:39:42 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 07:39:42 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 07:39:43 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 07:39:43 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 07:39:43 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 07:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 07:39:44 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a415398f56fd89230566f3c623eea17cc29b061818559ba9837ba1a4887b4cd`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 283.8 KB (283779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2985b75ffb7277e0af4f0ba32138e5ffbc08cbaafa8ee86e3a58e934856249`  
		Last Modified: Sat, 12 Nov 2022 07:40:06 GMT  
		Size: 5.7 MB (5665663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f35a40a61c3c6a4707e65800bd53125df681c82c7666ed6d280c4248a54916`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b90a370f6eaec648684bb229c57da61bca8f51b24151dc70ffc1aea34f170`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:5ca39447e22a9e806cab62b4e5e2b17da98ca6113a684c4ece72f8d37cb5aaed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8537456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a9b99971badf661b7041958513d3751044c16a00a613dbe65da792b634288c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:33:16 GMT
RUN apk add --no-cache ca-certificates
# Fri, 11 Nov 2022 10:59:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 11 Nov 2022 10:59:58 GMT
VOLUME [/var/lib/registry]
# Fri, 11 Nov 2022 10:59:58 GMT
EXPOSE 5000
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 11 Nov 2022 10:59:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 10:59:58 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8415f382965830234a69673048d6fa882f7175ec97a16992b879d5d4a2dc88e8`  
		Last Modified: Thu, 10 Nov 2022 21:39:30 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee67f647d65a58ecb4bf40f5d3cb957e9b3fc956cf81dd56b3f98bdadaa2d5f`  
		Last Modified: Fri, 11 Nov 2022 11:00:18 GMT  
		Size: 5.5 MB (5544457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9bab66e23c868da4ea5008f6a6176f7bdc46cdece00e811509d22adf0aaf8d`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c72f6ac9862aaa36a29163f839656b9aa8ba0283c7a5c2f76fe88adae9fd9`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; ppc64le

```console
$ docker pull registry@sha256:8f310e3982b1ba87f5ea7f7c9784222866c1e5509e908497cd69bb94b8dd979c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8405958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae1fa10bc3925145d17482a6b54bdf70f4a80b369acea0e4776061c184051e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 07:02:36 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 07:02:36 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 07:02:36 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 07:02:37 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 07:02:37 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 07:02:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:02:38 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c4e7a809aef7d2d2286f53f0ab8202889ab62e4e4aa37c362aa44ede3d3829`  
		Last Modified: Fri, 07 Oct 2022 07:02:59 GMT  
		Size: 5.3 MB (5315282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83514372477efeb9e3db0df5000ddc7fcb6a49f643ebd01f3ee506dcf5b4d42`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466369018e2f57f308829f188ea1ab9dec34369e9b480d882734ff187e424f7d`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; s390x

```console
$ docker pull registry@sha256:6465929d9408d02cf382deeca942b7b409679df24b66584b53971ac9e20f5125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8687719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3175df2169ddb7091a3c7e07bc2644eb29439a7c5cfb3a3a9d3ff3f03680fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:22:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 09:22:59 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 09:22:59 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 09:23:00 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 09:23:00 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 09:23:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:23:00 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037f11071fe29a7a8203a872a5afa3f906654430004f690bb3c62892b74de6a8`  
		Last Modified: Fri, 07 Oct 2022 09:23:20 GMT  
		Size: 5.8 MB (5811555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac317d99396baaa0e0a67ebb4e0997973504c8f1538249f5cb605858d668fe2c`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04604a51f8c29b012551b4143d17061b5a3b7345e580ea7ac9479618fb962ced`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.8`

```console
$ docker pull registry@sha256:3e7b956e2ed16cd83121f285efce86f7f99579d9582b09edf9a2e1f7cbfbcc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:2.8` - linux; amd64

```console
$ docker pull registry@sha256:11bb1b1a54493dc3626f4bd3cdd74f83e4e5157239ea607a70cbe634f50bb89c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9197217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb3d42c17449436b2b75ef51b7ab9df91c403294c9b97da504cb56917af2842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 03:36:10 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 03:36:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 03:36:10 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 03:36:10 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 03:36:11 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 03:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 03:36:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6a6c5733af45e9529485356193e527ccb28fd2617c9bfc98e7e237b4840752`  
		Last Modified: Fri, 07 Oct 2022 03:36:23 GMT  
		Size: 6.1 MB (6105818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136d5c19b1da0f0d701b57e37bc8bedc173bcdc314255ec8274d3aa7399911d`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4a5435f342c8bab6154a6d584a1c2d5d38e612db1fe26eb258fc0da1ebbcc9`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm variant v6

```console
$ docker pull registry@sha256:1aed93dd3bbcfa6cb7c2b34d72b3c7cda7a4ac2c5514e1bb07f9e65c2347ff02
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8571014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484ee5e0ac9884efb0df4890fb12fc7c5d1f53db956e049a1e3a60613ef75844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:12:13 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 08:12:15 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 08:12:15 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 08:12:15 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 08:12:16 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 08:12:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 08:12:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 08:12:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0748778b12033c88c7e03677ee64967de1101113fa637901277bce9624bf55`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 284.6 KB (284637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e52eb5f5e6317d293f5b3c7f4791f1d11e6216233264b6ea1ce9c68518bd2`  
		Last Modified: Sat, 12 Nov 2022 08:12:37 GMT  
		Size: 5.7 MB (5670688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc870a8c59287200d56b4dff441512feefe9a3e26357d8f93767127fe1b7b9e`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65572f819874d25d88df345faf5a1d9c8f90bddd85eef22d1faf5ca7fb78b8d6`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm variant v7

```console
$ docker pull registry@sha256:b3256abf52ddc180bf6ade033d36db87584535fbb4dde979bb7887dbc9b06b82
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8368814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552d9229824aa8e9d3b7767a164ae8b87b96e407c6e6654d0eab5d552a1fcfc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:48:22 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 07:39:42 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 07:39:42 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 07:39:43 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 07:39:43 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 07:39:43 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 07:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 07:39:44 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a415398f56fd89230566f3c623eea17cc29b061818559ba9837ba1a4887b4cd`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 283.8 KB (283779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2985b75ffb7277e0af4f0ba32138e5ffbc08cbaafa8ee86e3a58e934856249`  
		Last Modified: Sat, 12 Nov 2022 07:40:06 GMT  
		Size: 5.7 MB (5665663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f35a40a61c3c6a4707e65800bd53125df681c82c7666ed6d280c4248a54916`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b90a370f6eaec648684bb229c57da61bca8f51b24151dc70ffc1aea34f170`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:5ca39447e22a9e806cab62b4e5e2b17da98ca6113a684c4ece72f8d37cb5aaed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8537456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a9b99971badf661b7041958513d3751044c16a00a613dbe65da792b634288c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:33:16 GMT
RUN apk add --no-cache ca-certificates
# Fri, 11 Nov 2022 10:59:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 11 Nov 2022 10:59:58 GMT
VOLUME [/var/lib/registry]
# Fri, 11 Nov 2022 10:59:58 GMT
EXPOSE 5000
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 11 Nov 2022 10:59:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 10:59:58 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8415f382965830234a69673048d6fa882f7175ec97a16992b879d5d4a2dc88e8`  
		Last Modified: Thu, 10 Nov 2022 21:39:30 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee67f647d65a58ecb4bf40f5d3cb957e9b3fc956cf81dd56b3f98bdadaa2d5f`  
		Last Modified: Fri, 11 Nov 2022 11:00:18 GMT  
		Size: 5.5 MB (5544457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9bab66e23c868da4ea5008f6a6176f7bdc46cdece00e811509d22adf0aaf8d`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c72f6ac9862aaa36a29163f839656b9aa8ba0283c7a5c2f76fe88adae9fd9`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; ppc64le

```console
$ docker pull registry@sha256:8f310e3982b1ba87f5ea7f7c9784222866c1e5509e908497cd69bb94b8dd979c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8405958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae1fa10bc3925145d17482a6b54bdf70f4a80b369acea0e4776061c184051e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 07:02:36 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 07:02:36 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 07:02:36 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 07:02:37 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 07:02:37 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 07:02:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:02:38 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c4e7a809aef7d2d2286f53f0ab8202889ab62e4e4aa37c362aa44ede3d3829`  
		Last Modified: Fri, 07 Oct 2022 07:02:59 GMT  
		Size: 5.3 MB (5315282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83514372477efeb9e3db0df5000ddc7fcb6a49f643ebd01f3ee506dcf5b4d42`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466369018e2f57f308829f188ea1ab9dec34369e9b480d882734ff187e424f7d`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; s390x

```console
$ docker pull registry@sha256:6465929d9408d02cf382deeca942b7b409679df24b66584b53971ac9e20f5125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8687719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3175df2169ddb7091a3c7e07bc2644eb29439a7c5cfb3a3a9d3ff3f03680fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:22:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 09:22:59 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 09:22:59 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 09:23:00 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 09:23:00 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 09:23:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:23:00 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037f11071fe29a7a8203a872a5afa3f906654430004f690bb3c62892b74de6a8`  
		Last Modified: Fri, 07 Oct 2022 09:23:20 GMT  
		Size: 5.8 MB (5811555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac317d99396baaa0e0a67ebb4e0997973504c8f1538249f5cb605858d668fe2c`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04604a51f8c29b012551b4143d17061b5a3b7345e580ea7ac9479618fb962ced`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.8.1`

```console
$ docker pull registry@sha256:3e7b956e2ed16cd83121f285efce86f7f99579d9582b09edf9a2e1f7cbfbcc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:2.8.1` - linux; amd64

```console
$ docker pull registry@sha256:11bb1b1a54493dc3626f4bd3cdd74f83e4e5157239ea607a70cbe634f50bb89c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9197217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb3d42c17449436b2b75ef51b7ab9df91c403294c9b97da504cb56917af2842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 03:36:10 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 03:36:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 03:36:10 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 03:36:10 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 03:36:11 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 03:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 03:36:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6a6c5733af45e9529485356193e527ccb28fd2617c9bfc98e7e237b4840752`  
		Last Modified: Fri, 07 Oct 2022 03:36:23 GMT  
		Size: 6.1 MB (6105818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136d5c19b1da0f0d701b57e37bc8bedc173bcdc314255ec8274d3aa7399911d`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4a5435f342c8bab6154a6d584a1c2d5d38e612db1fe26eb258fc0da1ebbcc9`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.1` - linux; arm variant v6

```console
$ docker pull registry@sha256:1aed93dd3bbcfa6cb7c2b34d72b3c7cda7a4ac2c5514e1bb07f9e65c2347ff02
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8571014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484ee5e0ac9884efb0df4890fb12fc7c5d1f53db956e049a1e3a60613ef75844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:12:13 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 08:12:15 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 08:12:15 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 08:12:15 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 08:12:16 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 08:12:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 08:12:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 08:12:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0748778b12033c88c7e03677ee64967de1101113fa637901277bce9624bf55`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 284.6 KB (284637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e52eb5f5e6317d293f5b3c7f4791f1d11e6216233264b6ea1ce9c68518bd2`  
		Last Modified: Sat, 12 Nov 2022 08:12:37 GMT  
		Size: 5.7 MB (5670688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc870a8c59287200d56b4dff441512feefe9a3e26357d8f93767127fe1b7b9e`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65572f819874d25d88df345faf5a1d9c8f90bddd85eef22d1faf5ca7fb78b8d6`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.1` - linux; arm variant v7

```console
$ docker pull registry@sha256:b3256abf52ddc180bf6ade033d36db87584535fbb4dde979bb7887dbc9b06b82
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8368814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552d9229824aa8e9d3b7767a164ae8b87b96e407c6e6654d0eab5d552a1fcfc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:48:22 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 07:39:42 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 07:39:42 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 07:39:43 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 07:39:43 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 07:39:43 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 07:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 07:39:44 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a415398f56fd89230566f3c623eea17cc29b061818559ba9837ba1a4887b4cd`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 283.8 KB (283779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2985b75ffb7277e0af4f0ba32138e5ffbc08cbaafa8ee86e3a58e934856249`  
		Last Modified: Sat, 12 Nov 2022 07:40:06 GMT  
		Size: 5.7 MB (5665663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f35a40a61c3c6a4707e65800bd53125df681c82c7666ed6d280c4248a54916`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b90a370f6eaec648684bb229c57da61bca8f51b24151dc70ffc1aea34f170`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.1` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:5ca39447e22a9e806cab62b4e5e2b17da98ca6113a684c4ece72f8d37cb5aaed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8537456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a9b99971badf661b7041958513d3751044c16a00a613dbe65da792b634288c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:33:16 GMT
RUN apk add --no-cache ca-certificates
# Fri, 11 Nov 2022 10:59:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 11 Nov 2022 10:59:58 GMT
VOLUME [/var/lib/registry]
# Fri, 11 Nov 2022 10:59:58 GMT
EXPOSE 5000
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 11 Nov 2022 10:59:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 10:59:58 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8415f382965830234a69673048d6fa882f7175ec97a16992b879d5d4a2dc88e8`  
		Last Modified: Thu, 10 Nov 2022 21:39:30 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee67f647d65a58ecb4bf40f5d3cb957e9b3fc956cf81dd56b3f98bdadaa2d5f`  
		Last Modified: Fri, 11 Nov 2022 11:00:18 GMT  
		Size: 5.5 MB (5544457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9bab66e23c868da4ea5008f6a6176f7bdc46cdece00e811509d22adf0aaf8d`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c72f6ac9862aaa36a29163f839656b9aa8ba0283c7a5c2f76fe88adae9fd9`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.1` - linux; ppc64le

```console
$ docker pull registry@sha256:8f310e3982b1ba87f5ea7f7c9784222866c1e5509e908497cd69bb94b8dd979c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8405958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae1fa10bc3925145d17482a6b54bdf70f4a80b369acea0e4776061c184051e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 07:02:36 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 07:02:36 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 07:02:36 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 07:02:37 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 07:02:37 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 07:02:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:02:38 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c4e7a809aef7d2d2286f53f0ab8202889ab62e4e4aa37c362aa44ede3d3829`  
		Last Modified: Fri, 07 Oct 2022 07:02:59 GMT  
		Size: 5.3 MB (5315282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83514372477efeb9e3db0df5000ddc7fcb6a49f643ebd01f3ee506dcf5b4d42`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466369018e2f57f308829f188ea1ab9dec34369e9b480d882734ff187e424f7d`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.1` - linux; s390x

```console
$ docker pull registry@sha256:6465929d9408d02cf382deeca942b7b409679df24b66584b53971ac9e20f5125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8687719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3175df2169ddb7091a3c7e07bc2644eb29439a7c5cfb3a3a9d3ff3f03680fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:22:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 09:22:59 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 09:22:59 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 09:23:00 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 09:23:00 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 09:23:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:23:00 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037f11071fe29a7a8203a872a5afa3f906654430004f690bb3c62892b74de6a8`  
		Last Modified: Fri, 07 Oct 2022 09:23:20 GMT  
		Size: 5.8 MB (5811555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac317d99396baaa0e0a67ebb4e0997973504c8f1538249f5cb605858d668fe2c`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04604a51f8c29b012551b4143d17061b5a3b7345e580ea7ac9479618fb962ced`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:latest`

```console
$ docker pull registry@sha256:3e7b956e2ed16cd83121f285efce86f7f99579d9582b09edf9a2e1f7cbfbcc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:latest` - linux; amd64

```console
$ docker pull registry@sha256:11bb1b1a54493dc3626f4bd3cdd74f83e4e5157239ea607a70cbe634f50bb89c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9197217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb3d42c17449436b2b75ef51b7ab9df91c403294c9b97da504cb56917af2842`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 03:36:10 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 03:36:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 03:36:10 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 03:36:10 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 03:36:11 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 03:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 03:36:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6a6c5733af45e9529485356193e527ccb28fd2617c9bfc98e7e237b4840752`  
		Last Modified: Fri, 07 Oct 2022 03:36:23 GMT  
		Size: 6.1 MB (6105818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b136d5c19b1da0f0d701b57e37bc8bedc173bcdc314255ec8274d3aa7399911d`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4a5435f342c8bab6154a6d584a1c2d5d38e612db1fe26eb258fc0da1ebbcc9`  
		Last Modified: Fri, 07 Oct 2022 03:36:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:1aed93dd3bbcfa6cb7c2b34d72b3c7cda7a4ac2c5514e1bb07f9e65c2347ff02
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8571014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484ee5e0ac9884efb0df4890fb12fc7c5d1f53db956e049a1e3a60613ef75844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:12:13 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 08:12:15 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 08:12:15 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 08:12:15 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 08:12:16 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 08:12:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 08:12:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 08:12:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0748778b12033c88c7e03677ee64967de1101113fa637901277bce9624bf55`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 284.6 KB (284637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e52eb5f5e6317d293f5b3c7f4791f1d11e6216233264b6ea1ce9c68518bd2`  
		Last Modified: Sat, 12 Nov 2022 08:12:37 GMT  
		Size: 5.7 MB (5670688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc870a8c59287200d56b4dff441512feefe9a3e26357d8f93767127fe1b7b9e`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65572f819874d25d88df345faf5a1d9c8f90bddd85eef22d1faf5ca7fb78b8d6`  
		Last Modified: Sat, 12 Nov 2022 08:12:36 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v7

```console
$ docker pull registry@sha256:b3256abf52ddc180bf6ade033d36db87584535fbb4dde979bb7887dbc9b06b82
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8368814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552d9229824aa8e9d3b7767a164ae8b87b96e407c6e6654d0eab5d552a1fcfc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:48:22 GMT
RUN apk add --no-cache ca-certificates
# Sat, 12 Nov 2022 07:39:42 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 12 Nov 2022 07:39:42 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 12 Nov 2022 07:39:43 GMT
VOLUME [/var/lib/registry]
# Sat, 12 Nov 2022 07:39:43 GMT
EXPOSE 5000
# Sat, 12 Nov 2022 07:39:43 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 12 Nov 2022 07:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 07:39:44 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a415398f56fd89230566f3c623eea17cc29b061818559ba9837ba1a4887b4cd`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 283.8 KB (283779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2985b75ffb7277e0af4f0ba32138e5ffbc08cbaafa8ee86e3a58e934856249`  
		Last Modified: Sat, 12 Nov 2022 07:40:06 GMT  
		Size: 5.7 MB (5665663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f35a40a61c3c6a4707e65800bd53125df681c82c7666ed6d280c4248a54916`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b90a370f6eaec648684bb229c57da61bca8f51b24151dc70ffc1aea34f170`  
		Last Modified: Sat, 12 Nov 2022 07:40:05 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:5ca39447e22a9e806cab62b4e5e2b17da98ca6113a684c4ece72f8d37cb5aaed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8537456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a9b99971badf661b7041958513d3751044c16a00a613dbe65da792b634288c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:33:16 GMT
RUN apk add --no-cache ca-certificates
# Fri, 11 Nov 2022 10:59:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 11 Nov 2022 10:59:58 GMT
VOLUME [/var/lib/registry]
# Fri, 11 Nov 2022 10:59:58 GMT
EXPOSE 5000
# Fri, 11 Nov 2022 10:59:58 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 11 Nov 2022 10:59:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 10:59:58 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8415f382965830234a69673048d6fa882f7175ec97a16992b879d5d4a2dc88e8`  
		Last Modified: Thu, 10 Nov 2022 21:39:30 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee67f647d65a58ecb4bf40f5d3cb957e9b3fc956cf81dd56b3f98bdadaa2d5f`  
		Last Modified: Fri, 11 Nov 2022 11:00:18 GMT  
		Size: 5.5 MB (5544457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9bab66e23c868da4ea5008f6a6176f7bdc46cdece00e811509d22adf0aaf8d`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783c72f6ac9862aaa36a29163f839656b9aa8ba0283c7a5c2f76fe88adae9fd9`  
		Last Modified: Fri, 11 Nov 2022 11:00:17 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; ppc64le

```console
$ docker pull registry@sha256:8f310e3982b1ba87f5ea7f7c9784222866c1e5509e908497cd69bb94b8dd979c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8405958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae1fa10bc3925145d17482a6b54bdf70f4a80b369acea0e4776061c184051e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 07:02:36 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 07:02:36 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 07:02:36 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 07:02:37 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 07:02:37 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 07:02:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:02:38 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c4e7a809aef7d2d2286f53f0ab8202889ab62e4e4aa37c362aa44ede3d3829`  
		Last Modified: Fri, 07 Oct 2022 07:02:59 GMT  
		Size: 5.3 MB (5315282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83514372477efeb9e3db0df5000ddc7fcb6a49f643ebd01f3ee506dcf5b4d42`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466369018e2f57f308829f188ea1ab9dec34369e9b480d882734ff187e424f7d`  
		Last Modified: Fri, 07 Oct 2022 07:02:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; s390x

```console
$ docker pull registry@sha256:6465929d9408d02cf382deeca942b7b409679df24b66584b53971ac9e20f5125
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8687719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3175df2169ddb7091a3c7e07bc2644eb29439a7c5cfb3a3a9d3ff3f03680fb9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:22:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 09:22:59 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 09:22:59 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 09:23:00 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 09:23:00 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 09:23:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:23:00 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037f11071fe29a7a8203a872a5afa3f906654430004f690bb3c62892b74de6a8`  
		Last Modified: Fri, 07 Oct 2022 09:23:20 GMT  
		Size: 5.8 MB (5811555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac317d99396baaa0e0a67ebb4e0997973504c8f1538249f5cb605858d668fe2c`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04604a51f8c29b012551b4143d17061b5a3b7345e580ea7ac9479618fb962ced`  
		Last Modified: Fri, 07 Oct 2022 09:23:19 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
