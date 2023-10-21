## `registry:latest`

```console
$ docker pull registry@sha256:c21c00cb0eaeb276c8c7533ab0bb81ae89c8f183d8b1576aa459dd22f17148b9
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
$ docker pull registry@sha256:c7e7796afbd3178fa965bff101e3a24ff5d024aea329c8cd66c213b6a99a644e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10091047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae1560ca86fd99c4932c235774a65173f550179a92e3ba101b2ef783a701d20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 03 Oct 2023 04:04:09 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 03 Oct 2023 04:04:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 03 Oct 2023 04:04:10 GMT
VOLUME [/var/lib/registry]
# Tue, 03 Oct 2023 04:04:10 GMT
EXPOSE 5000
# Tue, 03 Oct 2023 04:04:10 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 03 Oct 2023 04:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 03 Oct 2023 04:04:10 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a1aa97222427ee7d9c3e3c1d5b2d5538133b11259dc53e0322c293815d315`  
		Last Modified: Tue, 03 Oct 2023 04:04:21 GMT  
		Size: 6.4 MB (6403779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ff0af69d791a580f3ee5320e41cdeb6e9af91fc64620b25efe5ae74c8f2afc`  
		Last Modified: Tue, 03 Oct 2023 04:04:20 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17443307a4fc26d14cb10c30ce7c3f04a5fb1afb4e7e7d064a14d444505e4d77`  
		Last Modified: Tue, 03 Oct 2023 04:04:20 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:ef0761f4123d5a5f8bef6bcd6dcf64e5f6b64d8bd50d77faf27763caa0a358a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9454891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d304bc591a91bcab579c8c5dcc42a0f2d39794fed50fba2d41fce0daf6b404fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Sat, 21 Oct 2023 00:43:19 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 21 Oct 2023 00:43:19 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 21 Oct 2023 00:43:19 GMT
VOLUME [/var/lib/registry]
# Sat, 21 Oct 2023 00:43:19 GMT
EXPOSE 5000
# Sat, 21 Oct 2023 00:43:19 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:43:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:43:19 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c4d313d1c5bae6ab2e6cce25660ec750fa6fa615eeae309d85e604429cd76b`  
		Last Modified: Sat, 21 Oct 2023 00:43:28 GMT  
		Size: 6.0 MB (6024106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392234a55753865d296a55e7aea1c88a8f6edcf11fc06d908fd09ed96d514318`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2328408f21f593e8530046181a0b6f3143b2a01dd5fa6381acbbdd0e273797`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v7

```console
$ docker pull registry@sha256:de69e98781316c8f2701a0fdcef65ddcae9e0556444ae715b1f212dc589466e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9201811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b69f2a23fadcdf8de772cd63005516ff407c8ddfdeb6ed2807b1bd40baf7321`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Sat, 21 Oct 2023 01:07:32 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 21 Oct 2023 01:07:32 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 21 Oct 2023 01:07:32 GMT
VOLUME [/var/lib/registry]
# Sat, 21 Oct 2023 01:07:33 GMT
EXPOSE 5000
# Sat, 21 Oct 2023 01:07:33 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 21 Oct 2023 01:07:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 01:07:33 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdc25c78c6320d723eb83ac9f88cce561747a816e577db141512defb094570c`  
		Last Modified: Sat, 21 Oct 2023 01:07:43 GMT  
		Size: 6.0 MB (6017219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1d1e208a58be79fcd27e3a4d75515257cd3103d1059ceeb7469b3edbe2e990`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6552666e0a9959dae14630ad8b1878583616261685058957aba69b872b5bf9`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:8c3fe90b69e58516cb6c6203b98b6f6d9fa9f0c1639f46c08ec6dd8dfbe932d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9443480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98f2675080be6c716ca8fd019eaf9adcda2ba0349def7d5f546475aab8cf368`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:03:38 GMT
RUN apk add --no-cache ca-certificates
# Tue, 03 Oct 2023 04:17:46 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Tue, 03 Oct 2023 04:17:46 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Tue, 03 Oct 2023 04:17:46 GMT
VOLUME [/var/lib/registry]
# Tue, 03 Oct 2023 04:17:46 GMT
EXPOSE 5000
# Tue, 03 Oct 2023 04:17:47 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Tue, 03 Oct 2023 04:17:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 03 Oct 2023 04:17:47 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21914ef412ef71f6092299b025bf4d504a49024701bf684bc9efd218155c63`  
		Last Modified: Fri, 29 Sep 2023 01:03:48 GMT  
		Size: 286.3 KB (286306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965a63904b4247ac2324c3e7c0d0a12ca87a5cca50ab7869850c4220e6cad45b`  
		Last Modified: Tue, 03 Oct 2023 04:17:56 GMT  
		Size: 5.8 MB (5824732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52253bc9cdcdf12b78757bcb55bed3dc7bf483ee5ee13fab9e3c78c4d69c7eb`  
		Last Modified: Tue, 03 Oct 2023 04:17:55 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dac6f62e0d0014a22d520abd991d7dcfb9574086a51e5b29cddb1c0908b363`  
		Last Modified: Tue, 03 Oct 2023 04:17:55 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; ppc64le

```console
$ docker pull registry@sha256:0e349e3063ecc4fa1b70278dcf5dacb253567ccc5d79b21921b61060b897fec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9323000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cd816a3231311c3643fa1655eb155912a2da267d679878a92aa33df1369488b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Sat, 21 Oct 2023 00:50:08 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 21 Oct 2023 00:50:08 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 21 Oct 2023 00:50:09 GMT
VOLUME [/var/lib/registry]
# Sat, 21 Oct 2023 00:50:09 GMT
EXPOSE 5000
# Sat, 21 Oct 2023 00:50:09 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:50:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:50:10 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac2f4c8413c78a90db4d529e6b2b2a727112166d7907a16fe27d4cff250411c`  
		Last Modified: Sat, 21 Oct 2023 00:50:21 GMT  
		Size: 5.7 MB (5689216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d0cfbff5ff55ad587638e15636e61748271179f8dcd497a59df142dc9fc1b6`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c8b2c0e344960f0828a04567d8976893ec61266a0146d88bd94086377cd3b`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; s390x

```console
$ docker pull registry@sha256:598a61ae064a85cea4e7162643506d8a1600e741115fd627388f30cbd3db0830
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9660863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4082b3ffee44ee1f3e6d536db94dca79159394091c0004649994e43e294cf839`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Sat, 21 Oct 2023 00:44:46 GMT
RUN set -eux; 	version='2.8.3'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b1f750ecbe09f38e2143e22c61a25e3da2afe1510d9522859230b480e642ceff' ;; 		aarch64) arch='arm64';   sha256='7d2252eeeac97dd60fb9b36bebd15b95d7f947c4c82b8e0824cb55233ece9cd0' ;; 		armhf)   arch='armv6';   sha256='b00606466f976b6757268f1e7691918cbeca4af6fd4093a114b9186744ee8ef0' ;; 		armv7)   arch='armv7';   sha256='d3d7d958a7cc04159d43871261b1ed470ba72531d345fada311068962b967517' ;; 		ppc64le) arch='ppc64le'; sha256='9003659e5571bee89ee6d686057d02e9c0896d327276f268189922036e1ca84b' ;; 		s390x)   arch='s390x';   sha256='2c1347c73f881c320ff707055aecf649a888df39252e8bdc4fdfac7f59a383f1' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Sat, 21 Oct 2023 00:44:46 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Sat, 21 Oct 2023 00:44:46 GMT
VOLUME [/var/lib/registry]
# Sat, 21 Oct 2023 00:44:46 GMT
EXPOSE 5000
# Sat, 21 Oct 2023 00:44:47 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:44:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:44:47 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ebcfe33c20986dcaec85ca64e4e3c5b043b20e62267593d26f6e5f0303e997`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 6.2 MB (6160052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e38cfd9b82a55bf9cecaca8643f60a6726051b81629efad8a7c8704fae07a3`  
		Last Modified: Sat, 21 Oct 2023 00:44:59 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b9973ffb9464475d796f95bcf7cd5074822fdaf77d15ec42010994d1eeaf29`  
		Last Modified: Sat, 21 Oct 2023 00:44:59 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
