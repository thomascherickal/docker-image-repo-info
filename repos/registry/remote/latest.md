## `registry:latest`

```console
$ docker pull registry@sha256:e964452846203f2ce4966e1d43281d37e9cdbf12022f4c6641bea4d00b36e8aa
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
$ docker pull registry@sha256:3c403e5d9c0125e68253050e2d49a7041d2f939a4ee3f2109822be7a423fec9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8569953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77497992d1cc1d68152e3efa42d91b24a9534d8323291043edc2b965aff8e8d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Sat, 08 Oct 2022 02:57:58 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 08 Oct 2022 02:57:58 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 08 Oct 2022 02:57:58 GMT
VOLUME [/var/lib/registry]
# Sat, 08 Oct 2022 02:57:58 GMT
EXPOSE 5000
# Sat, 08 Oct 2022 02:57:59 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 08 Oct 2022 02:57:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 08 Oct 2022 02:57:59 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1ecf3bffab6b082cae2805cd592e0024b07e625e7810833c3d3badd5c1fa71`  
		Last Modified: Sat, 08 Oct 2022 02:58:19 GMT  
		Size: 5.7 MB (5670686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d264c4cb646d6e3eb59e9fd32948351917f54784adf5a748e3afea25b8e022b`  
		Last Modified: Sat, 08 Oct 2022 02:58:18 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea66b4af353bef3dd23a60737d0f64178a8daeed2ddec85a0f3ec96fedb6cb5b`  
		Last Modified: Sat, 08 Oct 2022 02:58:18 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v7

```console
$ docker pull registry@sha256:856e0c9800df1470c0ea022137034cdc433e69b17dbabe29b6d622f11b2d6428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8367161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756bf2ab4de8ee2f08f3c9e0665cbdaed6ab7257c05ee9bdf8f4d4e4bced928`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 Aug 2022 02:47:50 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 11 Aug 2022 02:47:51 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 11 Aug 2022 02:47:51 GMT
VOLUME [/var/lib/registry]
# Thu, 11 Aug 2022 02:47:51 GMT
EXPOSE 5000
# Thu, 11 Aug 2022 02:47:51 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 11 Aug 2022 02:47:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 02:47:51 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecb342ccbc80554d1c07a229c787ff1fcf54215a6851667c6d8b0d8f3d595e7`  
		Last Modified: Thu, 11 Aug 2022 02:48:13 GMT  
		Size: 5.7 MB (5665666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e674c0b8a72796b1ad1d8cc97e4e94de61010ab0048047df93bb175cb5a73763`  
		Last Modified: Thu, 11 Aug 2022 02:48:12 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845c03b376db4320fb753f409ff334619c9541319016234075f8a87dafbee84`  
		Last Modified: Thu, 11 Aug 2022 02:48:12 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:d8ce78e6d1b909b07abac9fc2cbbc82a4359f89899a8286b4b4ad64b7e0f2494
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8537228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bcf88391173d5ffd5cc5542c0d3335124607bfe16f11d07bbbfcafd2348059`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 07:04:05 GMT
RUN set -eux; 	version='2.8.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='f1a376964912a5fd7d588107ebe5185da77803244e15476d483c945959347ee2' ;; 		aarch64) arch='arm64';   sha256='4c588c8e62c9a84f1eecfba4c842fe363b91be87fd42e3b5dac45148a2f46c52' ;; 		armhf)   arch='armv6';   sha256='d711b3b6e77f3acc7c89fad9310413ef145751ac702627dc1fa89991bf3b6104' ;; 		armv7)   arch='armv7';   sha256='d2f2180c1a847056f9c5dcfd1d6fda4c6086d126204541e0ed047c04f30a0f91' ;; 		ppc64le) arch='ppc64le'; sha256='ca77cdfb7b1415869558c118b5e783bb9d695a74d8426a0bd8d8a39beb23fb85' ;; 		s390x)   arch='s390x';   sha256='3e505af15c562870869441d5d1f79988c3c666b9a4370894ecf2f064860b48ba' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 07 Oct 2022 07:04:07 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 07 Oct 2022 07:04:07 GMT
VOLUME [/var/lib/registry]
# Fri, 07 Oct 2022 07:04:08 GMT
EXPOSE 5000
# Fri, 07 Oct 2022 07:04:10 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 07 Oct 2022 07:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:04:11 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb556f39845e9506e3500b5bb5e74c696935b5b3d729bb5c7121ba9a420ded8c`  
		Last Modified: Fri, 07 Oct 2022 07:04:30 GMT  
		Size: 5.5 MB (5544450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bbf04a79081d9f1f6cca63e9480201759523dd8129c33a90fa103740dada3b`  
		Last Modified: Fri, 07 Oct 2022 07:04:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c60cee15e894d66ba4a00568a27b094f725197640e58d81129d9241a13b2ee`  
		Last Modified: Fri, 07 Oct 2022 07:04:28 GMT  
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
