## `julia:rc`

```console
$ docker pull julia@sha256:a0a63ad413da87017712812c004b99cf229b0331a2c809f144067ef62ff2b732
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `julia:rc` - linux; amd64

```console
$ docker pull julia@sha256:b37e2f406c661a38307f33406896fbe293fe36fe330e5134848fad54793836ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182090992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cd5230b1ec8080fa670b6ce81a57e93eaa5f495741d378ba4ed5f0b0c2647a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:13:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:13:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 07:13:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 07:13:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 18:31:15 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 18:31:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 18:31:36 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:31:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:31:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7139d3ae92ad41af38fdee8794327adf0811f25a5a629e20792a4b0bb8ca11c4`  
		Last Modified: Thu, 09 Feb 2023 07:16:31 GMT  
		Size: 2.4 MB (2426546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5082f1e1e311e8b015255a88f93d0aa84af586d6c6d74f266f20d75446b9a0ed`  
		Last Modified: Fri, 10 Feb 2023 18:34:12 GMT  
		Size: 148.3 MB (148252258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cd76b9642b0acdd8f4f90620e46487996bc6ac532912e23c3f561f94883c7e`  
		Last Modified: Fri, 10 Feb 2023 18:33:48 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:574ec3a53dcc38182d075a3c3c05692a230018f0ff3d3e203e53780a92147f42
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174580406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92d35f1e36df8e2eea0cdc3acc71dd9ae22aaf879570bdd9fb53b4b0a431e59c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:40:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 13:40:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 13:40:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 01:53:43 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 01:54:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 01:54:12 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:54:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3befbc1072899da37ba03cc74c4f850ac9c608aaf7fd9945b690181250505123`  
		Last Modified: Thu, 09 Feb 2023 13:43:09 GMT  
		Size: 2.4 MB (2414195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d69f3e89e543cc34ba93012f542f57fafe16858c0c7ca151a8a55312f6891d`  
		Last Modified: Fri, 10 Feb 2023 01:55:33 GMT  
		Size: 142.1 MB (142103326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5126e2dc2a7e068345a63158cff28a94a72c3354782d7beaa9a4d12bcf8bbd`  
		Last Modified: Fri, 10 Feb 2023 01:55:15 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; 386

```console
$ docker pull julia@sha256:0c8b15ba1e938494820a729e9b2281867a229b3794192aa60aba4c3fda74868a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.1 MB (180144598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6feddc7d281635cbed61e7426c87735ef9ae45fa64c4c4a67cde6e7b6399a8f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:29:00 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 12:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 12:29:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 01:40:30 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 01:40:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 01:40:57 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be442f0f4ba505349cfe9c32e43ccce6c6d5fe4681dd52f3116fa76df6b79d33`  
		Last Modified: Thu, 09 Feb 2023 12:33:03 GMT  
		Size: 2.3 MB (2326815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd03e724e7a1fafff539a91868920834154209f3d9cdf833252014f55e7db770`  
		Last Modified: Fri, 10 Feb 2023 01:43:05 GMT  
		Size: 145.4 MB (145420530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d00fb72a8c3c2545dff21bcc845c310dcc9e0f57606e4c902d9a962209811`  
		Last Modified: Fri, 10 Feb 2023 01:42:45 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; ppc64le

```console
$ docker pull julia@sha256:acd84621c7390ed122e115dc908f6cd0ccdfbad0d751c96dbaa057755e8e3dba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169347530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0aa427d3f99542ac0f3fb413ebd5d700fea17df940a56c6ab81ba98712c2cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:59:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 09 Feb 2023 12:59:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 12:59:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 10 Feb 2023 03:32:08 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 03:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-beta4-linux-x86_64.tar.gz'; 			sha256='ce40a62760c854008afbc476a5851386b43556e09609d655fa8ae453beb588c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-beta4-linux-aarch64.tar.gz'; 			sha256='284ba730f5cbf24383aa09a7d8196eb9efbe03ae25af84244b1880b7d92c0be9'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-beta4-linux-i686.tar.gz'; 			sha256='58f8890212e429c9c47ae39e5c51fa4dab24deb5f5d8bc4c2b89c0f005a71549'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-beta4-linux-ppc64le.tar.gz'; 			sha256='40dacbbeb851845d2e8ef5cd15d584e6ffd0c199546ca9f71fe9266213244c72'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 10 Feb 2023 03:33:01 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 10 Feb 2023 03:33:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 03:33:02 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dcbe2f622b59de794cef13dd77a3dfa15ec928758d438ca961cbbee86c9097`  
		Last Modified: Thu, 09 Feb 2023 13:02:30 GMT  
		Size: 2.6 MB (2627282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c87b42d488e0268a86638c989ea3d1590f11693475e7ad1034ad44846defa`  
		Last Modified: Fri, 10 Feb 2023 03:34:18 GMT  
		Size: 131.4 MB (131430618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8a8b7074d56ce74557d77b1b73c074fc2ce57a680e96d0f68814012f084d4`  
		Last Modified: Fri, 10 Feb 2023 03:33:41 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.20348.1547; amd64

```console
$ docker pull julia@sha256:389013e85b083043639880ae549a4810fafeacd9683ebc9ca63c99ce78198418
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1840331663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0059e7307b0a386f9d14aa57e04f5c387ed0651651ac064766170e57de7bd63`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 05:05:05 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Thu, 16 Feb 2023 05:05:06 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-beta4-win64.exe
# Thu, 16 Feb 2023 05:05:07 GMT
ENV JULIA_SHA256=c298228ad482b9941f496b88cffa4d7db516be7bae576e9d83a2bff435435ba5
# Thu, 16 Feb 2023 05:07:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:07:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1288b34d1f2768852a5d3130c058aea65d028c00a6e18bfe54bfdd04d0bfab39`  
		Last Modified: Thu, 16 Feb 2023 05:22:59 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ca136d8c3fa8927c68065772c9f69534f195d766898717c831687f98e8af1e`  
		Last Modified: Thu, 16 Feb 2023 05:23:00 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cf2259a3b12c93c72ec0990c05387ecc96a99e012250026949b4085fe89b83`  
		Last Modified: Thu, 16 Feb 2023 05:22:59 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16544ee4e1e92a098e5872bba261073c6729f7c77e0257e81fd42f5556253a56`  
		Last Modified: Thu, 16 Feb 2023 05:23:42 GMT  
		Size: 161.0 MB (160978548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfaa904d0b14e5533ff3e40f07a4629803535def6322291861e5e2de3bd3660`  
		Last Modified: Thu, 16 Feb 2023 05:22:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.4010; amd64

```console
$ docker pull julia@sha256:fe8f37020ffee8825e98a65011d58706225c6bbbfea42abc82ee140d67f572f8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123700158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c97d0ee8d90341a511cd52be826fc35ca4f7ff80a10a741f959e7bc2ccee36`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 05:07:21 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Thu, 16 Feb 2023 05:07:23 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-beta4-win64.exe
# Thu, 16 Feb 2023 05:07:24 GMT
ENV JULIA_SHA256=c298228ad482b9941f496b88cffa4d7db516be7bae576e9d83a2bff435435ba5
# Thu, 16 Feb 2023 05:10:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:10:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef91ea2e383675be9aa1e58d446ce7d00a0bf7f7d2270674bfc401a1ac70812`  
		Last Modified: Thu, 16 Feb 2023 05:23:53 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a237e1f45e64852113d607ce7e58f94c1d3312699ea488fef374f9f6c6f7058`  
		Last Modified: Thu, 16 Feb 2023 05:23:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a9528c0423be5a8026968d5949fee41f20ebd4ff4730bba3fa4eebc49e24d3`  
		Last Modified: Thu, 16 Feb 2023 05:23:53 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a77afc3e3a1a3daa4a29e4879fa46c0f6840781e64ac802da1b9a614c5d97`  
		Last Modified: Thu, 16 Feb 2023 05:24:36 GMT  
		Size: 160.7 MB (160735361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f7150e58f3a4a4da3159201e1fb2707b701fd1fd4354f3edee76214e0519a3`  
		Last Modified: Thu, 16 Feb 2023 05:23:53 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
