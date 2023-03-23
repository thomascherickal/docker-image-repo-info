## `julia:rc`

```console
$ docker pull julia@sha256:b522beb5ce2a01bdd56aa48eb98a485398533dc55adcbb96147397d14981330a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1607; amd64
	-	windows version 10.0.17763.4131; amd64

### `julia:rc` - linux; amd64

```console
$ docker pull julia@sha256:255e55b830e2907d3d91ed190edeb9da7d08d22c161e1042b29052e19470ef73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182169951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8cc7a0ac15c1c160053a8b795ea885dea44e8157befcd007c8afd6d0ce03d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:15:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:15:02 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Mar 2023 09:15:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:15:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Mar 2023 09:15:02 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 23 Mar 2023 09:15:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc1-linux-x86_64.tar.gz'; 			sha256='357ddb46518a2ded6d867f930f088238dcdc580c53b3c627b9011650200294ee'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc1-linux-aarch64.tar.gz'; 			sha256='8637f7facae9f8d5975a6f09f50104d4f34be3ee425324e2e4d7375410cf7e13'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc1-linux-i686.tar.gz'; 			sha256='f726767f995aab05f241a9312bbc1a84922fbc81a9ad8647bebefe2154b6bf5e'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc1-linux-ppc64le.tar.gz'; 			sha256='71c6e4987c4a62d1c728ece21bc68572f49a533cc80276afa2f193916b0c7994'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Mar 2023 09:15:20 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 23 Mar 2023 09:15:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:15:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d11f2d375f52c4aff365d0de067316ab1272f9210de405fdb00b70e639ba1`  
		Last Modified: Thu, 23 Mar 2023 09:17:43 GMT  
		Size: 2.4 MB (2426599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cb4a96311ac138d97ca96c361b2ce60ca1eca74bce8cc94450e184ea4a577c`  
		Last Modified: Thu, 23 Mar 2023 09:18:04 GMT  
		Size: 148.3 MB (148331573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89fb0dfdcb35bee96a38d0b0fb422b2942bdc6c5316abc1777c7987881b8dd`  
		Last Modified: Thu, 23 Mar 2023 09:17:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:70889788de8b862ac68b46459ad26860208f3c0acd8c2e886ac223418d1238b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.0 MB (174973319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f3c9714d701198c8fe3d78ea618d809078efcb0007f67250cc957d474b15be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:13:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Mar 2023 09:13:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:13:22 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Mar 2023 09:13:22 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 23 Mar 2023 09:13:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc1-linux-x86_64.tar.gz'; 			sha256='357ddb46518a2ded6d867f930f088238dcdc580c53b3c627b9011650200294ee'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc1-linux-aarch64.tar.gz'; 			sha256='8637f7facae9f8d5975a6f09f50104d4f34be3ee425324e2e4d7375410cf7e13'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc1-linux-i686.tar.gz'; 			sha256='f726767f995aab05f241a9312bbc1a84922fbc81a9ad8647bebefe2154b6bf5e'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc1-linux-ppc64le.tar.gz'; 			sha256='71c6e4987c4a62d1c728ece21bc68572f49a533cc80276afa2f193916b0c7994'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Mar 2023 09:13:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 23 Mar 2023 09:13:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:13:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dae24c4ed3424e55959d0c4023f7917665d7dfade75d67d25064d114029099`  
		Last Modified: Thu, 23 Mar 2023 09:15:49 GMT  
		Size: 2.4 MB (2414202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558b776a3d6a0091f12b78cb487e5b15c4f48c5840afd1e26a996fae8c14918a`  
		Last Modified: Thu, 23 Mar 2023 09:16:05 GMT  
		Size: 142.5 MB (142496041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e3902c50300a78ea28b10f0378094f7494a45c62254f589eb603a322c3eda9`  
		Last Modified: Thu, 23 Mar 2023 09:15:49 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; 386

```console
$ docker pull julia@sha256:0734e4de802711f437e27992433b0f262fbeb72230404a64cdc8fb2c4c0ca933
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.5 MB (180531991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f457c79081f518ccb7a8b4cc40be8d2b196a9f888ed603253b69905c2a778ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:57:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:57:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Mar 2023 13:57:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 13:57:08 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Mar 2023 13:57:08 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 23 Mar 2023 13:57:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc1-linux-x86_64.tar.gz'; 			sha256='357ddb46518a2ded6d867f930f088238dcdc580c53b3c627b9011650200294ee'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc1-linux-aarch64.tar.gz'; 			sha256='8637f7facae9f8d5975a6f09f50104d4f34be3ee425324e2e4d7375410cf7e13'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc1-linux-i686.tar.gz'; 			sha256='f726767f995aab05f241a9312bbc1a84922fbc81a9ad8647bebefe2154b6bf5e'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc1-linux-ppc64le.tar.gz'; 			sha256='71c6e4987c4a62d1c728ece21bc68572f49a533cc80276afa2f193916b0c7994'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Mar 2023 13:57:33 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:57:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 13:57:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2805ff5d8a1ec712f796a611f4adb5ac76815f4d61126cb80847e81481d33a34`  
		Last Modified: Thu, 23 Mar 2023 14:00:15 GMT  
		Size: 2.5 MB (2532328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f2c64cc09354c66f2a5ac807ff5e36e4ee1035187355fb3ca54f06bd412139`  
		Last Modified: Thu, 23 Mar 2023 14:00:44 GMT  
		Size: 145.6 MB (145603014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e0f0a5faf3ddb67c18320ecbdd7479e98ff45fbfc5d36ea028a638e8da1a8d`  
		Last Modified: Thu, 23 Mar 2023 14:00:14 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; ppc64le

```console
$ docker pull julia@sha256:7544d518edab151c38062b120e3237118422d80cfcbbf8ea35c55dbd60723f3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.7 MB (170727542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ac23afc89675fdafd8d658702ef989008a7025a921d37df7ed023f08c64a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:42:52 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 23 Mar 2023 09:42:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:42:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 23 Mar 2023 09:42:53 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 23 Mar 2023 09:43:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-rc1-linux-x86_64.tar.gz'; 			sha256='357ddb46518a2ded6d867f930f088238dcdc580c53b3c627b9011650200294ee'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-rc1-linux-aarch64.tar.gz'; 			sha256='8637f7facae9f8d5975a6f09f50104d4f34be3ee425324e2e4d7375410cf7e13'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-rc1-linux-i686.tar.gz'; 			sha256='f726767f995aab05f241a9312bbc1a84922fbc81a9ad8647bebefe2154b6bf5e'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-rc1-linux-ppc64le.tar.gz'; 			sha256='71c6e4987c4a62d1c728ece21bc68572f49a533cc80276afa2f193916b0c7994'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 23 Mar 2023 09:43:39 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 23 Mar 2023 09:43:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:43:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cb7ea675c84c4da69169d3af4a61542b472f69e1ff5bffe7ab367ec7811793`  
		Last Modified: Thu, 23 Mar 2023 09:44:51 GMT  
		Size: 2.6 MB (2627351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df674fb5e7ae386a255a31955d5906e9ca09426017c548390a70cb06a4f1c2c`  
		Last Modified: Thu, 23 Mar 2023 09:45:26 GMT  
		Size: 132.8 MB (132811767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d2ca93f681d9fc8074b0e7d32d038a6408a7b9f1e62423195517bea28d7642`  
		Last Modified: Thu, 23 Mar 2023 09:44:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.20348.1607; amd64

```console
$ docker pull julia@sha256:288d74cd17704ed3b346367515657ff32fd5d97f49359704eca994eadef4b481
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875474172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e9ec49f069de38df5bff185d7703f996474fee5aaacee04bcda7be383e8c97`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 07:17:58 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 16 Mar 2023 07:17:59 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-rc1-win64.exe
# Thu, 16 Mar 2023 07:18:00 GMT
ENV JULIA_SHA256=8bcb9ac062b86407c16f21052c05cc4a414a2623e708ccf4c41394857c849063
# Thu, 16 Mar 2023 07:19:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 16 Mar 2023 07:19:47 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67daee0f13e6333b8b5b67f371bf6093e3abb1849a56687bc035808355cce75`  
		Last Modified: Thu, 16 Mar 2023 07:35:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abf109fc0cd05d1b49903d175a52b06446e945a00b9d9013ec4b81352cff359`  
		Last Modified: Thu, 16 Mar 2023 07:35:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7f5351c49fb41584daebb08449283d2c4822d473cfa484e79f74af8a3f6c00`  
		Last Modified: Thu, 16 Mar 2023 07:35:00 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf502eaf6c6536a1a04bc772ddd09e62cc7952b46c5e968fabe5a67a2893ee4`  
		Last Modified: Thu, 16 Mar 2023 07:35:43 GMT  
		Size: 161.5 MB (161527035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022cfad4d7d74a3fcbbdeaf66cd313314851186ab45b8cbb0368ae1fa046bdb3`  
		Last Modified: Thu, 16 Mar 2023 07:35:00 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.4131; amd64

```console
$ docker pull julia@sha256:00fffb28e1000e8935ac615023c771cd1674cae417dd47a021522571a4ea9066
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2174800441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f0b03004e64ba01edce93f6a13ac78a54b9e7fc957a40599eadd9c5665b320`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 07:20:06 GMT
ENV JULIA_VERSION=1.9.0-rc1
# Thu, 16 Mar 2023 07:20:07 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-rc1-win64.exe
# Thu, 16 Mar 2023 07:20:08 GMT
ENV JULIA_SHA256=8bcb9ac062b86407c16f21052c05cc4a414a2623e708ccf4c41394857c849063
# Thu, 16 Mar 2023 07:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Thu, 16 Mar 2023 07:23:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a82d12251bcae9056bf6a6f14747ada9fcdf40428483e075e9be108ca5fd2f9`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf31eddd4d173e07844fb9f65e557a1007a73ff38547e8a04c8d9fae0f1075f9`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac9b4231675af55156ec7e72b036fde2dd179c361952d3dcea9238f06245dfb`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e799e4d617c85ef3c77f7ace87d13cdf6bd3e3ef134669c4e48f86d3e3f82c`  
		Last Modified: Thu, 16 Mar 2023 07:36:37 GMT  
		Size: 161.3 MB (161284359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a667a31e1e4ce2707e0421cb3b81fa9175d73e48b4af1850251cb79b867ffab4`  
		Last Modified: Thu, 16 Mar 2023 07:35:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
