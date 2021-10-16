## `mongo:latest`

```console
$ docker pull mongo@sha256:e81cabac4254ba26d634857dca172abcca1eb7a1f5cb2217e3dfd4797b1b214c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:af71b1de6636e0819661a0d67ede72947ac4fd8e60d984132ffa9183738a9a82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.5 MB (249537889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a14d3979c54cfd497d225371c3e0403a1481b455cb76187775916348ca9e4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:26:54 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 01 Oct 2021 05:27:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:27:03 GMT
ENV GOSU_VERSION=1.12
# Fri, 01 Oct 2021 05:27:03 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 01 Oct 2021 05:27:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 01 Oct 2021 05:27:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 01 Oct 2021 05:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 05:27:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 01 Oct 2021 05:27:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:27:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 01 Oct 2021 05:27:32 GMT
ENV MONGO_MAJOR=5.0
# Fri, 01 Oct 2021 05:27:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 01 Oct 2021 05:27:33 GMT
ENV MONGO_VERSION=5.0.3
# Fri, 01 Oct 2021 05:27:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 01 Oct 2021 05:28:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 01 Oct 2021 05:28:00 GMT
VOLUME [/data/db /data/configdb]
# Fri, 01 Oct 2021 05:28:00 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Fri, 01 Oct 2021 05:28:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 05:28:01 GMT
EXPOSE 27017
# Fri, 01 Oct 2021 05:28:01 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a49f973a13ed259e90f90d516bfd4e86e1294e08ede4b21ddfc91edb575b5c`  
		Last Modified: Fri, 01 Oct 2021 05:29:53 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d4dd6d90045fa1230831362a51b6b81ea0517b3465770ded77c3a427dc997`  
		Last Modified: Fri, 01 Oct 2021 05:29:54 GMT  
		Size: 3.1 MB (3064401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e410f3a61fe9b9491dc6759a94320308ed31e2a7f55773efd31b149b2dcc5f`  
		Last Modified: Fri, 01 Oct 2021 05:29:54 GMT  
		Size: 6.5 MB (6506405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84513ed7bcb687931b1e7054ac30be79aa065bda2aead342ce9fdf4cf16a8d50`  
		Last Modified: Fri, 01 Oct 2021 05:29:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c69ef6aac84f33a417053e791c50647b3042ffec8d33c9dfad2ec52c06ba821`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc764861fa21f832bce37509cafb48035d10dc8a553d1f2e6910d4c6d8767e1`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a312d8b37ffda4e2af86a952f762d3dc6dbbf4638ddc151aacadbba9e3299d30`  
		Last Modified: Fri, 01 Oct 2021 05:30:19 GMT  
		Size: 211.4 MB (211389736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f757690572b3fb279e22d555aa3830afd42b562890b8f2386531bd49c64b84`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6327a25cb49090b335dca3053e4cf22e0b7a646e951b198e773c98b11d41a5`  
		Last Modified: Fri, 01 Oct 2021 05:29:51 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:add6da48a188a4f979c1b99e6f1e2baa746b4fbdd42ff5d176d45de97d48d448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.5 MB (239484798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addfd455919fa552fae7dc3cfd6d8fa690c784f7bf07aeaa866e5c87ab106063`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:06:06 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Sat, 16 Oct 2021 02:06:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:06:15 GMT
ENV GOSU_VERSION=1.12
# Sat, 16 Oct 2021 02:06:16 GMT
ENV JSYAML_VERSION=3.13.1
# Sat, 16 Oct 2021 02:06:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 16 Oct 2021 02:06:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 16 Oct 2021 02:06:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 16 Oct 2021 02:06:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Sat, 16 Oct 2021 02:06:45 GMT
ARG MONGO_REPO=repo.mongodb.org
# Sat, 16 Oct 2021 02:06:46 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Sat, 16 Oct 2021 02:06:47 GMT
ENV MONGO_MAJOR=5.0
# Sat, 16 Oct 2021 02:06:48 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Sat, 16 Oct 2021 02:06:49 GMT
ENV MONGO_VERSION=5.0.3
# Sat, 16 Oct 2021 02:07:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Sat, 16 Oct 2021 02:07:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Sat, 16 Oct 2021 02:07:12 GMT
VOLUME [/data/db /data/configdb]
# Sat, 16 Oct 2021 02:07:14 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Sat, 16 Oct 2021 02:07:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 02:07:15 GMT
EXPOSE 27017
# Sat, 16 Oct 2021 02:07:16 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b19666caec16fe4ae329c791ac93b397bbc78b9f84cb6e735d21b83b2eb9c0e`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b1addf2da74eccff510de6aa5ab3d3d000656817b97884d02f892fb93248a`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 2.9 MB (2911827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef180f0d597c6eed96a83a2f6d97d4345b9909ebbee8ac80b5ecc71a368d23b`  
		Last Modified: Sat, 16 Oct 2021 02:11:20 GMT  
		Size: 6.2 MB (6248421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6d24c0ec70825ca68ce4d4304ca3d41b4d65622f2c1758be2423bc43e5b3d`  
		Last Modified: Sat, 16 Oct 2021 02:11:19 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346d14d0731950cdc142603e6f36a1a1f88862b63bfbca743f453854687c6d25`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c6a1451b8d8b9cded5ff44f9960282c4072f710a83595c62fc6778da82bb02`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68748565d9e0d7cff2e11e0e2920c28476b051004b142f623dfd774b7c5e3374`  
		Last Modified: Sat, 16 Oct 2021 02:11:43 GMT  
		Size: 203.1 MB (203145319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7832c0e6bbd861db05e9e2017dcecd553ba04004ea2a7c0d4e02af1aac6851ff`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6468d66f0471f9c6d1bb37fda98f07757e8d839a49f24450a4b29c8f83aeea33`  
		Last Modified: Sat, 16 Oct 2021 02:11:17 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull mongo@sha256:e2747a08b689a3b97a4d09929a097dbee0f6bca563ff022f104a13142e2c262e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2979520355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579f3eb8ee743f4d6188a27507b0c99918ca88f64701c91ce3e827d6841901ae`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Oct 2021 01:34:40 GMT
ENV MONGO_VERSION=5.0.3
# Thu, 14 Oct 2021 01:34:41 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Thu, 14 Oct 2021 01:34:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Thu, 14 Oct 2021 01:37:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Oct 2021 01:37:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Oct 2021 01:37:18 GMT
EXPOSE 27017
# Thu, 14 Oct 2021 01:37:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b2385e226e317a6557eaceb5c6dc1c367964183df6748248f8af5921c23462`  
		Last Modified: Thu, 14 Oct 2021 02:12:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08208875db9c78866fea34cdc6dc4d3963a8dc959f4ec4e00de909d304d47c43`  
		Last Modified: Thu, 14 Oct 2021 02:12:20 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffaedd446f56ec6d6ec35fca8ceed8e8ed372f2cde489271ff057fdd964f54a`  
		Last Modified: Thu, 14 Oct 2021 02:12:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d465b78d6d6813f216b6b4d6ab90ef93e13f6b08e8ac5e0832822e32ed53d561`  
		Last Modified: Thu, 14 Oct 2021 02:13:16 GMT  
		Size: 293.2 MB (293191826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3571d9235cdda81b5cd4c0793bf5f049574bd1127ad9013174679b2116b4394e`  
		Last Modified: Thu, 14 Oct 2021 02:12:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef366eda8992bb91d0b5e1da4d6655e0d78447b8e6c02ad9c2e6d8d909064c4`  
		Last Modified: Thu, 14 Oct 2021 02:12:18 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52f9c42f83c400061de870926fd0203a5ad3a1e1b57dbc203c78d25236edb40`  
		Last Modified: Thu, 14 Oct 2021 02:12:18 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4704; amd64

```console
$ docker pull mongo@sha256:5aa1e501fdf40a5b943041a7c76b98e5eb36453475d222f22d2f7ecb7c68040a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6570428452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa652834c2451f4d3fdfeef337e698fccc2a69bed8550c93fa12d4769f726d2b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Oct 2021 01:37:38 GMT
ENV MONGO_VERSION=5.0.3
# Thu, 14 Oct 2021 01:37:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Thu, 14 Oct 2021 01:37:40 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Thu, 14 Oct 2021 01:40:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Oct 2021 01:40:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Oct 2021 01:40:08 GMT
EXPOSE 27017
# Thu, 14 Oct 2021 01:40:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026fa80ac8ef8a7f950cb3273ddbdfea355144ec3e61cecc6b41eefcbbdcf02c`  
		Last Modified: Thu, 14 Oct 2021 02:13:33 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02845091172815e9e6943dfa2c88c656ad80313fb7efb0da2ef810eec120aeac`  
		Last Modified: Thu, 14 Oct 2021 02:13:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2b50335afc1b22c1071610521067d3372df20bf6d29dd1caf9abd8251ac67a`  
		Last Modified: Thu, 14 Oct 2021 02:13:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb2e5dc23b57a70c519fae7e3501305a9c9af6f2e454c7197634835eae46327`  
		Last Modified: Thu, 14 Oct 2021 02:19:01 GMT  
		Size: 297.7 MB (297652044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9a4a355fd7a90856553ea198dc91afe423683f53e764a04fe792646249be02`  
		Last Modified: Thu, 14 Oct 2021 02:13:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d1efcb2961b1f99dee8b381f05dce8d1a18733bf7148227277c74e4a582946`  
		Last Modified: Thu, 14 Oct 2021 02:13:31 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4978e2dae55b23d4f58b6f36a52b8f5e82f0d2975c8b7fe370e425ba3e196977`  
		Last Modified: Thu, 14 Oct 2021 02:13:31 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
