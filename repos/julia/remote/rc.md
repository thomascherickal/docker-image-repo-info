## `julia:rc`

```console
$ docker pull julia@sha256:338e0d08ff32e7e63208588524cbbad1cbbe322cfcd25e8baa6a88ac9eb8ace0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

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

### `julia:rc` - windows version 10.0.20348.1487; amd64

```console
$ docker pull julia@sha256:a114768836a56347ec62444e0f46b356bb18631fd8f8f05f453a56f6cb0a8e1c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1546869777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f41148c7c4add6734f3b964622cd1df807eb08408a6b561a72cd36271225dad5`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 10 Feb 2023 02:19:24 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 02:19:25 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-beta4-win64.exe
# Fri, 10 Feb 2023 02:19:26 GMT
ENV JULIA_SHA256=c298228ad482b9941f496b88cffa4d7db516be7bae576e9d83a2bff435435ba5
# Fri, 10 Feb 2023 02:21:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 10 Feb 2023 02:21:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a49a63d08a7e38a0b02595dbb45cdb00993fc8282c5e698fa6471cbeea813`  
		Last Modified: Fri, 10 Feb 2023 02:24:54 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4e794dcfc47ebe1fd147ac84cce206785e1f453bc09e5508979a8b22633533`  
		Last Modified: Fri, 10 Feb 2023 02:24:54 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c8b51d1e52df1d5c6283d2000b824e38cd9338c3054788c3671b5dde817ca2`  
		Last Modified: Fri, 10 Feb 2023 02:24:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f637bed8f5eb6de6b430fa7fe288ad5b614c746d2f6916d83eb24f0dc358a88`  
		Last Modified: Fri, 10 Feb 2023 02:25:40 GMT  
		Size: 160.8 MB (160833616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4efa18bfa53ac6d1c7c2f50c78f9e8e3edc3288bad9b44057f3971d4f1a365e`  
		Last Modified: Fri, 10 Feb 2023 02:24:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.3887; amd64

```console
$ docker pull julia@sha256:c84b01774711e9a5391f4ae71c8db173c78dbd9107b42b29d044cd1d1190716f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1868570307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ae443099acc375a96b181a481893032b29fc0258c89e6f1a0cb3595dad9132`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 10 Feb 2023 02:21:26 GMT
ENV JULIA_VERSION=1.9.0-beta4
# Fri, 10 Feb 2023 02:21:27 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-beta4-win64.exe
# Fri, 10 Feb 2023 02:21:28 GMT
ENV JULIA_SHA256=c298228ad482b9941f496b88cffa4d7db516be7bae576e9d83a2bff435435ba5
# Fri, 10 Feb 2023 02:23:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Fri, 10 Feb 2023 02:23:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3116bd525a636fedba84e02e718621517d114cd385bb1252b651d9e826da07`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6239861d345b139582cd738362767489805b29eee49b573e1227038ffefbd1`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c7f6fe23fe1de7c3b898f3eb0497ea320133a9a65d11124878b65f8a50f35d`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ea8096cc5ce02c3797823496b6dadb8a89a115d2b9ab1e3d3e72ded0337c40`  
		Last Modified: Fri, 10 Feb 2023 02:26:31 GMT  
		Size: 160.6 MB (160619208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db011c318070090abfe67511ebbb77a5785c5d5ae1c358bb6ab0eb99c8d3dc`  
		Last Modified: Fri, 10 Feb 2023 02:25:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
