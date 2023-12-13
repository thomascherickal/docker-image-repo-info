## `julia:latest`

```console
$ docker pull julia@sha256:b4c77a71f83b54f2a2004b4c37205169900e0a582b1c2a14e5086aeff13e7d01
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:cac85d72f39f2cd687f4e3ca72f8d2168054526f84c6af22ca2649e5fd07404b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183238445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f86a5fde63b2c5d993ce973d21d30f03aa558151cb211bc23a04bf3fdf194c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5efbdc2ebf09ef570aaa6fd0accc2640f439d8db6a62904e0ae7544c59219699`  
		Last Modified: Tue, 21 Nov 2023 06:17:11 GMT  
		Size: 5.5 MB (5513932 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ebce95a9be2e1151edb3e59ac6ea7d7af35a9024086d9adf64d1d14bed6d4f5`  
		Last Modified: Tue, 21 Nov 2023 06:17:15 GMT  
		Size: 148.6 MB (148574235 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbe6b57d7f8d999957bbfd91cd41b7d478b3c6d4c21d54af282a105ff7319320`  
		Last Modified: Tue, 21 Nov 2023 06:17:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:latest` - unknown; unknown

```console
$ docker pull julia@sha256:8fecc8e23de9ffdf448cbbc6e8a83481edcf5bd5cc581a399b1857589de9aa29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2121809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ad78363b91f6efa8b7e94329f9ce7c3b67a98a5d1e63978a123e800db6f0cf1`

```dockerfile
```

-	Layers:
	-	`sha256:f8d35c76f9e48556a9bd9e7e8570848f4ed65eaf6fbf2add4c6783d45550064f`  
		Last Modified: Tue, 21 Nov 2023 06:17:11 GMT  
		Size: 2.1 MB (2102491 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e13ac30a55665f2d1000a74a0b6db35cb08e51c8474cbb45315e2af8211d7456`  
		Last Modified: Tue, 21 Nov 2023 06:17:10 GMT  
		Size: 19.3 KB (19318 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:fdc163a7f9d4317ab2f521df2112764480d890927864ececae297177506091c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177250566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd812cc53a7737158a3242122975da69165eb841cc1df95a8030131611bb4f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f85159850f58855dcffd5466740e815e89db336b54c17992bd695d28f6445907`  
		Last Modified: Wed, 22 Nov 2023 11:41:23 GMT  
		Size: 5.3 MB (5339531 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb285d3998b15f0dce9d2f1c3ca2b596f6acdac72856022308bf6db6a99aef6f`  
		Last Modified: Wed, 22 Nov 2023 11:44:36 GMT  
		Size: 142.7 MB (142731383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7295f223155951910d3a5863724b974cbc54ec53d0ae50cc1492b6dd294853e`  
		Last Modified: Wed, 22 Nov 2023 11:44:33 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:latest` - unknown; unknown

```console
$ docker pull julia@sha256:db8cffb3f2821a121007e33624c0d6d0ef6affc5b6bea7f5d12c5ddc9faca891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2122003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e214ba88571c81ef0596d2430e35525cefd5608eb1d66ff84ab32f7e73c38f2a`

```dockerfile
```

-	Layers:
	-	`sha256:32222188ac4cd669aa96d563a1669b13209e2caa392f60a2fdfafe62e6987357`  
		Last Modified: Wed, 22 Nov 2023 11:44:33 GMT  
		Size: 2.1 MB (2102834 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:da4ec56c3ef14c32756153144198df5d62b0da4636ddd767af66028913ae7e81`  
		Last Modified: Wed, 22 Nov 2023 11:44:33 GMT  
		Size: 19.2 KB (19169 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:0ae0863813fded32ba259f440f361c1576896521171f9b4041a82d15a5e29ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173105420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e4aa1f390be62e67bcc4929c1baea02c2afc0ce0b48aac7c036b0429a8c40d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d7cd90867b450ef3c3e781ddc1e00f4b6831fe3a4125c99581810e1daeb1664`  
		Last Modified: Tue, 21 Nov 2023 06:16:55 GMT  
		Size: 5.7 MB (5669529 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b08c1803543d7f23472e94e2f011318cfe309f23d12420c7f294b84a3e865a7b`  
		Last Modified: Tue, 21 Nov 2023 06:16:59 GMT  
		Size: 137.3 MB (137271414 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a435ad69b62cea8213cb59fc2affe7d8d565a311d9a488ad3b8217a933c0927`  
		Last Modified: Tue, 21 Nov 2023 06:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:latest` - unknown; unknown

```console
$ docker pull julia@sha256:88a32fc4cd8f61ea098f7cc22522f5ad6377d3700a2735de8e9b8c56efc2fb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 KB (19051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:211162025ab9c5d977ef27b6bf024d1b06c9b1aae8d8984ffd9d502038b33d8e`

```dockerfile
```

-	Layers:
	-	`sha256:6e2f6e837048c5981bf3680315abffd1e0f79146c0584585063437103f32e17a`  
		Last Modified: Tue, 21 Nov 2023 06:16:55 GMT  
		Size: 19.1 KB (19051 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:dd06a36b88132b66630d42417996f21d9b2a4caf07e8545e170eaec597370d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172174165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c965aa21b776f7eaeade75b0ec4d178a5260a21756f049a7d8c5c4ac9e8a0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07ccc63e35557563b4da5d8fa292d0ad021bcbb9995fe7c99490246f238b8ef1`  
		Last Modified: Tue, 21 Nov 2023 16:48:52 GMT  
		Size: 6.0 MB (6045874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47ed8e4d9ad432a0b1afc3d3e55d63d9f1bf7a0e3cd3bb77a7b96bdfad81c0ff`  
		Last Modified: Tue, 21 Nov 2023 16:48:55 GMT  
		Size: 133.0 MB (132986311 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d876d227c12584cb08d4923c41026c926b048e6b763db5e63d8276434a1b94e`  
		Last Modified: Tue, 21 Nov 2023 16:48:51 GMT  
		Size: 373.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:latest` - unknown; unknown

```console
$ docker pull julia@sha256:55228ff063c1653bf3225872dc8ba38ba5a618869685c064136b52d69098252c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2126409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf19d64d710e05fae37e8af20948aa972de64b7757c0a512cbe0cb196b84c03`

```dockerfile
```

-	Layers:
	-	`sha256:24eea3f73941bc674a7d5433d59f49859f01ec986c06e243860807f392e74d8e`  
		Last Modified: Tue, 21 Nov 2023 16:48:52 GMT  
		Size: 2.1 MB (2107028 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:98c87fd6d899525394ade41172f6cbbcaa154d08cd1908106f47cfb2f63abb65`  
		Last Modified: Tue, 21 Nov 2023 16:48:51 GMT  
		Size: 19.4 KB (19381 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:latest` - windows version 10.0.20348.2159; amd64

```console
$ docker pull julia@sha256:e8ae350fad38994e18e5629d416f5af53996a6c81b4566a2880394531192bb10
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2050937989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a56be2e208eadb76cfb9d6dac21e9c668515a940a1287cda85bb27309aeaa4`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Wed, 13 Dec 2023 01:00:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 01:00:40 GMT
ENV JULIA_VERSION=1.9.4
# Wed, 13 Dec 2023 01:00:41 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.4-win64.exe
# Wed, 13 Dec 2023 01:00:42 GMT
ENV JULIA_SHA256=8a491b31a8430c3662dff34bf349653e2d13ef98a4dcf7caa740359b6c5fef3e
# Wed, 13 Dec 2023 01:01:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 01:01:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c3d7d9e67d19f20b517c255509f543cdc513ced1bf6e4f52e86a3c8216ff97`  
		Last Modified: Wed, 13 Dec 2023 01:01:50 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19230b1f20bc3619715a10cbe43cfe909db3c0cdde738512c62373ead8e88c30`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0de6ec128bcc06ccd1d674892753b4f9a3f5f5374f498a2000b79877a2955e`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959173d16c0662324dbf72691a9129569bb673eb54d11c90e3eec8cea65ec96`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56553cb8fb17531c1d53f4ee3634cd4cdf0c4f0d20fe58f0fcbecce687f1550`  
		Last Modified: Wed, 13 Dec 2023 01:02:10 GMT  
		Size: 161.7 MB (161657448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3cd76f5ba33226dc072de95b22e8ffd072791762784856fcbd2e42e28257ea`  
		Last Modified: Wed, 13 Dec 2023 01:01:49 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.5206; amd64

```console
$ docker pull julia@sha256:e1d508ddc678da33ba7059509c666c8b5e00609ec9893856015a37753b520cf2
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2221367249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7a3030f61103b06c70e6e63b8dbebb2a03e5a72fcdc84127d23d3640131dc7b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Wed, 13 Dec 2023 00:59:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Wed, 13 Dec 2023 00:59:26 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.4-win64.exe
# Wed, 13 Dec 2023 00:59:26 GMT
ENV JULIA_SHA256=8a491b31a8430c3662dff34bf349653e2d13ef98a4dcf7caa740359b6c5fef3e
# Wed, 13 Dec 2023 01:01:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 01:01:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746378b37a6d8a631d7e79fc45399c0855998e354a13c0887f576815daa9c18a`  
		Last Modified: Wed, 13 Dec 2023 01:01:30 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df0849a1d21fdf6bcec3caba4e081e92f35e7ab04af9abe2858fa8d23373f81`  
		Last Modified: Wed, 13 Dec 2023 01:01:28 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca894edae761ee7ac28ddff4721d035dbc92f811a8084434479662e5b3acb78e`  
		Last Modified: Wed, 13 Dec 2023 01:01:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc74be6513022993310b9c7a67d4f4e366466d41bec174b25124718af9ed9c5`  
		Last Modified: Wed, 13 Dec 2023 01:01:28 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664e3c7593417896b7af1b9401b03ce08c0b30251a9a82f766e6bf531f6da53b`  
		Last Modified: Wed, 13 Dec 2023 01:01:50 GMT  
		Size: 161.7 MB (161651728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038c700ba2295acf65bf1430d06939639a9b5ebeb88b40703d51c2d20f015a04`  
		Last Modified: Wed, 13 Dec 2023 01:01:28 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
