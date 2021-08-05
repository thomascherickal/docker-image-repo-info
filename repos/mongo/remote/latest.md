## `mongo:latest`

```console
$ docker pull mongo@sha256:de4bdff428f383375b32a4bf4b38ab4d4e445bb985c84950577b44d0321ff37b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:3938ddf3039cc291ce26ef63fddfb36441f8fae9909a5e5ec521453d850de812
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248438628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269b735e72cb9c7173c52d775d56453594f32a37f63a71a5404390ce4d51db7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:19:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 27 Jul 2021 00:19:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:19:09 GMT
ENV GOSU_VERSION=1.12
# Tue, 27 Jul 2021 00:19:09 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 27 Jul 2021 00:19:20 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Jul 2021 00:19:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 27 Jul 2021 00:19:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Tue, 27 Jul 2021 00:19:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 27 Jul 2021 00:19:22 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 27 Jul 2021 00:19:22 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 27 Jul 2021 00:19:23 GMT
ENV MONGO_MAJOR=5.0
# Tue, 27 Jul 2021 00:19:23 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 05 Aug 2021 21:33:57 GMT
ENV MONGO_VERSION=5.0.2
# Thu, 05 Aug 2021 21:34:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 05 Aug 2021 21:34:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 05 Aug 2021 21:34:29 GMT
VOLUME [/data/db /data/configdb]
# Thu, 05 Aug 2021 21:34:29 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Thu, 05 Aug 2021 21:34:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 21:34:30 GMT
EXPOSE 27017
# Thu, 05 Aug 2021 21:34:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6335cf672677ce540e0f02f99098fdbb5fe6c11e4322a415119dd06f3be5c0a0`  
		Last Modified: Tue, 27 Jul 2021 00:23:01 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc70ccc8ebe91e13d0460b1b78df150627a7bfc892b2c6cc87112b06dcd2eb6`  
		Last Modified: Tue, 27 Jul 2021 00:22:59 GMT  
		Size: 3.1 MB (3063745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a3c6bd4175a271cffe4b4ea115ba6b94fa4fff3080aea88bf69c8fd3f281c`  
		Last Modified: Tue, 27 Jul 2021 00:22:59 GMT  
		Size: 6.5 MB (6505864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960f3b9b27d33484b86cc838f3f5c815a0d06833e1af863dedaedc06dfa1b514`  
		Last Modified: Tue, 27 Jul 2021 00:22:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff995a136b4c466ef26b6a73769cb41165c8c17601f986304cb30d6cdfc3e95`  
		Last Modified: Tue, 27 Jul 2021 00:22:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4249be7550a87f522c717dd417cd2cb7dd9cca40b8a28ef718ac441376b94a47`  
		Last Modified: Tue, 27 Jul 2021 00:22:56 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc105ff5aa3c95b1bd85a3de5d04f1b89a0cb413ff63c2ae06dd69d1055663d5`  
		Last Modified: Thu, 05 Aug 2021 21:35:32 GMT  
		Size: 210.3 MB (210292636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82819807d07a07bd4a2da6ca2dc5059101647d729e915af34c4685b06fc1d9c8`  
		Last Modified: Thu, 05 Aug 2021 21:35:05 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81447d2c233f0fbbb1fde2e92e6dd9dcc33983fac3441e63b21eb6d3585db95c`  
		Last Modified: Thu, 05 Aug 2021 21:35:05 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:750b49c7ae0106f2ba218d9f49106ed91593f2c0727ec8a0c67d8e42fcab87f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.9 MB (237860656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394109e13c9f4e9981092285d96e85d4a295801624c5f9faf93954cc898c41e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:28:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 26 Jul 2021 23:28:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:28:57 GMT
ENV GOSU_VERSION=1.12
# Mon, 26 Jul 2021 23:28:57 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 26 Jul 2021 23:29:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 26 Jul 2021 23:29:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 26 Jul 2021 23:29:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 26 Jul 2021 23:29:15 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 26 Jul 2021 23:29:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 26 Jul 2021 23:29:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 26 Jul 2021 23:29:15 GMT
ENV MONGO_MAJOR=5.0
# Mon, 26 Jul 2021 23:29:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 05 Aug 2021 21:54:34 GMT
ENV MONGO_VERSION=5.0.2
# Thu, 05 Aug 2021 21:54:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 05 Aug 2021 21:54:57 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 05 Aug 2021 21:54:57 GMT
VOLUME [/data/db /data/configdb]
# Thu, 05 Aug 2021 21:54:57 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Thu, 05 Aug 2021 21:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 21:54:57 GMT
EXPOSE 27017
# Thu, 05 Aug 2021 21:54:58 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c078c670449119708548deb73fc4b2367fa17e7aa2ccf7d9635f052a393175d7`  
		Last Modified: Mon, 26 Jul 2021 23:32:50 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d7ca682de71cc0d28d5a25c21dcd26bce98321effac96e7c222cad612f192f`  
		Last Modified: Mon, 26 Jul 2021 23:32:51 GMT  
		Size: 2.9 MB (2913005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1276b06a5f9112b01253aa3f54e3998c37b6a78454d9c53873756a9feb2852d1`  
		Last Modified: Mon, 26 Jul 2021 23:32:52 GMT  
		Size: 6.4 MB (6406013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b013f927ec79564222ec0dc72cf65f4fe208c8cb483473270d2ef088d3dff15e`  
		Last Modified: Mon, 26 Jul 2021 23:32:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb2ec585db85844694fb5c40b3aaf11584b901a26a90e01ab19a11dfe0743e7`  
		Last Modified: Mon, 26 Jul 2021 23:32:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d617d81a7e82ac4f372117a401b12f4646105669b226e2513f2edf29223807`  
		Last Modified: Mon, 26 Jul 2021 23:32:48 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7298e8dce6d45b0f1589509f6deedfdc70e6a70c6427c9dd4c0720a2993f6159`  
		Last Modified: Thu, 05 Aug 2021 21:56:33 GMT  
		Size: 201.4 MB (201362943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1790452de67cc844d6c4b03e751d7fe4e2f3d040f9e9ce5ba2916b26be52f30c`  
		Last Modified: Thu, 05 Aug 2021 21:56:04 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad154a091baba107422a8b030aa963ff50ae52fad4ed5232acc0f8dfc617e76`  
		Last Modified: Thu, 05 Aug 2021 21:56:05 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull mongo@sha256:7f9a32eec6f5804309f996816938bd8ccf63fefcc9370d751b50dc3b5d0f2074
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2976198684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f3df5fa2043b4ba1ec5d3bcec3352f13bd9e0865868363aed844b92ce5e6bf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 05 Aug 2021 21:15:21 GMT
ENV MONGO_VERSION=5.0.2
# Thu, 05 Aug 2021 21:15:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.2-signed.msi
# Thu, 05 Aug 2021 21:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=8c517e4b1598d627ee16c2dd45be90397bf040cf2845eef2aff0b9bc25062228
# Thu, 05 Aug 2021 21:17:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 05 Aug 2021 21:17:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 05 Aug 2021 21:17:49 GMT
EXPOSE 27017
# Thu, 05 Aug 2021 21:17:52 GMT
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
	-	`sha256:dbfaea6ff2465a6876267b3cf736ca2829d0c38c133eaa24f8108fb70e4b8e4d`  
		Last Modified: Thu, 05 Aug 2021 21:24:29 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77955ed311898043bbe149dc3c66e1a071df4a6b3fc8775e9473980ad7d5fa`  
		Last Modified: Thu, 05 Aug 2021 21:24:29 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2130afeb329a6949621ac7d3da1e51e4f82981820cbd2d8491a0795b92e787`  
		Last Modified: Thu, 05 Aug 2021 21:24:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd36685c3e8bd8c6fee72ac04e3f3e6ef5cb50bfcaaea6d09b5780be4a65869`  
		Last Modified: Thu, 05 Aug 2021 21:29:49 GMT  
		Size: 290.7 MB (290741928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9656db404f6054408953812fcbbb4a8f964b102cd798f9b3b5cafe1f3dd1b73`  
		Last Modified: Thu, 05 Aug 2021 21:24:26 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231979b9550fc2a3cf73b834cd716c48ece14908411681a3ec56a670127d9cb1`  
		Last Modified: Thu, 05 Aug 2021 21:24:26 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04e6d9fdfff0fa71c06252999e8a7285087380982a52feb4632d7e26eed2627`  
		Last Modified: Thu, 05 Aug 2021 21:24:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4530; amd64

```console
$ docker pull mongo@sha256:48f33ad940095393cf0ca36bd93bbd509ff9b5734963d0f86306273fb560a8d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6564790442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adcfe53b040d7a3e6be110c4826a4a17e8a2e5023938c709c572463aac5a70a5`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 05 Aug 2021 21:18:02 GMT
ENV MONGO_VERSION=5.0.2
# Thu, 05 Aug 2021 21:18:05 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.2-signed.msi
# Thu, 05 Aug 2021 21:18:07 GMT
ENV MONGO_DOWNLOAD_SHA256=8c517e4b1598d627ee16c2dd45be90397bf040cf2845eef2aff0b9bc25062228
# Thu, 05 Aug 2021 21:20:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 05 Aug 2021 21:21:00 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 05 Aug 2021 21:21:03 GMT
EXPOSE 27017
# Thu, 05 Aug 2021 21:21:05 GMT
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
	-	`sha256:66621c417ef0c52ad82579ecba48db8a7b1bb4be439def736aec2880a8919573`  
		Last Modified: Thu, 05 Aug 2021 21:30:10 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faf8fd84aba2e08bc0b9f30d4719e358497d05e9960027c5ba9ce71e8e0ccc7`  
		Last Modified: Thu, 05 Aug 2021 21:30:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f8c421adf1f6252e10e8ef42fe9e31081f4c8d42ae8756f00285b7a4f22425`  
		Last Modified: Thu, 05 Aug 2021 21:30:07 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4934777b42c788fc8735ff4e965b26c0b9783b00120eaada40d0d00d2b8df091`  
		Last Modified: Thu, 05 Aug 2021 21:35:56 GMT  
		Size: 295.1 MB (295148447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e6093429f6fc9a7e714308688bef6e2f59cdd0554ffae34fa930582e41da0c`  
		Last Modified: Thu, 05 Aug 2021 21:30:07 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442bf8d18468bc0699e54e62e4ca95b28f63284b1781d907797a41f9e3ba41f5`  
		Last Modified: Thu, 05 Aug 2021 21:30:06 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08b16d65cadb168ab2e8af69d77c549bd254c8b529823208458b88bcdb5fdec`  
		Last Modified: Thu, 05 Aug 2021 21:30:06 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
