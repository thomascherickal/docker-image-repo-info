## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:eb5c0723b9f6606b7e4d2bacf0bd4c73f7744a42bbe2efc7deade4c3b6c019db
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:8fbc33f46226f23126e16188eb4950f7c471ba49c6f579f7e8c7bb6419d1b52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.0 MB (203963745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7334b58ef2e50efd647155a27538b9cc6f110246ab838e73b77b5a0bf29c10c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 10 Nov 2023 15:26:46 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 10 Nov 2023 15:26:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_VERSION=1.10.0-rc1
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc1-linux-x86_64.tar.gz'; 			sha256='fab4b6ae9f39b0a59e4d98db73b563521716cdcfe34247638146f208a57a5b5b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc1-linux-aarch64.tar.gz'; 			sha256='9388c0e8f16b19233a5a80d09d9f16cdb4f94c3b5f6ee9e0b6a0bf852299c30a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc1-linux-i686.tar.gz'; 			sha256='1c137371781d126d50871d394a70765ba610c8aaf2b70d0d87004c2e41e290e6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc1","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc1?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3957be72bebec83cfdbb5805a8ef6ff2f60a5d2895cacff4bb7ac16b9e0ff603`  
		Last Modified: Tue, 21 Nov 2023 06:17:05 GMT  
		Size: 2.2 MB (2222805 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bef7759662b230c2af50e66bf1f1d1fab085e4b5129919b4df15cd5e0a6de8ab`  
		Last Modified: Tue, 21 Nov 2023 06:17:09 GMT  
		Size: 170.3 MB (170322744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64891b7f1eec3a6f9f14536fc4f9cf1c2d2120fedb2d0ff04c466d3eee019117`  
		Last Modified: Tue, 21 Nov 2023 06:17:05 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:a5ae5cdd55a065674b29244d7c9d46a6d3b28ed18eb43747943162f16acaf3e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2248418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620293965f13763cd1738ee10316c2f95ad43b52216742b73110c3caf749285c`

```dockerfile
```

-	Layers:
	-	`sha256:4d2abd7b32a94827c6d98b4a160a8b6e2e2d5adee485cb0ef1da9ab0b847bc64`  
		Last Modified: Tue, 21 Nov 2023 06:17:05 GMT  
		Size: 2.2 MB (2231093 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2074629778bd768a6e2eee5ab1ebee744b368b9f19663332657054646b8aa1c`  
		Last Modified: Tue, 21 Nov 2023 06:17:05 GMT  
		Size: 17.3 KB (17325 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5682af8f0af4661d7a5392fcc0d52a65edd154e2621b819f8e775cb620e9ef89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196838941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b048ba6439610aa0999bf8d1451cbd8493faf3ce5355f20fe3c65ea8ad423edd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 10 Nov 2023 15:26:46 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 10 Nov 2023 15:26:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_VERSION=1.10.0-rc1
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc1-linux-x86_64.tar.gz'; 			sha256='fab4b6ae9f39b0a59e4d98db73b563521716cdcfe34247638146f208a57a5b5b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc1-linux-aarch64.tar.gz'; 			sha256='9388c0e8f16b19233a5a80d09d9f16cdb4f94c3b5f6ee9e0b6a0bf852299c30a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc1-linux-i686.tar.gz'; 			sha256='1c137371781d126d50871d394a70765ba610c8aaf2b70d0d87004c2e41e290e6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc1","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc1?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7125e296ac071a07e741c080fa505548be787bc563978ba1f28cbadf817a297`  
		Last Modified: Wed, 22 Nov 2023 11:43:36 GMT  
		Size: 2.2 MB (2210605 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38ae71756e65f8fab922040e60a0dd8dfe5963663426dd1eacb767b4c7923d3e`  
		Last Modified: Wed, 22 Nov 2023 11:43:41 GMT  
		Size: 164.6 MB (164563837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8dd2e0ef1995b0d9ff6b910c2c065d75b215f6b31a15adec8bbf9fe4128f5f93`  
		Last Modified: Wed, 22 Nov 2023 11:43:36 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:5e7cf83b1f9f082abc3cc4a312d1c1fe387b8edf5cab7c0845ccbaf88e262a8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2248749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c421f234f43a916aae58ba96bd53918789cc08b785a619ab6a132a435531f848`

```dockerfile
```

-	Layers:
	-	`sha256:cb46427a4e7a75dffb422e53269bc50ab5d352230b58c77b3ac0eac187dcf552`  
		Last Modified: Wed, 22 Nov 2023 11:43:36 GMT  
		Size: 2.2 MB (2231416 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7bb1d6fec831a7b59a0d1cd6f5ca19d44e00aff5ec939abd715dc38996fd1bd2`  
		Last Modified: Wed, 22 Nov 2023 11:43:36 GMT  
		Size: 17.3 KB (17333 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:679998ac9b2bceb779f4e56862e1aa82f721bc6f464f78ef1f890eb485f43f1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191219871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fedb8e38bffef6cb14a89f354abfb4eef72c3e0e6cfa29c87925b43f027310`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 10 Nov 2023 15:26:46 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 10 Nov 2023 15:26:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Nov 2023 15:26:46 GMT
ENV JULIA_VERSION=1.10.0-rc1
# Fri, 10 Nov 2023 15:26:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc1-linux-x86_64.tar.gz'; 			sha256='fab4b6ae9f39b0a59e4d98db73b563521716cdcfe34247638146f208a57a5b5b'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc1-linux-aarch64.tar.gz'; 			sha256='9388c0e8f16b19233a5a80d09d9f16cdb4f94c3b5f6ee9e0b6a0bf852299c30a'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc1-linux-i686.tar.gz'; 			sha256='1c137371781d126d50871d394a70765ba610c8aaf2b70d0d87004c2e41e290e6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc1","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc1?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:26:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc9ffab954c04639b90d80577244cd2c1e4f2c2489f2156de0adf605f8174ce7`  
		Last Modified: Tue, 21 Nov 2023 06:17:10 GMT  
		Size: 2.3 MB (2328503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6969c31872751df3d5d617511c0a8848169754ef1dad589564b38bea23afe1bd`  
		Last Modified: Tue, 21 Nov 2023 06:17:14 GMT  
		Size: 156.5 MB (156488364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:83ab679f8aee90be208b470b826c393d9fef7de07e40ff401b80aaf272178b62`  
		Last Modified: Tue, 21 Nov 2023 06:17:09 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:295c3f6524cf66660d2e243d44f6507a735632ae916de9850acee1a0cf2e441a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 KB (17084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c222d6e5be1a4c8aa9118c3d290c9675b84d753aff75ecd2b8aa0bb1050b5c`

```dockerfile
```

-	Layers:
	-	`sha256:c9c5f2d319146cfaeb40253216990067d3cc03ac7b866e163c53bd50df0a1ea8`  
		Last Modified: Tue, 21 Nov 2023 06:17:10 GMT  
		Size: 17.1 KB (17084 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:b6c596de81d68b7a22c35ec65e491622b6fce3a25e88ee5b0bc78edca7d81f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.6 MB (191550407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0d9d044caa31a37434b428554665f324b8966b508618aea8ff8712cf1ee64f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:a935b2993c62bfb1ade6ba0ffcf1f955422f6f76c63a723877d4bca5bb2aff7b in / 
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 03 Oct 2023 23:59:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c4a0eee30f72e7c0e9938500fbc7f30b5eb02d04d49bfe7f18a17af1a6d82f81`  
		Last Modified: Wed, 01 Nov 2023 00:26:59 GMT  
		Size: 35.3 MB (35293810 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f18b73091125f2b78d22b50ccf4901ba0daac56dcf2d60f317040a844f84eba1`  
		Last Modified: Wed, 01 Nov 2023 15:26:58 GMT  
		Size: 2.4 MB (2424869 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfbd9c969473c8dcca330f150bcf9fbe50fc63ba462e68ecd0d4c3f90887bef8`  
		Last Modified: Wed, 01 Nov 2023 15:27:10 GMT  
		Size: 153.8 MB (153831353 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a40791d2b612179a5f9ef6e9ed6c4b70d92c778b0644c1a058eb6138c8431c2`  
		Last Modified: Wed, 01 Nov 2023 15:26:58 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:ec8b50a7bfd7b4f702f34579b0b77dfe53c1ad38a6d4c5495dfaaf737d2c8861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 MB (2251550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1bcab6a3b4c78b4baee86cf644e553f6272779e4fd64d842c718ed2d889a24`

```dockerfile
```

-	Layers:
	-	`sha256:39a948527286455f4b804414127b15ee1b1b9f3e56d95c2e787de75c5015c994`  
		Last Modified: Wed, 01 Nov 2023 15:26:58 GMT  
		Size: 2.2 MB (2234571 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5d2020ec108a5338ebccab8139a2517c5bb5d4a4f225308d1147ebf9fb23b20f`  
		Last Modified: Wed, 01 Nov 2023 15:26:58 GMT  
		Size: 17.0 KB (16979 bytes)  
		MIME: application/vnd.in-toto+json
