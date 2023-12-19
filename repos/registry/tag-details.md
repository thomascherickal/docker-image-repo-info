<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `registry`

-	[`registry:2`](#registry2)
-	[`registry:2.8`](#registry28)
-	[`registry:2.8.3`](#registry283)
-	[`registry:3.0.0-alpha.1`](#registry300-alpha1)
-	[`registry:latest`](#registrylatest)

## `registry:2`

```console
$ docker pull registry@sha256:0a182cb82c93939407967d6d71d6caf11dcef0e5689c6afe2d60518e3b34ab86
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
$ docker pull registry@sha256:860f379a011eddfab604d9acfe3cf50b2d6e958026fb0f977132b0b083b1a3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10091524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909c3ff012b7f9fc4b802b73f250ad45e4ffa385299b71fdd6813f70a6711792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 05:59:31 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 05:59:31 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 05:59:31 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 05:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 05:59:31 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e875fe5e6b9cf6984ba5c486d6786a6e62f0725ccd08c8f925464cf3a39253e6`  
		Last Modified: Fri, 01 Dec 2023 05:59:41 GMT  
		Size: 6.4 MB (6403793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4bf2f86f9efe9ca5e2d78cda880ca1f2d8605d141e824e918ca984cbd7c13`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513cca25bbf844ab9c79643ad2b8e44ec938d7c81a094f1161c5c09538c2f6`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v6

```console
$ docker pull registry@sha256:fb6ae2c1ea0187406fe39a4ce923eb30e74aa9d7d396d2171b3e64e3c535a309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9456473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0dfab1fcd28281b3ab589f36e50194b875ad74b24afef4516dce19e45721658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 11:13:22 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 11:13:22 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 11:13:22 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 11:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:22 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0121d17a28a917cf8eed6df8437e20307da5470118b339c8d75bf042b7a6a7c`  
		Last Modified: Fri, 01 Dec 2023 11:13:31 GMT  
		Size: 6.0 MB (6024107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7352c67115d13474ebda7aa1eab3aa85f48e3f9870c0b217b3d69bb1df736047`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe926da741926c7f284fc8aa53c4bbab15e4907a25808099b913153ea0ca4f8`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v7

```console
$ docker pull registry@sha256:3166995ffab4033d4400c48a594ca3b2f754825b251b74e2d73e481c58ac612d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9202916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b0c275698e3f8b08827600f629044835f4d8d44e36f46011cc441c8f8630fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:08:47 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:08:47 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:08:48 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:08:48 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:08:48 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:08:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:08:48 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2a5c450ad539c19d039de6765a66bcea6ba840416ea012fadf23ab9c48c2d`  
		Last Modified: Fri, 01 Dec 2023 09:08:56 GMT  
		Size: 6.0 MB (6017219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d90b15526d5227036c129e5d6ba476db2c679a642368d75b83379112261aba3`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc8b927649fa946b85ca6841783a6cc126af20aba2c528dcce8aaae828f23eb`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:4881477afa5ca95c1aaea90a16038511f8ae719e204e1bcd4736b9c923422796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9444683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56655e0dde91bc61f6ca157985e67ac1098df556df011f9abeb0842766788a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 02:43:55 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 02:43:55 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 02:43:55 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 02:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 02:43:55 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c071d160e74fa00ea78c4aa36fa8406b604557eea293adb424584dbd48361bdd`  
		Last Modified: Fri, 01 Dec 2023 02:44:04 GMT  
		Size: 5.8 MB (5824732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fa29fe57de2c472c0482ef4001fb612dc1b233940645946131698421b8e39`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff48572bdb67fb86b487701204e3dafe44cd728c5baff6a58719641ad7ab11`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; ppc64le

```console
$ docker pull registry@sha256:66ae01fe8c805d611e1890a5d529ba462ccc111e499327033ae16547de7acf1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9324810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed66e38a7ef70eb6cec12254e785fb1cc1d42df29fb9ab327a80ae2d875ac17`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:20:14 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:20:14 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:20:15 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:20:15 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:20:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:20:17 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b951cfeed5797587ecf47747da15e3ecd147c4e7b7f3b6de280017b23dcdb896`  
		Last Modified: Fri, 01 Dec 2023 09:20:29 GMT  
		Size: 5.7 MB (5689216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206a7cc025f36aca61a70fbf339c31348236f6a0e1ea75675fa9137989733524`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d608cef607088cf39e2a4f5488511b4dedb6334d165cd0f787794a2ecd83da`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; s390x

```console
$ docker pull registry@sha256:99d58f17ef257c7195dca7084ca24ba9df47fa420ae055198f3a8ac9c3689c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294a423956e20e4d65a3ec7d35d38426590c6522c9bb669d1a89bde3b7b9f299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:23:56 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 08:23:56 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 08:23:56 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 08:23:57 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 08:23:57 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 08:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 08:23:57 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df1db0a68aeb6fbac17c638a66dccba8359333f6c239616dfed192320897054`  
		Last Modified: Fri, 01 Dec 2023 08:24:11 GMT  
		Size: 6.2 MB (6160052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c75b818b12c3588dcc656fac631ed2807f821f3b7c594f3b999593ec5dd274d`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951769fe941e528f7e7bf6acd99565734544a47731425ba83011de9f63dd96b2`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.8`

```console
$ docker pull registry@sha256:0a182cb82c93939407967d6d71d6caf11dcef0e5689c6afe2d60518e3b34ab86
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
$ docker pull registry@sha256:860f379a011eddfab604d9acfe3cf50b2d6e958026fb0f977132b0b083b1a3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10091524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909c3ff012b7f9fc4b802b73f250ad45e4ffa385299b71fdd6813f70a6711792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 05:59:31 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 05:59:31 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 05:59:31 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 05:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 05:59:31 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e875fe5e6b9cf6984ba5c486d6786a6e62f0725ccd08c8f925464cf3a39253e6`  
		Last Modified: Fri, 01 Dec 2023 05:59:41 GMT  
		Size: 6.4 MB (6403793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4bf2f86f9efe9ca5e2d78cda880ca1f2d8605d141e824e918ca984cbd7c13`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513cca25bbf844ab9c79643ad2b8e44ec938d7c81a094f1161c5c09538c2f6`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm variant v6

```console
$ docker pull registry@sha256:fb6ae2c1ea0187406fe39a4ce923eb30e74aa9d7d396d2171b3e64e3c535a309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9456473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0dfab1fcd28281b3ab589f36e50194b875ad74b24afef4516dce19e45721658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 11:13:22 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 11:13:22 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 11:13:22 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 11:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:22 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0121d17a28a917cf8eed6df8437e20307da5470118b339c8d75bf042b7a6a7c`  
		Last Modified: Fri, 01 Dec 2023 11:13:31 GMT  
		Size: 6.0 MB (6024107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7352c67115d13474ebda7aa1eab3aa85f48e3f9870c0b217b3d69bb1df736047`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe926da741926c7f284fc8aa53c4bbab15e4907a25808099b913153ea0ca4f8`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm variant v7

```console
$ docker pull registry@sha256:3166995ffab4033d4400c48a594ca3b2f754825b251b74e2d73e481c58ac612d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9202916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b0c275698e3f8b08827600f629044835f4d8d44e36f46011cc441c8f8630fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:08:47 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:08:47 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:08:48 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:08:48 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:08:48 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:08:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:08:48 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2a5c450ad539c19d039de6765a66bcea6ba840416ea012fadf23ab9c48c2d`  
		Last Modified: Fri, 01 Dec 2023 09:08:56 GMT  
		Size: 6.0 MB (6017219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d90b15526d5227036c129e5d6ba476db2c679a642368d75b83379112261aba3`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc8b927649fa946b85ca6841783a6cc126af20aba2c528dcce8aaae828f23eb`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:4881477afa5ca95c1aaea90a16038511f8ae719e204e1bcd4736b9c923422796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9444683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56655e0dde91bc61f6ca157985e67ac1098df556df011f9abeb0842766788a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 02:43:55 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 02:43:55 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 02:43:55 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 02:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 02:43:55 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c071d160e74fa00ea78c4aa36fa8406b604557eea293adb424584dbd48361bdd`  
		Last Modified: Fri, 01 Dec 2023 02:44:04 GMT  
		Size: 5.8 MB (5824732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fa29fe57de2c472c0482ef4001fb612dc1b233940645946131698421b8e39`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff48572bdb67fb86b487701204e3dafe44cd728c5baff6a58719641ad7ab11`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; ppc64le

```console
$ docker pull registry@sha256:66ae01fe8c805d611e1890a5d529ba462ccc111e499327033ae16547de7acf1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9324810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed66e38a7ef70eb6cec12254e785fb1cc1d42df29fb9ab327a80ae2d875ac17`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:20:14 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:20:14 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:20:15 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:20:15 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:20:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:20:17 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b951cfeed5797587ecf47747da15e3ecd147c4e7b7f3b6de280017b23dcdb896`  
		Last Modified: Fri, 01 Dec 2023 09:20:29 GMT  
		Size: 5.7 MB (5689216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206a7cc025f36aca61a70fbf339c31348236f6a0e1ea75675fa9137989733524`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d608cef607088cf39e2a4f5488511b4dedb6334d165cd0f787794a2ecd83da`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8` - linux; s390x

```console
$ docker pull registry@sha256:99d58f17ef257c7195dca7084ca24ba9df47fa420ae055198f3a8ac9c3689c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294a423956e20e4d65a3ec7d35d38426590c6522c9bb669d1a89bde3b7b9f299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:23:56 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 08:23:56 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 08:23:56 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 08:23:57 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 08:23:57 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 08:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 08:23:57 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df1db0a68aeb6fbac17c638a66dccba8359333f6c239616dfed192320897054`  
		Last Modified: Fri, 01 Dec 2023 08:24:11 GMT  
		Size: 6.2 MB (6160052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c75b818b12c3588dcc656fac631ed2807f821f3b7c594f3b999593ec5dd274d`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951769fe941e528f7e7bf6acd99565734544a47731425ba83011de9f63dd96b2`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.8.3`

```console
$ docker pull registry@sha256:0a182cb82c93939407967d6d71d6caf11dcef0e5689c6afe2d60518e3b34ab86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:2.8.3` - linux; amd64

```console
$ docker pull registry@sha256:860f379a011eddfab604d9acfe3cf50b2d6e958026fb0f977132b0b083b1a3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10091524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909c3ff012b7f9fc4b802b73f250ad45e4ffa385299b71fdd6813f70a6711792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 05:59:31 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 05:59:31 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 05:59:31 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 05:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 05:59:31 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e875fe5e6b9cf6984ba5c486d6786a6e62f0725ccd08c8f925464cf3a39253e6`  
		Last Modified: Fri, 01 Dec 2023 05:59:41 GMT  
		Size: 6.4 MB (6403793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4bf2f86f9efe9ca5e2d78cda880ca1f2d8605d141e824e918ca984cbd7c13`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513cca25bbf844ab9c79643ad2b8e44ec938d7c81a094f1161c5c09538c2f6`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.3` - linux; arm variant v6

```console
$ docker pull registry@sha256:fb6ae2c1ea0187406fe39a4ce923eb30e74aa9d7d396d2171b3e64e3c535a309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9456473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0dfab1fcd28281b3ab589f36e50194b875ad74b24afef4516dce19e45721658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 11:13:22 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 11:13:22 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 11:13:22 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 11:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:22 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0121d17a28a917cf8eed6df8437e20307da5470118b339c8d75bf042b7a6a7c`  
		Last Modified: Fri, 01 Dec 2023 11:13:31 GMT  
		Size: 6.0 MB (6024107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7352c67115d13474ebda7aa1eab3aa85f48e3f9870c0b217b3d69bb1df736047`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe926da741926c7f284fc8aa53c4bbab15e4907a25808099b913153ea0ca4f8`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.3` - linux; arm variant v7

```console
$ docker pull registry@sha256:3166995ffab4033d4400c48a594ca3b2f754825b251b74e2d73e481c58ac612d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9202916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b0c275698e3f8b08827600f629044835f4d8d44e36f46011cc441c8f8630fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:08:47 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:08:47 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:08:48 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:08:48 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:08:48 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:08:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:08:48 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2a5c450ad539c19d039de6765a66bcea6ba840416ea012fadf23ab9c48c2d`  
		Last Modified: Fri, 01 Dec 2023 09:08:56 GMT  
		Size: 6.0 MB (6017219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d90b15526d5227036c129e5d6ba476db2c679a642368d75b83379112261aba3`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc8b927649fa946b85ca6841783a6cc126af20aba2c528dcce8aaae828f23eb`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.3` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:4881477afa5ca95c1aaea90a16038511f8ae719e204e1bcd4736b9c923422796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9444683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56655e0dde91bc61f6ca157985e67ac1098df556df011f9abeb0842766788a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 02:43:55 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 02:43:55 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 02:43:55 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 02:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 02:43:55 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c071d160e74fa00ea78c4aa36fa8406b604557eea293adb424584dbd48361bdd`  
		Last Modified: Fri, 01 Dec 2023 02:44:04 GMT  
		Size: 5.8 MB (5824732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fa29fe57de2c472c0482ef4001fb612dc1b233940645946131698421b8e39`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff48572bdb67fb86b487701204e3dafe44cd728c5baff6a58719641ad7ab11`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.3` - linux; ppc64le

```console
$ docker pull registry@sha256:66ae01fe8c805d611e1890a5d529ba462ccc111e499327033ae16547de7acf1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9324810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed66e38a7ef70eb6cec12254e785fb1cc1d42df29fb9ab327a80ae2d875ac17`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:20:14 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:20:14 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:20:15 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:20:15 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:20:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:20:17 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b951cfeed5797587ecf47747da15e3ecd147c4e7b7f3b6de280017b23dcdb896`  
		Last Modified: Fri, 01 Dec 2023 09:20:29 GMT  
		Size: 5.7 MB (5689216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206a7cc025f36aca61a70fbf339c31348236f6a0e1ea75675fa9137989733524`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d608cef607088cf39e2a4f5488511b4dedb6334d165cd0f787794a2ecd83da`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.8.3` - linux; s390x

```console
$ docker pull registry@sha256:99d58f17ef257c7195dca7084ca24ba9df47fa420ae055198f3a8ac9c3689c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294a423956e20e4d65a3ec7d35d38426590c6522c9bb669d1a89bde3b7b9f299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:23:56 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 08:23:56 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 08:23:56 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 08:23:57 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 08:23:57 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 08:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 08:23:57 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df1db0a68aeb6fbac17c638a66dccba8359333f6c239616dfed192320897054`  
		Last Modified: Fri, 01 Dec 2023 08:24:11 GMT  
		Size: 6.2 MB (6160052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c75b818b12c3588dcc656fac631ed2807f821f3b7c594f3b999593ec5dd274d`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951769fe941e528f7e7bf6acd99565734544a47731425ba83011de9f63dd96b2`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:3.0.0-alpha.1`

```console
$ docker pull registry@sha256:5a6f2081e521a2b8d7a225d69dbc9149000bddb78edff55fa17e353e621ea115
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `registry:3.0.0-alpha.1` - linux; arm variant v6

```console
$ docker pull registry@sha256:b9bc48e4f87d57cc7196a94fd8180bdaf1420618e3a6b2c75cdcb3ca4379de3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13397369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11bae78972e152046c730c3f437ee31158a80fa042d6ef4850760afeaecbc0e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Tue, 19 Dec 2023 18:49:31 GMT
RUN set -eux; 	version='3.0.0-alpha.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='968a6dcc648aa842963ae00a28128200b6134732ff73db6fc1e52c6f9099d1f9' ;; 		aarch64) arch='arm64';   sha256='4f0d3ab06b8f77abf5ae39f08a214c2451b9eec4b1b9bb2eb9b9b9da3a3ad4cf' ;; 		armhf)   arch='armv6';   sha256='5ac4ac9cd5c7c658cd719efc44a67a0ef4b03e0618aa359ae726938eade66300' ;; 		armv7)   arch='armv7';   sha256='3c2eb167a162a17453dee0e43fb97b5abb771decf60b492e2867a2354fd0618d' ;; 		ppc64le) arch='ppc64le'; sha256='1e39ce43428437faf31f5df636d94c4dc21958076ebf96c1bd3baf67c3f7199a' ;; 		s390x)   arch='s390x';   sha256='94c53ba2254013b3e38d0c0a8d8005e41681f1f394c23a61db9953d61c134c07' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 19 Dec 2023 18:49:32 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 19 Dec 2023 18:49:32 GMT
VOLUME [/var/lib/registry]
# Tue, 19 Dec 2023 18:49:32 GMT
EXPOSE 5000
# Tue, 19 Dec 2023 18:49:32 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 19 Dec 2023 18:49:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 18:49:32 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ceb200511104b043198dbf160e1bdca9ba30c9f5ee53b33783eb084472220b3`  
		Last Modified: Tue, 19 Dec 2023 18:49:46 GMT  
		Size: 10.0 MB (9965003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e6c32259148b92d8e682121d58a8c7a46137a284795be244a5a6adc9de9a3d`  
		Last Modified: Tue, 19 Dec 2023 18:49:43 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79647b7c95df044d54f40f022d8d113709fec105f3cac3afe946300b0a64b232`  
		Last Modified: Tue, 19 Dec 2023 18:49:43 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:3.0.0-alpha.1` - linux; arm variant v7

```console
$ docker pull registry@sha256:0f9439b8aa4b197430cf9a670c1868bf052329396a3f1ebb642a021af374c6d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a57033cce6600ad0d15e89d94b49ec82bda990b5c122e41ca6addfb4642c01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 19 Dec 2023 21:53:45 GMT
RUN set -eux; 	version='3.0.0-alpha.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='968a6dcc648aa842963ae00a28128200b6134732ff73db6fc1e52c6f9099d1f9' ;; 		aarch64) arch='arm64';   sha256='4f0d3ab06b8f77abf5ae39f08a214c2451b9eec4b1b9bb2eb9b9b9da3a3ad4cf' ;; 		armhf)   arch='armv6';   sha256='5ac4ac9cd5c7c658cd719efc44a67a0ef4b03e0618aa359ae726938eade66300' ;; 		armv7)   arch='armv7';   sha256='3c2eb167a162a17453dee0e43fb97b5abb771decf60b492e2867a2354fd0618d' ;; 		ppc64le) arch='ppc64le'; sha256='1e39ce43428437faf31f5df636d94c4dc21958076ebf96c1bd3baf67c3f7199a' ;; 		s390x)   arch='s390x';   sha256='94c53ba2254013b3e38d0c0a8d8005e41681f1f394c23a61db9953d61c134c07' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 19 Dec 2023 21:53:45 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 19 Dec 2023 21:53:45 GMT
VOLUME [/var/lib/registry]
# Tue, 19 Dec 2023 21:53:45 GMT
EXPOSE 5000
# Tue, 19 Dec 2023 21:53:46 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 19 Dec 2023 21:53:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 21:53:46 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5362942bf2e8f101ff844dde2d5bdd7296f99e22a5099fd17f1626e7a96af13f`  
		Last Modified: Tue, 19 Dec 2023 21:53:59 GMT  
		Size: 10.0 MB (9954528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ec10c6493f87b8ba01602176d954fb262fad0331141c3d179b63f637bb8ea`  
		Last Modified: Tue, 19 Dec 2023 21:53:57 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a95e9d88a83c661d01655d3fe46e48342e0273034f6a17eb83f4d2d94ba4d`  
		Last Modified: Tue, 19 Dec 2023 21:53:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:3.0.0-alpha.1` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:72ff480556864721573b45b11f95d3ddf6444266339a96e5c8580563cbebd866
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13349445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fca0564182eb163b8dd7b8aa05c095457d4c04b80d64802edb0339c370d6cd9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Tue, 19 Dec 2023 22:07:22 GMT
RUN set -eux; 	version='3.0.0-alpha.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='968a6dcc648aa842963ae00a28128200b6134732ff73db6fc1e52c6f9099d1f9' ;; 		aarch64) arch='arm64';   sha256='4f0d3ab06b8f77abf5ae39f08a214c2451b9eec4b1b9bb2eb9b9b9da3a3ad4cf' ;; 		armhf)   arch='armv6';   sha256='5ac4ac9cd5c7c658cd719efc44a67a0ef4b03e0618aa359ae726938eade66300' ;; 		armv7)   arch='armv7';   sha256='3c2eb167a162a17453dee0e43fb97b5abb771decf60b492e2867a2354fd0618d' ;; 		ppc64le) arch='ppc64le'; sha256='1e39ce43428437faf31f5df636d94c4dc21958076ebf96c1bd3baf67c3f7199a' ;; 		s390x)   arch='s390x';   sha256='94c53ba2254013b3e38d0c0a8d8005e41681f1f394c23a61db9953d61c134c07' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 19 Dec 2023 22:07:22 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 19 Dec 2023 22:07:22 GMT
VOLUME [/var/lib/registry]
# Tue, 19 Dec 2023 22:07:23 GMT
EXPOSE 5000
# Tue, 19 Dec 2023 22:07:23 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 19 Dec 2023 22:07:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 22:07:23 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488ee1c8c604774b3ef5c80468211342aefdc783debf3d90fb83bf9b22292b84`  
		Last Modified: Tue, 19 Dec 2023 22:07:35 GMT  
		Size: 9.7 MB (9729494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f0b4b32b984465f9a2c2f80305db4019a8a0d4c3cfae695295192ef8bbb7fd`  
		Last Modified: Tue, 19 Dec 2023 22:07:34 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807ef47f5c68b2f7a1f8044cdbc823ed9ef2c34a8ecaed41cfdfa051ee151a5`  
		Last Modified: Tue, 19 Dec 2023 22:07:34 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:3.0.0-alpha.1` - linux; s390x

```console
$ docker pull registry@sha256:2e5fb530120c4563ace8293f4e7874cb298f1b5b60f632256dbdeb59f8e539f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13598351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e1e59108675092f7cc4900d265006c9f1c573b7f514d7375249b4e580735e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Tue, 19 Dec 2023 20:26:35 GMT
RUN set -eux; 	version='3.0.0-alpha.1'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='968a6dcc648aa842963ae00a28128200b6134732ff73db6fc1e52c6f9099d1f9' ;; 		aarch64) arch='arm64';   sha256='4f0d3ab06b8f77abf5ae39f08a214c2451b9eec4b1b9bb2eb9b9b9da3a3ad4cf' ;; 		armhf)   arch='armv6';   sha256='5ac4ac9cd5c7c658cd719efc44a67a0ef4b03e0618aa359ae726938eade66300' ;; 		armv7)   arch='armv7';   sha256='3c2eb167a162a17453dee0e43fb97b5abb771decf60b492e2867a2354fd0618d' ;; 		ppc64le) arch='ppc64le'; sha256='1e39ce43428437faf31f5df636d94c4dc21958076ebf96c1bd3baf67c3f7199a' ;; 		s390x)   arch='s390x';   sha256='94c53ba2254013b3e38d0c0a8d8005e41681f1f394c23a61db9953d61c134c07' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 19 Dec 2023 20:26:36 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 19 Dec 2023 20:26:36 GMT
VOLUME [/var/lib/registry]
# Tue, 19 Dec 2023 20:26:36 GMT
EXPOSE 5000
# Tue, 19 Dec 2023 20:26:37 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 19 Dec 2023 20:26:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 20:26:37 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9f15b569239982f8ae6630d9b2def6ddd9030ffb714d8f22fc379a5535969`  
		Last Modified: Tue, 19 Dec 2023 20:26:57 GMT  
		Size: 10.1 MB (10095195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaaa30c53056c1363b439eb6fac014c8ef78817f2328b54af526d274937b17e`  
		Last Modified: Tue, 19 Dec 2023 20:26:56 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1308a0f330e41f27686421339e65a605633447d89e32677b61675db025861dd`  
		Last Modified: Tue, 19 Dec 2023 20:26:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:latest`

```console
$ docker pull registry@sha256:0a182cb82c93939407967d6d71d6caf11dcef0e5689c6afe2d60518e3b34ab86
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
$ docker pull registry@sha256:860f379a011eddfab604d9acfe3cf50b2d6e958026fb0f977132b0b083b1a3d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10091524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909c3ff012b7f9fc4b802b73f250ad45e4ffa385299b71fdd6813f70a6711792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 05:59:31 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 05:59:31 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 05:59:31 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 05:59:31 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 05:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 05:59:31 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e875fe5e6b9cf6984ba5c486d6786a6e62f0725ccd08c8f925464cf3a39253e6`  
		Last Modified: Fri, 01 Dec 2023 05:59:41 GMT  
		Size: 6.4 MB (6403793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4bf2f86f9efe9ca5e2d78cda880ca1f2d8605d141e824e918ca984cbd7c13`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513cca25bbf844ab9c79643ad2b8e44ec938d7c81a094f1161c5c09538c2f6`  
		Last Modified: Fri, 01 Dec 2023 05:59:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:fb6ae2c1ea0187406fe39a4ce923eb30e74aa9d7d396d2171b3e64e3c535a309
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9456473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0dfab1fcd28281b3ab589f36e50194b875ad74b24afef4516dce19e45721658`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 11:13:22 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 11:13:22 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 11:13:22 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 11:13:22 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 11:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:22 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0121d17a28a917cf8eed6df8437e20307da5470118b339c8d75bf042b7a6a7c`  
		Last Modified: Fri, 01 Dec 2023 11:13:31 GMT  
		Size: 6.0 MB (6024107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7352c67115d13474ebda7aa1eab3aa85f48e3f9870c0b217b3d69bb1df736047`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe926da741926c7f284fc8aa53c4bbab15e4907a25808099b913153ea0ca4f8`  
		Last Modified: Fri, 01 Dec 2023 11:13:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v7

```console
$ docker pull registry@sha256:3166995ffab4033d4400c48a594ca3b2f754825b251b74e2d73e481c58ac612d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9202916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b0c275698e3f8b08827600f629044835f4d8d44e36f46011cc441c8f8630fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:08:47 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:08:47 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:08:48 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:08:48 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:08:48 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:08:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:08:48 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2a5c450ad539c19d039de6765a66bcea6ba840416ea012fadf23ab9c48c2d`  
		Last Modified: Fri, 01 Dec 2023 09:08:56 GMT  
		Size: 6.0 MB (6017219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d90b15526d5227036c129e5d6ba476db2c679a642368d75b83379112261aba3`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc8b927649fa946b85ca6841783a6cc126af20aba2c528dcce8aaae828f23eb`  
		Last Modified: Fri, 01 Dec 2023 09:08:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:4881477afa5ca95c1aaea90a16038511f8ae719e204e1bcd4736b9c923422796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9444683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56655e0dde91bc61f6ca157985e67ac1098df556df011f9abeb0842766788a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 02:43:55 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 02:43:55 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 02:43:55 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 02:43:55 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 02:43:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 02:43:55 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c071d160e74fa00ea78c4aa36fa8406b604557eea293adb424584dbd48361bdd`  
		Last Modified: Fri, 01 Dec 2023 02:44:04 GMT  
		Size: 5.8 MB (5824732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fa29fe57de2c472c0482ef4001fb612dc1b233940645946131698421b8e39`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff48572bdb67fb86b487701204e3dafe44cd728c5baff6a58719641ad7ab11`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; ppc64le

```console
$ docker pull registry@sha256:66ae01fe8c805d611e1890a5d529ba462ccc111e499327033ae16547de7acf1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9324810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed66e38a7ef70eb6cec12254e785fb1cc1d42df29fb9ab327a80ae2d875ac17`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 09:20:14 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 09:20:14 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 09:20:15 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 09:20:15 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 09:20:16 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 09:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:20:17 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b951cfeed5797587ecf47747da15e3ecd147c4e7b7f3b6de280017b23dcdb896`  
		Last Modified: Fri, 01 Dec 2023 09:20:29 GMT  
		Size: 5.7 MB (5689216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206a7cc025f36aca61a70fbf339c31348236f6a0e1ea75675fa9137989733524`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d608cef607088cf39e2a4f5488511b4dedb6334d165cd0f787794a2ecd83da`  
		Last Modified: Fri, 01 Dec 2023 09:20:27 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; s390x

```console
$ docker pull registry@sha256:99d58f17ef257c7195dca7084ca24ba9df47fa420ae055198f3a8ac9c3689c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294a423956e20e4d65a3ec7d35d38426590c6522c9bb669d1a89bde3b7b9f299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:23:56 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Fri, 01 Dec 2023 08:23:56 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Fri, 01 Dec 2023 08:23:56 GMT
VOLUME [/var/lib/registry]
# Fri, 01 Dec 2023 08:23:57 GMT
EXPOSE 5000
# Fri, 01 Dec 2023 08:23:57 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Fri, 01 Dec 2023 08:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 08:23:57 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df1db0a68aeb6fbac17c638a66dccba8359333f6c239616dfed192320897054`  
		Last Modified: Fri, 01 Dec 2023 08:24:11 GMT  
		Size: 6.2 MB (6160052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c75b818b12c3588dcc656fac631ed2807f821f3b7c594f3b999593ec5dd274d`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951769fe941e528f7e7bf6acd99565734544a47731425ba83011de9f63dd96b2`  
		Last Modified: Fri, 01 Dec 2023 08:24:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
