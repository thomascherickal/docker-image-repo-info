## `haxe:latest`

```console
$ docker pull haxe@sha256:df67e73cbb7de6023df6063b618658c7453ec666e204940d08d246504ccc9c2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:a84f9d6c315f151dba10b98ba814bc49740de2c36d43ee3076f462b0aa443d1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140033197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8a84fb6d89e9f37d1f65151d0113b256cfe6546e84f7abde9396d509b6fba2`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:22:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:56:13 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 04:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 04:56:19 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 21 Sep 2023 04:57:57 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 21 Sep 2023 04:57:57 GMT
ENV HAXE_VERSION=4.3.2
# Thu, 21 Sep 2023 04:57:57 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 21 Sep 2023 05:00:57 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.2 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 21 Sep 2023 05:00:58 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1459d3ab8b5e46ac1a0a00134fe2f7b693474eb6d75ace97ecbe811a6f5b0e`  
		Last Modified: Wed, 20 Sep 2023 09:31:06 GMT  
		Size: 15.8 MB (15760408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab00e7798a04602c3f6e2dc445a994d75e96c45533cd44701f58509982a8c5`  
		Last Modified: Wed, 20 Sep 2023 09:31:23 GMT  
		Size: 54.6 MB (54584790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1539da90d520715d758e75854c9b0d351a6a7371ebc5102eb5ca59e07e48c320`  
		Last Modified: Thu, 21 Sep 2023 05:39:04 GMT  
		Size: 1.4 MB (1368847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45500c9a6f9e5462d4028cb4ea2d21d89c11ff6d86afe82ef766861d75bbf95f`  
		Last Modified: Thu, 21 Sep 2023 05:39:04 GMT  
		Size: 1.4 MB (1447561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b6f91cc0ae1c35a44b26d8fedbb735a683c9b937d27334583b96109a18757`  
		Last Modified: Thu, 21 Sep 2023 05:39:06 GMT  
		Size: 11.8 MB (11814877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:6ea09f5d5a14c2ab0cab61370bc63c05d36be1099eb28cf0679484f897ef2b10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129485160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:243f0c3d1021fecd466db5dddc2201317a7305f26fc84e475559014f6fe968f1`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:26:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 05:44:07 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Sep 2023 05:44:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 05:44:12 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 21 Sep 2023 05:45:38 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 21 Sep 2023 05:45:38 GMT
ENV HAXE_VERSION=4.3.2
# Thu, 21 Sep 2023 05:45:39 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 21 Sep 2023 05:48:12 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.2 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 21 Sep 2023 05:48:12 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbd770246538a809113f7f8fd84fedf3bd2bee5ed2f4fad2ab81cca9a78580d`  
		Last Modified: Wed, 20 Sep 2023 15:36:25 GMT  
		Size: 14.9 MB (14868646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145367a45c553b855c9dec20850966d6ec435636dba00c32133a9181c6f0b3e9`  
		Last Modified: Wed, 20 Sep 2023 15:36:43 GMT  
		Size: 50.4 MB (50355432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f92921f5f9ddffeb6d851c2c85ed9d720091b35830fd13e141fe2df41e21ae9`  
		Last Modified: Thu, 21 Sep 2023 06:22:18 GMT  
		Size: 1.3 MB (1281867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4332f8334e6e91dfd934dd97bd84caabfd5582f074f23a29b0054cb869c8b37f`  
		Last Modified: Thu, 21 Sep 2023 06:22:19 GMT  
		Size: 1.4 MB (1387859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2563ec3f03a402df3d877d8b2a2a2e70daaa49dbd1ecad24b28bc54ad6d2bb6`  
		Last Modified: Thu, 21 Sep 2023 06:22:20 GMT  
		Size: 11.4 MB (11371805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:52cb94dcafada22bdcad0aada5b7ef1c9afd05bc1c68a6ad228515bef0ace7b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140404740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9a78b73c69d06864e4f7688e2c7b35073f3518cbb0ce638fb66be44f9f62db`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:24:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:25:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:23:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 22:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre2-8-0 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:23:24 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 20 Sep 2023 22:24:33 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 20 Sep 2023 22:24:33 GMT
ENV HAXE_VERSION=4.3.2
# Wed, 20 Sep 2023 22:24:33 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 20 Sep 2023 22:27:28 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre2-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.3.2 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] || [ -f /usr/src/haxe/haxe.opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 20 Sep 2023 22:27:28 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60045eb75c62e890b95d28e4893132a6c7d61ec9979104ee4ff6e86c4badee`  
		Last Modified: Wed, 20 Sep 2023 09:33:11 GMT  
		Size: 15.7 MB (15746671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292737ab468ef80c6f78bdde4896157b8953d1e5556e1e526f40aeadcb547573`  
		Last Modified: Wed, 20 Sep 2023 09:33:26 GMT  
		Size: 54.7 MB (54676309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd73f62bf17ca55af4ef20eff5fbbb9c277e398b8114141587fd1df596f5d00`  
		Last Modified: Wed, 20 Sep 2023 22:59:23 GMT  
		Size: 1.4 MB (1359638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da82a6a021ec438cd4a5c320b4c56914e59b9d44120f181da9ee932e93f12938`  
		Last Modified: Wed, 20 Sep 2023 22:59:23 GMT  
		Size: 1.4 MB (1438444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106876ec41a024aaf335cbb67068cbdff0ceba2d050eb247c09d3658ca4abfc`  
		Last Modified: Wed, 20 Sep 2023 22:59:25 GMT  
		Size: 13.5 MB (13478786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.1970; amd64

```console
$ docker pull haxe@sha256:af75fec74a8933f43898867a8949d7a9db729910ab17161452c5214d0a4daff3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1863726909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84429290fa1cc41194463fee0a3b74fd14cdb15b986c333827db8200802fe564`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 03:53:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:39:44 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 13 Sep 2023 05:39:44 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 13 Sep 2023 05:39:45 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 13 Sep 2023 05:39:46 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 13 Sep 2023 05:39:47 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 13 Sep 2023 05:40:11 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 05:41:18 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 05:41:39 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 13 Sep 2023 05:41:40 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 13 Sep 2023 05:42:13 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 14 Sep 2023 20:15:10 GMT
ENV HAXE_VERSION=4.3.2
# Thu, 14 Sep 2023 20:18:55 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.3.2/haxe-4.3.2-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (194276aa37e19945e7d993145b2c9442777f8047e78038147a684d1fb7e8e9df) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '194276aa37e19945e7d993145b2c9442777f8047e78038147a684d1fb7e8e9df') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 14 Sep 2023 20:19:19 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 14 Sep 2023 20:19:20 GMT
ENV HOMEDRIVE=C:
# Thu, 14 Sep 2023 20:19:44 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Sep 2023 20:20:06 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Thu, 14 Sep 2023 20:20:07 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f19fc66ee381d7fb9811b24aea9ed1dff8ef483bc0e019d3c24c09fb8fbecd`  
		Last Modified: Wed, 13 Sep 2023 04:35:02 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e68dc0d4fb536cab5ccd2f2bf30c5c58094aa8f0535b4dffd3f8aaafa6d54`  
		Last Modified: Wed, 13 Sep 2023 07:26:42 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d0618bbce7b7450c2195dfddff338f62ad4c3330b7c600bf0de9ecc21a3f18`  
		Last Modified: Wed, 13 Sep 2023 07:26:42 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c281276f67c8a38c4febfc4b3214c98459f8b828bbc8975d26d1f59e9964ad`  
		Last Modified: Wed, 13 Sep 2023 07:26:41 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6301eeb49baa8079e594079a5c201c299f148642f01576284024aba3d0aaec`  
		Last Modified: Wed, 13 Sep 2023 07:26:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dfb6265cbf19f6c864dbd1cf0268b4c8d54ecbcf6b91b5a3066c37b66843f2`  
		Last Modified: Wed, 13 Sep 2023 07:26:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d324074f39cb4c389dbe1b32689e0064a0b301c2d3802ead0b3d52deaaa687`  
		Last Modified: Wed, 13 Sep 2023 07:26:40 GMT  
		Size: 464.8 KB (464797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5d632bd226b55e08bc01164c39f42bca951066e0fdc761d3689e5156c6f7e3`  
		Last Modified: Wed, 13 Sep 2023 07:26:41 GMT  
		Size: 12.9 MB (12862505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea96481b20c5c8412c2647cb6c286a2c0f54a83d9e27954e654303b9238676a`  
		Last Modified: Wed, 13 Sep 2023 07:26:38 GMT  
		Size: 309.0 KB (308967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16ce96f791a27af3447584ddb8834399f73231025845d2cb1dd40a0337bcb41`  
		Last Modified: Wed, 13 Sep 2023 07:26:37 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1ac2adb50278b627134898c9b0f3e6ab6301d53a707c698aa5ddcefdc95d90`  
		Last Modified: Wed, 13 Sep 2023 07:26:38 GMT  
		Size: 2.1 MB (2139238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58e7f2c9ebe6b022ad91dd4a07987a9720dd0f75832bdfa981a3a5b7293cfd0`  
		Last Modified: Thu, 14 Sep 2023 21:17:21 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c662516390a866832fce14666f66d3fcc9dd24d47f94766b18b12dcfd7f5018`  
		Last Modified: Thu, 14 Sep 2023 21:17:25 GMT  
		Size: 9.6 MB (9599540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e90b25550cba2d0a6ff2ce1dab500e47ef8d1040c5962813142a54523fe9ce4`  
		Last Modified: Thu, 14 Sep 2023 21:17:19 GMT  
		Size: 346.6 KB (346574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5cbdc8fc64875f4e37c0ab61f70c5ee977945d2e77fe12a70adfedf0934d1b`  
		Last Modified: Thu, 14 Sep 2023 21:17:19 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062f3b9a9ee818fdc72a4ebca8605249d5d04db6480c8a99204b2de077a9637c`  
		Last Modified: Thu, 14 Sep 2023 21:17:19 GMT  
		Size: 349.1 KB (349062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865fd60e27ec9ee2c8a8634e8a10b4c920dd4beed88c34a013c621cb3be6fa27`  
		Last Modified: Thu, 14 Sep 2023 21:17:19 GMT  
		Size: 368.3 KB (368288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff885d17bbd96c4b25b6c80501d7026d54b73949a52d1de253d8ea5a6390e3ae`  
		Last Modified: Thu, 14 Sep 2023 21:17:18 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull haxe@sha256:e55190c0116786fa63169b6981d8a3cb7e86c08af3d791054935dd431bdfbcae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2042270353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f720a77c6dd2db8bbaed2c86967fd7ae997334b3cdd6ee0ec14125cb41df50`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:47:15 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 13 Sep 2023 05:47:16 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 13 Sep 2023 05:47:17 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 13 Sep 2023 05:47:17 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 13 Sep 2023 05:47:18 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 13 Sep 2023 05:48:14 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Sep 2023 05:50:01 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 13 Sep 2023 05:51:02 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 13 Sep 2023 05:51:03 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 13 Sep 2023 05:52:16 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 14 Sep 2023 20:20:24 GMT
ENV HAXE_VERSION=4.3.2
# Thu, 14 Sep 2023 20:24:47 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.3.2/haxe-4.3.2-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (194276aa37e19945e7d993145b2c9442777f8047e78038147a684d1fb7e8e9df) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '194276aa37e19945e7d993145b2c9442777f8047e78038147a684d1fb7e8e9df') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 14 Sep 2023 20:25:51 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 14 Sep 2023 20:25:52 GMT
ENV HOMEDRIVE=C:
# Thu, 14 Sep 2023 20:26:54 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Sep 2023 20:28:00 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Thu, 14 Sep 2023 20:28:01 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f61a9edd2b78447d6f270891365486c8c865c3a29c349ec352156584abad5b`  
		Last Modified: Wed, 13 Sep 2023 07:26:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd46a28ef1f551c32741e4e58980c2c5122f75791b710b72f4b306ffa273640`  
		Last Modified: Wed, 13 Sep 2023 07:26:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b060d9505a764f0154df84e8d9748f3e37c7d68336f8a8e727a9a898d93bb`  
		Last Modified: Wed, 13 Sep 2023 07:26:59 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c52242973f4c75297c6a8e89d99d62ee7a3c673b2c867d2fcb4fd9bfa79d940`  
		Last Modified: Wed, 13 Sep 2023 07:26:57 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c22319df8c56ec1d94c50cc8453919322004bf84c0ed167e296d68c60a824a`  
		Last Modified: Wed, 13 Sep 2023 07:26:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16378c6604a530287c6441f220066b490748ad02a9f94c186923d9a1cfa00a1f`  
		Last Modified: Wed, 13 Sep 2023 07:26:57 GMT  
		Size: 295.7 KB (295725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8b8d657da54c84a77ce6a22daa12f9bc7395a5848b6be01bae4a1e25af667b`  
		Last Modified: Wed, 13 Sep 2023 07:26:58 GMT  
		Size: 13.0 MB (13026938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bf93db41358b84907cc3eddd074ac88aa9209381e54e49605af913720a8968`  
		Last Modified: Wed, 13 Sep 2023 07:26:55 GMT  
		Size: 210.6 KB (210593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407620b72a089f5d71f76e1560fc8b385846c355b85bb86d08a19d0644b2e72`  
		Last Modified: Wed, 13 Sep 2023 07:26:54 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a57b3aaa37948a73ab8a5ea7b9e93cc121ece68e69e4b01e09fc4a5b39e59e`  
		Last Modified: Wed, 13 Sep 2023 07:26:55 GMT  
		Size: 2.1 MB (2127596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d967308b6b43e84413e3569c4038c76a3b4bdfa0145f84ca37567f6c26d4f45`  
		Last Modified: Thu, 14 Sep 2023 21:17:37 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20e89fb56338ac7de9292110d8a80e2bfe415ae4822b97269b9d2fe75f21c3`  
		Last Modified: Thu, 14 Sep 2023 21:17:41 GMT  
		Size: 9.5 MB (9502457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fd22e27be44b80f6d4501a4f182e6c4ed4ce4ae33597fd3967eb092f14efd8`  
		Last Modified: Thu, 14 Sep 2023 21:17:35 GMT  
		Size: 215.4 KB (215353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb7837f2327217f0b51ca2319b580dd458a06f723337344706226aa2e3c2bab`  
		Last Modified: Thu, 14 Sep 2023 21:17:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e95a9659c2715df568e631cc1c5309e636fd30507de13c05bf6b877eda6fa`  
		Last Modified: Thu, 14 Sep 2023 21:17:35 GMT  
		Size: 215.0 KB (214955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61dd8ce87089913a80a7a322d8e4efc87153ae3b264bec54eca153529ccfac2d`  
		Last Modified: Thu, 14 Sep 2023 21:17:35 GMT  
		Size: 332.8 KB (332829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87675ec4cb6790694b61b33303499b74f5b8ee30c574657d6833daa1a44bb64e`  
		Last Modified: Thu, 14 Sep 2023 21:17:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
