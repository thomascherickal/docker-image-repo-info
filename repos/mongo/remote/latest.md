## `mongo:latest`

```console
$ docker pull mongo@sha256:2bf2258cb12f8d4086965fe794605571c715fa4815dbcc299ea9768783bf4fa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:a9d3b8f4110063af6a00f30af9f543275f4a9b0b0edeb50e2c5ce9b99057e893
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244580365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d38962b1e5e53c2d00efc0f2d45f7508034895b14586363307f4181a42360d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:06:04 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 14 Jul 2021 01:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:06:13 GMT
ENV GOSU_VERSION=1.12
# Wed, 14 Jul 2021 01:06:13 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 14 Jul 2021 01:06:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jul 2021 01:06:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 19 Jul 2021 16:48:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 19 Jul 2021 16:48:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 19 Jul 2021 16:48:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 19 Jul 2021 16:48:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 19 Jul 2021 16:48:54 GMT
ENV MONGO_MAJOR=5.0
# Mon, 19 Jul 2021 16:48:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 19 Jul 2021 16:48:55 GMT
ENV MONGO_VERSION=5.0.0
# Mon, 19 Jul 2021 16:49:21 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 19 Jul 2021 16:49:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 19 Jul 2021 16:49:24 GMT
VOLUME [/data/db /data/configdb]
# Mon, 19 Jul 2021 16:49:24 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Mon, 19 Jul 2021 16:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 16:49:24 GMT
EXPOSE 27017
# Mon, 19 Jul 2021 16:49:25 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8490627ad476fc39c34e4117fe95181f23c0593c5939334f690c25267a15d1fc`  
		Last Modified: Wed, 14 Jul 2021 01:09:33 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d640de21f3bf1bccb594ae1a3788de970a320dd5c506685ddddb13af3871ff`  
		Last Modified: Wed, 14 Jul 2021 01:09:34 GMT  
		Size: 3.1 MB (3063668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4676d8bbe06cee8d0ab6acff7d9a319287a789dcd95864defe5419be03d50e86`  
		Last Modified: Wed, 14 Jul 2021 01:09:35 GMT  
		Size: 6.5 MB (6505798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33fdc30cbb092983846fd92465e892eeb6684e8391cc3b833f5980850b7e9c7`  
		Last Modified: Wed, 14 Jul 2021 01:09:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9826b02e88282f7c7ec38e49333df2b09a0d9c90bb52ced3c2e6ecc5778ac43e`  
		Last Modified: Mon, 19 Jul 2021 16:51:20 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cc237d4c679679cf14df4cf9c910c10094063a19b904659b4cd1ded414335`  
		Last Modified: Mon, 19 Jul 2021 16:51:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9a7cca861413aa40b73d76f24047efb91b4046194999e1b5c92d2d28bc71d4`  
		Last Modified: Mon, 19 Jul 2021 16:51:49 GMT  
		Size: 206.4 MB (206436832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3924ddfa6129dea5d96686c061885d3593eb6022844f602ec1621af457f8eb0c`  
		Last Modified: Mon, 19 Jul 2021 16:51:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deab31eec3dc9a672849fd78e63349c1e4b9b50e3cf36489467e205391be6c1e`  
		Last Modified: Mon, 19 Jul 2021 16:51:20 GMT  
		Size: 4.5 KB (4476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7979a25edfc1d6d3bfabcb99a901f3efba2c38db87c7a093ceab6f93fe3d90c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237267122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aacc569565364f0664a383fe91f56221c529adfe7fde5d7231907e9fccdb60b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:33:22 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 13 Jul 2021 23:33:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:33:30 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Jul 2021 23:33:30 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 13 Jul 2021 23:33:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:33:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 19 Jul 2021 18:54:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 19 Jul 2021 18:54:57 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 19 Jul 2021 18:54:57 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 19 Jul 2021 18:54:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 19 Jul 2021 18:54:57 GMT
ENV MONGO_MAJOR=5.0
# Mon, 19 Jul 2021 18:54:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 19 Jul 2021 18:54:58 GMT
ENV MONGO_VERSION=5.0.0
# Mon, 19 Jul 2021 18:55:19 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 19 Jul 2021 18:55:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 19 Jul 2021 18:55:21 GMT
VOLUME [/data/db /data/configdb]
# Mon, 19 Jul 2021 18:55:22 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Mon, 19 Jul 2021 18:55:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 18:55:22 GMT
EXPOSE 27017
# Mon, 19 Jul 2021 18:55:22 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0566436151d6a7bfcb49cbc366b5ba571653a68dae1979813510507f0b568665`  
		Last Modified: Tue, 13 Jul 2021 23:37:25 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e35ecfc23ef3b8965133b69f802364d5921cd8275578e99ebc64e709465495`  
		Last Modified: Tue, 13 Jul 2021 23:37:25 GMT  
		Size: 2.9 MB (2913102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03a1be757b04fe0321c6b2dc153d150f21357471d616a43fd71b7fdd3012a2e`  
		Last Modified: Tue, 13 Jul 2021 23:37:26 GMT  
		Size: 6.4 MB (6406269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea0d006dcea6ae065db690271b288012719161d730fdb41f36389e0c4a6b06b`  
		Last Modified: Tue, 13 Jul 2021 23:37:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3446d972a97ce431bcff1e43516e0139296db3068caec1863d4d86ceff5567`  
		Last Modified: Mon, 19 Jul 2021 18:57:29 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c476bc840c3d572702e123c86c5480f9f578675477c5ab557e4cc4b8800c9931`  
		Last Modified: Mon, 19 Jul 2021 18:57:30 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dea434cd2cc206c3cc7cfd0b0534c2af72a51fec61db5edce61f2625897388e`  
		Last Modified: Mon, 19 Jul 2021 18:58:00 GMT  
		Size: 200.8 MB (200770465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233d505385d1137a0ea01716993a9496cb43d79c99ffcca4b2e7e1f7246a1106`  
		Last Modified: Mon, 19 Jul 2021 18:57:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0176c9085e6783672879b8c72b1d9df81e43fb05b190825bd69215ab1c6841`  
		Last Modified: Mon, 19 Jul 2021 18:57:30 GMT  
		Size: 4.5 KB (4473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull mongo@sha256:583073797eacde924c96f95aff64c579246fa495549d10fb677bb37ea6cff4a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2975832945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c8a7ccb1909c83580f8c8769a2da646baf187cbdca1ba4ffc64ae7a74f6d8f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 01:07:30 GMT
ENV MONGO_VERSION=5.0.0
# Wed, 14 Jul 2021 01:07:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.0-signed.msi
# Wed, 14 Jul 2021 01:07:37 GMT
ENV MONGO_DOWNLOAD_SHA256=26920cf86cf1eea8acbf395ad12b0b94631ca4175dc47588a5dc4d9221f014cd
# Wed, 14 Jul 2021 01:13:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 01:14:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Jul 2021 01:14:07 GMT
EXPOSE 27017
# Wed, 14 Jul 2021 01:14:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ba00b69bf586531acf7efc20fc81dc4999d814cf0569cc072e1302492e3f11`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d00ee3059d4a1d94509843dca7851a95b814976100864963b647f52607358`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357882103d154942b3e8762c0dedc4c830de99023e0ecb345fb8fc9fbdeb4dbc`  
		Last Modified: Wed, 14 Jul 2021 02:02:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a8938c18426de8f03985c6d625d449b206a37bb87d01d3b00cd6c6fdd57aa9`  
		Last Modified: Wed, 14 Jul 2021 02:03:18 GMT  
		Size: 290.4 MB (290376267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bbcf6b6079d1ac7b75f7374484401ce5170d6176044d1f158ebcef72c0ba92`  
		Last Modified: Wed, 14 Jul 2021 02:02:17 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e672045b350b08cf7fcd9b8a6f01ab8af895b5cdfd81871e314ccb4d28efe`  
		Last Modified: Wed, 14 Jul 2021 02:02:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec691ab2f20fd8c0fac35aeecf30f62d30572db0b0966f5338fc68386e7e266`  
		Last Modified: Wed, 14 Jul 2021 02:02:17 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4530; amd64

```console
$ docker pull mongo@sha256:6482b51d0de718dc17aa087e321057559eafdcdf986f8d8e41446ec8b41c0fc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6564408948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25effbe6d69101bd7f3cb25be8c091f4403364440a2298c8ccb133dd9c410f58`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 01:14:28 GMT
ENV MONGO_VERSION=5.0.0
# Wed, 14 Jul 2021 01:14:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.0-signed.msi
# Wed, 14 Jul 2021 01:14:35 GMT
ENV MONGO_DOWNLOAD_SHA256=26920cf86cf1eea8acbf395ad12b0b94631ca4175dc47588a5dc4d9221f014cd
# Wed, 14 Jul 2021 01:23:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 01:23:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Jul 2021 01:23:20 GMT
EXPOSE 27017
# Wed, 14 Jul 2021 01:23:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f267a6cc1ee766b749b19baff8f6e0875ea6918b5b0720836082d434a7f42632`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c26de76b84a77e2e80235a036fda1baee78da3428eb9d63ef4c14b72feaf7d`  
		Last Modified: Wed, 14 Jul 2021 02:03:36 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f1fc594e3a7d5941b91a5f94a305bdefb4b18cd9a5e49dcb131ee57e1c0d`  
		Last Modified: Wed, 14 Jul 2021 02:03:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af26b0815d8544dc762b63891d76215bb55b0978c289d568ab58afa1fc5cbd96`  
		Last Modified: Wed, 14 Jul 2021 02:04:37 GMT  
		Size: 294.8 MB (294766930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766b54dba8ac38cfe817a8bcb2e6a99b8b9fbf512452b5ccb2769e1bfa944be8`  
		Last Modified: Wed, 14 Jul 2021 02:03:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278ac62d7576fdc7b729ea001e754038fa36669acff5291a75fd247d5d36337e`  
		Last Modified: Wed, 14 Jul 2021 02:03:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518d2932317a6fce3a384a0a2938c64345cc03b5f0e3b117e27ab20a2d6b9a64`  
		Last Modified: Wed, 14 Jul 2021 02:03:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
