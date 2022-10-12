## `mongo:latest`

```console
$ docker pull mongo@sha256:946d309038b2581d8913213333eb3f86142d95e770ec6a3e334ca9b43ebd402e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:e0b1614551474ee2f3c3ef7c9706b5e19f2107aa36b73c910522af9fa8eb756e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231723662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cca5cf682396e2ad3b4af822f1e0f64990a940cf9047c8d93b63af592e054aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:30:12 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 05 Oct 2022 18:30:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:30:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 05 Oct 2022 18:30:20 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 05 Oct 2022 18:30:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 18:30:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 18:30:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Wed, 05 Oct 2022 18:30:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 05 Oct 2022 18:30:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 18:30:35 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 18:30:35 GMT
ENV MONGO_MAJOR=6.0
# Wed, 05 Oct 2022 18:30:35 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 05 Oct 2022 18:30:35 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 05 Oct 2022 18:30:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 05 Oct 2022 18:30:59 GMT
VOLUME [/data/db /data/configdb]
# Wed, 05 Oct 2022 18:30:59 GMT
ENV HOME=/data/db
# Wed, 05 Oct 2022 18:30:59 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Wed, 05 Oct 2022 18:31:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:31:00 GMT
EXPOSE 27017
# Wed, 05 Oct 2022 18:31:00 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81bcd64a2d26fbd2741700cc3f6f1aa783ae202298d8010aca8c60f034c4e59`  
		Last Modified: Wed, 05 Oct 2022 18:33:32 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ed91f63dfa037fa6061dee8f91d31f24a66375c70d652e8ee3c77e9e20b0fe`  
		Last Modified: Wed, 05 Oct 2022 18:33:33 GMT  
		Size: 3.1 MB (3059535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d1770a2c11d56f4506d0efdc18d345c397565f38270c9f33347a483a8bfb58`  
		Last Modified: Wed, 05 Oct 2022 18:33:33 GMT  
		Size: 6.5 MB (6505968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d917eab2f0dc57fe40f116099f93a233b75e63df943d2a84d37623faf91ed`  
		Last Modified: Wed, 05 Oct 2022 18:33:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0226311fde3e7d308a8f05fcaae80f725c42a8094ac2b43ec3f2f620a56900d`  
		Last Modified: Wed, 05 Oct 2022 18:33:30 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf22b9bccca1cc8038cc7e33eadd8e43b69b9cd44f141529029365fdf0308dd2`  
		Last Modified: Wed, 05 Oct 2022 18:33:30 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4955b612fd63dc899305e7e50aff0bf7ab5e6dfedb95a184857d50e044c669`  
		Last Modified: Wed, 05 Oct 2022 18:33:57 GMT  
		Size: 193.6 MB (193574947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8341d9c8d5bd44deb9b5a949893e592e59b66a4de7d056f86568f05f53c7a6`  
		Last Modified: Wed, 05 Oct 2022 18:33:30 GMT  
		Size: 5.1 KB (5070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:0a6f2b19ee2f8c5193fa286524aa9949c3a68af5b2e8440d2f593996376504c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.9 MB (224938630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa885bebec49cae70e782b1d0fcb92fccebfb386ccd76251ceb1b0f99e08bb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:54:34 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 05 Oct 2022 16:54:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:54:45 GMT
ENV GOSU_VERSION=1.12
# Wed, 05 Oct 2022 16:54:46 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 05 Oct 2022 16:55:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 16:55:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 16:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Wed, 05 Oct 2022 16:55:06 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 05 Oct 2022 16:55:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 16:55:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 05 Oct 2022 16:55:09 GMT
ENV MONGO_MAJOR=6.0
# Wed, 05 Oct 2022 16:55:10 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 05 Oct 2022 16:55:11 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 05 Oct 2022 16:55:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 05 Oct 2022 16:55:35 GMT
VOLUME [/data/db /data/configdb]
# Wed, 05 Oct 2022 16:55:35 GMT
ENV HOME=/data/db
# Wed, 05 Oct 2022 16:55:37 GMT
COPY file:a062061dd38363517a589afdd763f61500b162faee89d415017c58fd70abe392 in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:55:38 GMT
EXPOSE 27017
# Wed, 05 Oct 2022 16:55:39 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a7df5fbbc12c4cd8f740fabdbbe301d6a4efe1b81b3f196474a28d0322c92`  
		Last Modified: Wed, 05 Oct 2022 16:59:14 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a5e151a7f04dcea23cd214c84a62e5c02bfd8bf21e50b6384cb32a7dac4ed`  
		Last Modified: Wed, 05 Oct 2022 16:59:14 GMT  
		Size: 2.9 MB (2905895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbed2c86a740691aafa2028087ed2a11f64352f3ab06a520efa22bc7c5246f03`  
		Last Modified: Wed, 05 Oct 2022 16:59:14 GMT  
		Size: 6.2 MB (6248099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5c6dc442fc2aca80b585c0c229cf8addb668c43cb2b7b15193532981186e6d`  
		Last Modified: Wed, 05 Oct 2022 16:59:11 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d00e8640a3f0c64b7cd189730daacde9c594bf5850cda768e9e0f97bfbfbcc`  
		Last Modified: Wed, 05 Oct 2022 16:59:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11bc600eb8d283a1a0030c98e1856fd8b96b8f8c86fd7feb0cf74e710e168b4`  
		Last Modified: Wed, 05 Oct 2022 16:59:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b720c57555ba599236671087a8d9d0dae2da8d3677a9e9c240128242c28796`  
		Last Modified: Wed, 05 Oct 2022 16:59:37 GMT  
		Size: 188.6 MB (188584399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194b45d19c19e2b2b24ad7d9b21b2be0ad2e16c100733b8f0ce8ed73fae5873e`  
		Last Modified: Wed, 05 Oct 2022 16:59:11 GMT  
		Size: 5.1 KB (5072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.20348.1129; amd64

```console
$ docker pull mongo@sha256:9f0124900745a02043158bec64db08934598aed691eff9b313a975930a1ab9cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2928919101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75bf702de10b4f40ad8964f5bdaa684e62d98feed607baf785fbcb255b7007f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Wed, 12 Oct 2022 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2022 17:07:21 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 12 Oct 2022 17:07:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.2-signed.msi
# Wed, 12 Oct 2022 17:07:23 GMT
ENV MONGO_DOWNLOAD_SHA256=964a7e33927a8c01a6177daf0bf49f3ec17560b1b78f8be60ec641a03c55cb18
# Wed, 12 Oct 2022 17:09:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 17:09:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Oct 2022 17:09:20 GMT
EXPOSE 27017
# Wed, 12 Oct 2022 17:09:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:81f8c9039f908cbcc912779f9e4c8c5ef145be551538af133f6a9e98c284e2c2`  
		Last Modified: Wed, 12 Oct 2022 14:57:06 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e33316874e96cca28048b1ef4278c583b132be32d3249f6ea78c78385dc1b3`  
		Last Modified: Wed, 12 Oct 2022 17:41:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269dfbb34bb45e2c569b49f31b03cbf5fcd75d896233851d92b8a05337d93b72`  
		Last Modified: Wed, 12 Oct 2022 17:41:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61182a2e145436d402b4cda85b23d80acd1b81bc58329c517fb125e2c735c11`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cd2e92dc993212dbc329b6f7e1bb7c60b7539fd9361ac039ff2a89494d56ef`  
		Last Modified: Wed, 12 Oct 2022 17:43:18 GMT  
		Size: 512.7 MB (512685908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27787617cbd4b0dc9c87d024c1fb08896b5cdaa18007b07d3f83e29929819e35`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b239164ce10fd9be5b8f93faf270cf0abe79a73f11368fbd3404bbb980f59b3`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca04e10644a32bd270c53ee57e9044f61bea611e31447e9b4aca0fa74d9f563`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.3532; amd64

```console
$ docker pull mongo@sha256:e9cc836d8b27bda179ccb5f98c53c51b94d35cf1c5f3c71e10a761480181e3e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 GB (3223653636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66de17796d800a70082f5398c0fc69393e464229b8fd8e7a99e375ae93a1a81`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2022 17:09:38 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 12 Oct 2022 17:09:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.2-signed.msi
# Wed, 12 Oct 2022 17:09:40 GMT
ENV MONGO_DOWNLOAD_SHA256=964a7e33927a8c01a6177daf0bf49f3ec17560b1b78f8be60ec641a03c55cb18
# Wed, 12 Oct 2022 17:12:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 17:12:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Oct 2022 17:12:33 GMT
EXPOSE 27017
# Wed, 12 Oct 2022 17:12:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1078c1a99ba07ad73a4e126d6581d11638f76c357e28c3eb681efd9cfee011`  
		Last Modified: Wed, 12 Oct 2022 17:43:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7ae69d61efab1b59e67a4700c9e9b0c0b0eafe8a8cd4716232bb2026029705`  
		Last Modified: Wed, 12 Oct 2022 17:43:36 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8870889cb57eba8c443d18b1b134d50416c81dba93e7f9e4247349e9ff47e41`  
		Last Modified: Wed, 12 Oct 2022 17:43:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9895666b3b625ce83fa3d38516b691a9b63c5a09981c1d3578b2c0938f921f`  
		Last Modified: Wed, 12 Oct 2022 17:44:49 GMT  
		Size: 512.5 MB (512480197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4133c0cf3dbc96c0edbb9dd37b38e240a5e75b250b0d39262da8fef8a029f1c`  
		Last Modified: Wed, 12 Oct 2022 17:43:33 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0eded977a45e28cb7062c482f62ff5e94eb85cb410b44c67d9f334e4ff91ad`  
		Last Modified: Wed, 12 Oct 2022 17:43:33 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbeed7a7903a3a89688e0a6507ee56f687fd147d5010c782f9f380bb6e6e9460`  
		Last Modified: Wed, 12 Oct 2022 17:43:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
