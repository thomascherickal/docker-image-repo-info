## `julia:buster`

```console
$ docker pull julia@sha256:82291a0c3038efb828e0c68e46435c005b6f4e084ae94dc051ff11bd03689c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:bc7b2de50f45a52ee81d8134c7ccb1d8489e2de90d2b9780e6566844d0896808
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.5 MB (180539134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5932c10cb605fab6d27b692b463641566772e309a3f84130756f927aff83e3dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 09 Jun 2023 06:31:01 GMT
ENV JULIA_VERSION=1.9.1
# Fri, 09 Jun 2023 06:31:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 09 Jun 2023 06:31:23 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Fri, 09 Jun 2023 06:31:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jun 2023 06:31:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b77d6de018a508622b570cd459ca3f8acdcb52dc63a0da69ce8c01a1fadee3`  
		Last Modified: Fri, 09 Jun 2023 06:33:27 GMT  
		Size: 148.9 MB (148928066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc64f31da26123c792af82fdf102092bfccc4589cf76a933450b18bfabc62bb4`  
		Last Modified: Fri, 09 Jun 2023 06:33:05 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e2c3f0f0476bba81a74049cb24fc82da729302a6ed576bd04db60ae7638ce009
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173368357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e74a79438d14aed75583bf1d5c212e5d0df21c95f9e76e6efd96e8cf9bc943`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:38:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:38:10 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 13 Jun 2023 05:38:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 05:38:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 13 Jun 2023 05:38:10 GMT
ENV JULIA_VERSION=1.9.1
# Tue, 13 Jun 2023 05:38:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 13 Jun 2023 05:38:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 13 Jun 2023 05:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 05:38:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9ded89591b3bcf8dc3f78882f12fde29f13535ae313d53c190bbcf4d9630e9`  
		Last Modified: Tue, 13 Jun 2023 05:39:51 GMT  
		Size: 4.3 MB (4349150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f2be50a289a7e14e6cd365b149934d1cb7e6fb56d98c716eef017bdc0c7ae`  
		Last Modified: Tue, 13 Jun 2023 05:40:07 GMT  
		Size: 143.1 MB (143097480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd00344a3285d60213915be39ceacfb4ff8ba841aebfc4ef263456da357f9c85`  
		Last Modified: Tue, 13 Jun 2023 05:39:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:2f626ad8dcda7c80fbb4223cdf07e98f45daa72c91d5bf60c5809fe8458af580
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.4 MB (178403825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fabf859a52e0d5ca7e794544dea48ca6e3d0abe5f89e159f9a23c398ae20252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:35 GMT
ADD file:89de6b7378fdf61514133b7bd1ed23bb24397ce045566a30fee2a1347bf6587f in / 
# Mon, 12 Jun 2023 23:40:36 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:28:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 13 Jun 2023 04:28:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:28:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 13 Jun 2023 04:28:59 GMT
ENV JULIA_VERSION=1.9.1
# Tue, 13 Jun 2023 04:29:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.1-linux-x86_64.tar.gz'; 			sha256='cde14a58f899251f30cfced87055626f44845780659ebe8d50cbc4c67b31997c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.1-linux-aarch64.tar.gz'; 			sha256='b643ccd3e2a5960f7ce7055243743d0a39badda3974bce3d77861dd363badd10'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.1-linux-i686.tar.gz'; 			sha256='662111251fe82fca5a23321cbe218d98c23683e76dc32e1a9756aa436de97890'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.1-linux-ppc64le.tar.gz'; 			sha256='391aba8e239bfa29c1d96e2d81d6ec50ab5b924ac2132ef934c556e0a3329fc5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 13 Jun 2023 04:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e3832d1e9e7d28b937b10dcb945a700a76b4e3e7cde251e8eff22782e1fa2a55`  
		Last Modified: Mon, 12 Jun 2023 23:47:50 GMT  
		Size: 27.8 MB (27797003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff80462f12db7312824188e68b8f63256d6525f483c22d4e7a3df43fbe91910`  
		Last Modified: Tue, 13 Jun 2023 04:31:21 GMT  
		Size: 4.6 MB (4622145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adc11f1affd836f879c5a71e8a3bbad227d758d4af8f697ef1e11853c067dc1`  
		Last Modified: Tue, 13 Jun 2023 04:31:50 GMT  
		Size: 146.0 MB (145984305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62203358dae2b7d29a829a9d110c5f12a2203e4ac66778df9a1fc5633544c40b`  
		Last Modified: Tue, 13 Jun 2023 04:31:20 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
