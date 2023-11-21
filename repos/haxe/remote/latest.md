## `haxe:latest`

```console
$ docker pull haxe@sha256:b7cb8bc5cb70eac7330437d0c9a3019d032acbbbceccaf8ee0872dec3120089e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.2113; amd64
	-	windows version 10.0.17763.5122; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:337e9c62569f69a7d39f643169156dd0c64b59a032667240d8cbf5c3832708c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140053509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb54794ebf682032aeab4490eed944d6171931d2c07d3e23744691b2237789ff`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 16:56:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 16:56:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 16:56:41 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 01 Nov 2023 16:57:55 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 21 Nov 2023 05:31:49 GMT
ENV HAXE_VERSION=4.3.3
# Tue, 21 Nov 2023 05:31:49 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 21 Nov 2023 05:34:59 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 21 Nov 2023 05:34:59 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edec3b277570c5b017f9ea002a0f618f7ff48c93b70156f1bde3336e27f9c096`  
		Last Modified: Wed, 01 Nov 2023 17:38:35 GMT  
		Size: 1.4 MB (1370276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf5ea448c1f54d9a8c2e95a520f6a689edda515acdd2e25dd6a87ac4256bea3`  
		Last Modified: Wed, 01 Nov 2023 17:38:35 GMT  
		Size: 1.4 MB (1449001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666cddbc70da3c0018cd71fb611ac8e8f7747a70ef48a6df6bb3e5cc9e0eb48d`  
		Last Modified: Tue, 21 Nov 2023 06:01:52 GMT  
		Size: 11.8 MB (11816349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:e44004a142fc4960c0308ce5ca3d32566e6020b024b97e447dd11042d83f8e23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129494162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7eba65b4646bd8f6bb836ceea5a7e19ad23e22d73be5b15b3a320e2cf181298`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:32:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 16:08:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 16:08:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 16:08:57 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 01 Nov 2023 16:10:21 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 21 Nov 2023 04:07:52 GMT
ENV HAXE_VERSION=4.3.3
# Tue, 21 Nov 2023 04:07:52 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 21 Nov 2023 04:11:12 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 21 Nov 2023 04:11:12 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b9dc19e6fd54f3a85453a84bc99da2ca6e508d91ce084872e33c6c60d774c`  
		Last Modified: Wed, 01 Nov 2023 02:43:18 GMT  
		Size: 50.4 MB (50353285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611268e24a228de2f9ab9fb56c44fced4eff688c78dc392bc6390b5118bb331c`  
		Last Modified: Wed, 01 Nov 2023 16:49:24 GMT  
		Size: 1.3 MB (1283260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f326ee6c88423ac5be7d90b39acf564ec32021a298b5a0adec922b8dd1fb473a`  
		Last Modified: Wed, 01 Nov 2023 16:49:24 GMT  
		Size: 1.4 MB (1389863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16861575dc7336925c7189619817836db35420b3b9d9cdfc9cf18b60287dfffc`  
		Last Modified: Tue, 21 Nov 2023 04:17:06 GMT  
		Size: 11.4 MB (11372681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:2ff523dc7bcf7cda62e83aa715ff2176845707c89b0e1b9019693757bd9310f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140437920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb8cc945ad2a6e22c30cd41f59f80ae6d6e2b6f8e8b7dfc8060f941665dcf35f`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:56:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 14:56:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 14:56:24 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 01 Nov 2023 14:57:38 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 21 Nov 2023 03:40:59 GMT
ENV HAXE_VERSION=4.3.3
# Tue, 21 Nov 2023 03:40:59 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 21 Nov 2023 03:43:57 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 21 Nov 2023 03:43:57 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e627bbf1475bea4dce35bb2c9ee58b6eb3be5573e4efe8bd5793ae6a1555118`  
		Last Modified: Wed, 01 Nov 2023 02:14:57 GMT  
		Size: 54.7 MB (54699568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc369846a28b5e43a662d551f25dee7a6016e63924a502323ad701d8b26726`  
		Last Modified: Wed, 01 Nov 2023 15:32:20 GMT  
		Size: 1.4 MB (1360722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52674589a4a6eeffc7cb00dd168728f1a9167e1217f4b8bd333ffebc259b355`  
		Last Modified: Wed, 01 Nov 2023 15:32:20 GMT  
		Size: 1.4 MB (1440536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ee5add4d35516f09bff771baa2c0da597e5a0ef3a687e09b0b0cd3b6895712`  
		Last Modified: Tue, 21 Nov 2023 04:05:29 GMT  
		Size: 13.5 MB (13479465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.2113; amd64

```console
$ docker pull haxe@sha256:47ade2ad189998b816cb1c85499df671e0bafb1cc4a4a30199a17e77978642d2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1913128905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f289a8f758db7ce1ad2f13cd92afc02b6f9d30c0dd81e29594d5400b2d74fe96`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 03:18:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:39:49 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Thu, 16 Nov 2023 05:39:50 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Thu, 16 Nov 2023 05:39:51 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Thu, 16 Nov 2023 05:39:52 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Thu, 16 Nov 2023 05:39:53 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Thu, 16 Nov 2023 05:40:14 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Nov 2023 05:41:20 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 05:41:41 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Thu, 16 Nov 2023 05:41:42 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 16 Nov 2023 05:42:17 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Tue, 21 Nov 2023 04:15:12 GMT
ENV HAXE_VERSION=4.3.3
# Tue, 21 Nov 2023 04:19:41 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.3.3/haxe-4.3.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (70953a966b90bceb664639d1a690567e39cf9e3ebacf8c622c17df76fa0a199b) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '70953a966b90bceb664639d1a690567e39cf9e3ebacf8c622c17df76fa0a199b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Tue, 21 Nov 2023 04:20:05 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Tue, 21 Nov 2023 04:20:06 GMT
ENV HOMEDRIVE=C:
# Tue, 21 Nov 2023 04:20:27 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 21 Nov 2023 04:21:33 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Tue, 21 Nov 2023 04:21:34 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a73dc3dec59ae25ff1232f5fdf2ab39df387f3bf86ba48717ff271d76c2feb`  
		Last Modified: Thu, 16 Nov 2023 04:19:26 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfcd55368a38484d2de1a90a30855aa5314351ae3bb0293211b33af2def4fbf`  
		Last Modified: Thu, 16 Nov 2023 07:36:25 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a882c5100700b01dbbca0202e499e72ca2c9ab5b42a6856196958689b3125eb6`  
		Last Modified: Thu, 16 Nov 2023 07:36:25 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e56c0af1fd9ffa19c9accad1656ed3680400b61e86ab3e74a2080314cebeaa`  
		Last Modified: Thu, 16 Nov 2023 07:36:25 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c354686de03e4bb676f400d5617c9b482e7ec34883217ef4fa39f8e2ec53ab`  
		Last Modified: Thu, 16 Nov 2023 07:36:23 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd2d432acda3088ac2b2c1348be20ef6495b4810e839f210c5641ff1146a1ad`  
		Last Modified: Thu, 16 Nov 2023 07:36:23 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b3dd1bb3dc188ce673d50ed60f484e4c81dbfe2f92664c99426ee9d43579fd`  
		Last Modified: Thu, 16 Nov 2023 07:36:23 GMT  
		Size: 446.4 KB (446449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e481474208df6d2f7fdd75f818e5c98d5e981599e048240bd61755805ac655e8`  
		Last Modified: Thu, 16 Nov 2023 07:36:24 GMT  
		Size: 12.8 MB (12844064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6f97bfc882f6fd2a6db8c7e14d2a78a6ec5d05e8ff73417d3b3826f77a902`  
		Last Modified: Thu, 16 Nov 2023 07:36:21 GMT  
		Size: 290.4 KB (290388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b4d22995960e4e74795d1d3571f619bc7f9acd3687019423fd848e776fa67a`  
		Last Modified: Thu, 16 Nov 2023 07:36:20 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aacf14cc4ff21704350d6128e36b5864a21498590cf98393b2b3c157a9a5f29`  
		Last Modified: Thu, 16 Nov 2023 07:36:21 GMT  
		Size: 2.1 MB (2119898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e2c9b8c9b449ad27af901e02445821ee538892e6bd422b8d9833a026f6a70`  
		Last Modified: Tue, 21 Nov 2023 04:33:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5814bfd193fee90835313844aef3f258224ac918cad72969100c30431c4ab90e`  
		Last Modified: Tue, 21 Nov 2023 04:33:14 GMT  
		Size: 9.6 MB (9594185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736029303321a4c418a5a731466af2f0393c9f5277696f1fe78a0282ad7683b4`  
		Last Modified: Tue, 21 Nov 2023 04:33:08 GMT  
		Size: 337.0 KB (336996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db268eede9c7ca7e438baf61777d6095287671304f08fe5e3928dc15f1b789aa`  
		Last Modified: Tue, 21 Nov 2023 04:33:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead5f9eb5483a1b12de1e12f17ae64c75eac4bcb8a4365d20527fa9c63d6de5f`  
		Last Modified: Tue, 21 Nov 2023 04:33:08 GMT  
		Size: 339.7 KB (339717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16c9205d61a894e6c3efb5907966125427bdd17ad1234e47f3996ed246c15c`  
		Last Modified: Tue, 21 Nov 2023 04:33:08 GMT  
		Size: 362.4 KB (362421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7d7f7c823ad903d1c53723da0ed02bacab0487466831ab20e550f6dc9fad9`  
		Last Modified: Tue, 21 Nov 2023 04:33:08 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.5122; amd64

```console
$ docker pull haxe@sha256:407862d5ac5b84ab524f6cd05e1e3068a88d658021ea7a3c7e08d47a4fe698c8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2083677902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe5b864b91d17d79754c7b632546452f829b0d8a4548dcb874deac6d10c28af`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 03:20:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Nov 2023 05:47:49 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Thu, 16 Nov 2023 05:47:50 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Thu, 16 Nov 2023 05:47:51 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Thu, 16 Nov 2023 05:47:52 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Thu, 16 Nov 2023 05:47:53 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Thu, 16 Nov 2023 05:49:02 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Nov 2023 05:51:03 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 05:52:13 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Thu, 16 Nov 2023 05:52:14 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 16 Nov 2023 05:53:59 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Tue, 21 Nov 2023 04:21:42 GMT
ENV HAXE_VERSION=4.3.3
# Tue, 21 Nov 2023 04:26:46 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.3.3/haxe-4.3.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (70953a966b90bceb664639d1a690567e39cf9e3ebacf8c622c17df76fa0a199b) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '70953a966b90bceb664639d1a690567e39cf9e3ebacf8c622c17df76fa0a199b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Tue, 21 Nov 2023 04:27:57 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Tue, 21 Nov 2023 04:27:58 GMT
ENV HOMEDRIVE=C:
# Tue, 21 Nov 2023 04:29:10 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 21 Nov 2023 04:30:27 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Tue, 21 Nov 2023 04:30:28 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e4111e1324ff2110def2382c3796071edd92a76a262efa6c0657d549b64496`  
		Last Modified: Thu, 16 Nov 2023 04:21:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9d10f9e0f90494272dd239c1daebb4bb542e8f6c7577eb1935f32c3f05754f`  
		Last Modified: Thu, 16 Nov 2023 07:36:44 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29721bdd71ffda78baa2c6ab72603b123d9ae69bd2d9784da6282001dde085d0`  
		Last Modified: Thu, 16 Nov 2023 07:36:44 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e596955e42375f64b3c5f2f546eb7f723ed64049bcada0ddfefb193fb869ad`  
		Last Modified: Thu, 16 Nov 2023 07:36:44 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d52aff758ccf00efa51fa8c830cba1eda65aecc200e2d3d540f1fac58ed612`  
		Last Modified: Thu, 16 Nov 2023 07:36:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee23f431b82211ed5d536021f9fc8ec76cfbb2961824846422490121e2f7b1`  
		Last Modified: Thu, 16 Nov 2023 07:36:42 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116db5fcad271ee788206dfe61c6d4f24a23a8ba30bc326e8183f7bddd0b180`  
		Last Modified: Thu, 16 Nov 2023 07:36:42 GMT  
		Size: 437.8 KB (437773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8231e4bdc6f7b3ad9cbc1f75d86e2ff0f96fa59dc5aaf593f801e556a3607b39`  
		Last Modified: Thu, 16 Nov 2023 07:36:44 GMT  
		Size: 12.9 MB (12881472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28070e45842fb9dcb9ac0b48a98a0710510f8c63724ca06401768ba38887f44`  
		Last Modified: Thu, 16 Nov 2023 07:36:40 GMT  
		Size: 283.4 KB (283400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba20379a0736d934cf0605e10a941488cf09f1fb975acab71dba223f564428c`  
		Last Modified: Thu, 16 Nov 2023 07:36:40 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46427b5c20f0ce5ca411b29b5bd77b30d1dacacf0e882ec7546c9d119759e5fc`  
		Last Modified: Thu, 16 Nov 2023 07:36:40 GMT  
		Size: 2.1 MB (2112877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff7b22c4c6e7d4adde0527da471ea33df6e6c7617c3b7dcb67728d7ca510b58`  
		Last Modified: Tue, 21 Nov 2023 04:33:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a5e198e20ff776c5dafd6b5ed6f3d500066dfecbacdf7df0cd12f7525f14c9`  
		Last Modified: Tue, 21 Nov 2023 04:33:30 GMT  
		Size: 9.5 MB (9503837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1905b23d665fb71f0292070a3e120eddaf224d6a21118c0d93053bdc3e308c9b`  
		Last Modified: Tue, 21 Nov 2023 04:33:24 GMT  
		Size: 333.4 KB (333374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bc7f66c338e4ecf54eb5e60adb12ebdc38f01894737a613048757b8b1701b2`  
		Last Modified: Tue, 21 Nov 2023 04:33:24 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e003778cb4b5f187e7ad3d4721743fc9adfd7b900e794cac08e000db7e5998c4`  
		Last Modified: Tue, 21 Nov 2023 04:33:24 GMT  
		Size: 334.8 KB (334754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d8c17eb62c007d59bffde13bbf8970ecf5213053e23eaa6c39eb2edaa39c75`  
		Last Modified: Tue, 21 Nov 2023 04:33:24 GMT  
		Size: 344.9 KB (344929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f42e16cb6e7e712939f0bf135bd83a27e3c0cb6625d40947cf0ca538f47b0d2`  
		Last Modified: Tue, 21 Nov 2023 04:33:24 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
