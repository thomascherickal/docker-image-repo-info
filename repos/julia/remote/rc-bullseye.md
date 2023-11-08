## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:c2ef4a7fcad3e5bf45d916d517714e0c2d63a469124ac0c5603f24418f24cc5c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:72e6ceceb0ded9241a3acfa277bbff1acd6360307c87a30b8503938686b88c7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.5 MB (203477306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de5db095a77427fd6134a1cc691fe2064d15619f63768aa9999f6a95710c9e79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
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
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:885eadfa9cd2e3f1291fc4903294370e4e73cefa182450a3ff71679f50e28b44`  
		Last Modified: Wed, 01 Nov 2023 01:02:51 GMT  
		Size: 2.2 MB (2222898 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0c9c0017958d8c6fbcae0632cb225eed4572725cbac71019c0abcab42eda59f`  
		Last Modified: Wed, 01 Nov 2023 01:02:59 GMT  
		Size: 169.8 MB (169836123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5df414a20097762b937f2ed2e53d0232f89ea048843179ce08122703ac8ec22`  
		Last Modified: Wed, 01 Nov 2023 01:02:51 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:0dc0c1e5f0b4db43cc4f5afde52c11dbf06740d9b02f634769816136af4ea9e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15c80a6658e7b9a328e3c405b500d82dcd451f32f1944fe96cfad212da95418`

```dockerfile
```

-	Layers:
	-	`sha256:866cd216174298223f776f81a55697397e4ebceb97062f2ef876d01de1f4afdb`  
		Last Modified: Wed, 01 Nov 2023 01:02:51 GMT  
		Size: 2.2 MB (2230074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d19c8c8c2474e8534e344db85fab82ee1732846cff86a75e394810e093b11e9d`  
		Last Modified: Wed, 01 Nov 2023 01:02:51 GMT  
		Size: 16.9 KB (16945 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ae8244a9f779f14803b86b40ffd2f26c22d3335d82a1b0c47aff2f606a5de88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196807549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d004b3841d0c2e19fe0d4769f4886fff6efeb312faac26cd2ef13fd68066adfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
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
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3640f1ff51e1a9280840799ad065bae045b52c2572ba536bf458d0b49dd134fb`  
		Last Modified: Thu, 02 Nov 2023 04:26:22 GMT  
		Size: 2.2 MB (2210613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3b519ed482a8c0c1b5400e6cc4f5222236ff649bf3d3e52079f8cff2c78515d`  
		Last Modified: Thu, 02 Nov 2023 04:26:28 GMT  
		Size: 164.5 MB (164532660 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bd070ebcaf91323c3fdb4af837ca83d3d08dde04d09c760a26866c3114dcf6cf`  
		Last Modified: Thu, 02 Nov 2023 04:26:21 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:ace62a9967c44e2e3529a188a2707561ff88781cd9795ba95d1f4632cf625372
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2247183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:500265c83f6518e2561954dba4ae596f06d72b15598f64d02a9f2b90ae28f0de`

```dockerfile
```

-	Layers:
	-	`sha256:0493e10d70e37026d1fd54e30691d30a547959d3a3c743cd13a962b36551c5c7`  
		Last Modified: Thu, 02 Nov 2023 04:26:21 GMT  
		Size: 2.2 MB (2230397 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d04609d90a82986c7585e1e0d0a7ed624de678ce4fc614efdbbadb9497db8e1b`  
		Last Modified: Thu, 02 Nov 2023 04:26:21 GMT  
		Size: 16.8 KB (16786 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:1e58530b32c0a34d41ebb4e59128f1c50a35279f4e98899115e4f4f1545dd219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191235644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6730663ce0d2a2f8ae7878946fa6022efb89fb6519e95aa06f992d113cb966a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
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
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:228fba57ed7938c60bc9d9d3f08c45e1d4596781feaac9bf351b0e87a0a0b122`  
		Last Modified: Wed, 01 Nov 2023 02:08:22 GMT  
		Size: 2.3 MB (2328545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39f0273d831e72fd3bbc4d781be75a66c134f178292be9d51a47b029c9bdab70`  
		Last Modified: Wed, 01 Nov 2023 02:08:29 GMT  
		Size: 156.5 MB (156504036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2068c27ada325ab869c1f24a9e8fad5992483c9b7ebc1216011c50cdf60c4a6a`  
		Last Modified: Wed, 01 Nov 2023 02:08:22 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:5eedfa3c5a2ab2306766c85184557dac0c47973bf4e71f26dea531d1b580dd4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 KB (16704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d0f49e264a2382de8087efe02da6aafc347a090963e1779a416f63fac1e325`

```dockerfile
```

-	Layers:
	-	`sha256:3a49190f4d41ba7942c7337870de87b025f7713989e3b46e74e395927548002c`  
		Last Modified: Wed, 01 Nov 2023 02:08:22 GMT  
		Size: 16.7 KB (16704 bytes)  
		MIME: application/vnd.in-toto+json
