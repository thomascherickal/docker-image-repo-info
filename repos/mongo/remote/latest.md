## `mongo:latest`

```console
$ docker pull mongo@sha256:ae1ae34d5e470af7b1a5ca26565e913eec5f9f645701036e6d6860dfcacfa116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:87ae78e36c0234dd0ef3c03a65d06353ffac67eb7b22c411cff960f134806642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248813510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf4b4ee3beead6425ed92e6ae915bd0a5da899bd43e2722a756eceb579aa5d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:51:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 31 Aug 2021 03:51:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:51:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 31 Aug 2021 03:51:15 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 31 Aug 2021 03:51:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:51:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:51:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:51:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 31 Aug 2021 03:51:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 31 Aug 2021 03:51:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 31 Aug 2021 03:51:35 GMT
ENV MONGO_MAJOR=5.0
# Tue, 31 Aug 2021 03:51:35 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 20 Sep 2021 22:20:11 GMT
ENV MONGO_VERSION=5.0.3
# Mon, 20 Sep 2021 22:20:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 20 Sep 2021 22:20:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 20 Sep 2021 22:20:48 GMT
VOLUME [/data/db /data/configdb]
# Mon, 20 Sep 2021 22:20:48 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Mon, 20 Sep 2021 22:20:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Sep 2021 22:20:48 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:20:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664b0ebdcc074096f3cdb5767cd0679b6eb1b867cc4803caebc900c3a0e3cd7a`  
		Last Modified: Tue, 31 Aug 2021 03:54:55 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d598f4d3c08173a580ddfbc1aab7570a506bbe19ef2f760eef62bb18b0f2fe42`  
		Last Modified: Tue, 31 Aug 2021 03:54:56 GMT  
		Size: 3.1 MB (3064917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291455135b00f1125d53ec53b9bd1246a1a95c5289d78d52aeeebc2ca216e5ed`  
		Last Modified: Tue, 31 Aug 2021 03:54:56 GMT  
		Size: 6.5 MB (6506306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46409342f130fad45e914eb39eb6ff00f27268fb1b229f287a6b8102d7aa9bf`  
		Last Modified: Tue, 31 Aug 2021 03:54:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2b9c6e6f3a34b81bff9c8e5cca15de3929bb9eaac42390afe055c4fb1dead8`  
		Last Modified: Tue, 31 Aug 2021 03:54:53 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149f6335fc27dbe4a0d20cedeadb246cd0527052841f69e697ecf1dc3e5345cf`  
		Last Modified: Tue, 31 Aug 2021 03:54:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0adda745823b05b58810f001e2b9c63d7c51d9bef9508d80d3f5d0fafe62aa`  
		Last Modified: Mon, 20 Sep 2021 22:22:49 GMT  
		Size: 210.7 MB (210663765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170bad7cd6cb209d04013bdd2899703d7b499e4bc21699f97e7bf86f6048af57`  
		Last Modified: Mon, 20 Sep 2021 22:22:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7fd7a769b4bc7b673d2aca605c010f13f8cd5ebc222d0940a9449a3d1ec94f`  
		Last Modified: Mon, 20 Sep 2021 22:22:21 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:60626ad703d8eb6d6c99109ddda65445e162819974686e3ea17fde2a6c492856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.2 MB (238240260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8863e1385d8c6e12bc18bccf4943b1e99ef82311c0902af6e2cd01f17a31b84e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:15:52 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 31 Aug 2021 03:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:15:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 31 Aug 2021 03:16:00 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 31 Aug 2021 03:16:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Aug 2021 03:16:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 31 Aug 2021 03:16:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Tue, 31 Aug 2021 03:16:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 31 Aug 2021 03:16:23 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 31 Aug 2021 03:16:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 31 Aug 2021 03:16:24 GMT
ENV MONGO_MAJOR=5.0
# Tue, 31 Aug 2021 03:16:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 20 Sep 2021 22:40:12 GMT
ENV MONGO_VERSION=5.0.3
# Mon, 20 Sep 2021 22:40:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 20 Sep 2021 22:40:37 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 20 Sep 2021 22:40:37 GMT
VOLUME [/data/db /data/configdb]
# Mon, 20 Sep 2021 22:40:37 GMT
COPY file:df3353d9b2c25ef83b499ecae7fd5d611adb4a9462a577435178acaad3c8c695 in /usr/local/bin/ 
# Mon, 20 Sep 2021 22:40:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Sep 2021 22:40:38 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:40:38 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9e2375f5b5048fb0013ccb2e7290680c2590799520474598fe5ed6e21b3fa9`  
		Last Modified: Tue, 31 Aug 2021 03:20:22 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc6079c33aea50db5ae3f5319d71f1cdf0b7d825e846d2d5d2051bddee77e6`  
		Last Modified: Tue, 31 Aug 2021 03:20:22 GMT  
		Size: 2.9 MB (2915391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e5461d9f2757a86731db084491d3c69e14f07c17810efd521d6aada80f86e2`  
		Last Modified: Tue, 31 Aug 2021 03:20:22 GMT  
		Size: 6.4 MB (6406210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249760dddaa1f69b0c9d1f8a23943c6d0eba70c05f68f93646af174928ab2ab7`  
		Last Modified: Tue, 31 Aug 2021 03:20:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e94ab21b2c6a234bc42bd66502c16587a74d8a32f4a6e9ee43682ef83aa9420`  
		Last Modified: Tue, 31 Aug 2021 03:20:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acb3085c69e083aa0d451db77aa3c6bbf3203d22bcd2e86928c4f08e75dd8a6`  
		Last Modified: Tue, 31 Aug 2021 03:20:19 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07313093f31c07221badf075779bfb02a222e3123935e9a1354292d7445f4373`  
		Last Modified: Mon, 20 Sep 2021 22:43:07 GMT  
		Size: 201.7 MB (201737114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91efeb9d2ad2bd28582978ba9587af025b84ce30be0bc5db536f37118994fa32`  
		Last Modified: Mon, 20 Sep 2021 22:42:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eb5729d7522eb0ef5a944ea8d611873f9ef18b751e26f24e4f48bb35fbf4e1`  
		Last Modified: Mon, 20 Sep 2021 22:42:39 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull mongo@sha256:2b500ba0a4cc9ce236bbf5e5af7d7378556709262e67a113213aaa5da62c377b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2979920524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d657dcf41c9f0c1a8383d1e4e8db079bb443c32d61d221966e18e0fe1f1fcd03`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 20 Sep 2021 22:14:14 GMT
ENV MONGO_VERSION=5.0.3
# Mon, 20 Sep 2021 22:14:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Mon, 20 Sep 2021 22:14:16 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Mon, 20 Sep 2021 22:16:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 20 Sep 2021 22:16:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 20 Sep 2021 22:16:12 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:16:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7f5fa305ac9a7cae1fc9cc688b53baa18837be3d5f79eb0587497835880f7`  
		Last Modified: Mon, 20 Sep 2021 22:32:34 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4692808562fcbc70235caff11f59a06500433671d6ff412182d5cf42219c80`  
		Last Modified: Mon, 20 Sep 2021 22:32:35 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874670cd184b2724b759e4e451b277cda6ecf83de8aac320fd86019859a084b5`  
		Last Modified: Mon, 20 Sep 2021 22:32:32 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6f2d37545c92b2c8ce7ceb68a1dc961e9a055f7e983b4c851809db2f173c8c`  
		Last Modified: Mon, 20 Sep 2021 22:33:21 GMT  
		Size: 293.2 MB (293213420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a6ebcc7b6571c8f36738797624455bc961dceb9fe56e8bd67a9ec81a1a987`  
		Last Modified: Mon, 20 Sep 2021 22:32:32 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73771d0c19d44eab18cec21179471862c21f26af6a9a033fe527498c395abf3e`  
		Last Modified: Mon, 20 Sep 2021 22:32:32 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa3a83f1f1d4a559192a9add79a3f1c06bbad9e9b8397b1713d063df259158`  
		Last Modified: Mon, 20 Sep 2021 22:32:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4651; amd64

```console
$ docker pull mongo@sha256:3ddad03a7279c1341b4570a743d2414bb5eeff5271cc8cec30e5094ae1926055
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6564471778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c572a2c8f778bcbba0790a1682b8100d9f10006717ffbf583456d516167c7ba4`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 20 Sep 2021 22:16:25 GMT
ENV MONGO_VERSION=5.0.3
# Mon, 20 Sep 2021 22:16:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Mon, 20 Sep 2021 22:16:27 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Mon, 20 Sep 2021 22:18:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 20 Sep 2021 22:18:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 20 Sep 2021 22:18:41 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:18:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afb02f0864e2f417689553ca4651007c924fde6a2a3b76821f118c040e5a8c6`  
		Last Modified: Mon, 20 Sep 2021 22:33:41 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c456a1eb4c2a7bb8ab05f8333ec09e03020f6f883882f5ae1f5d87127f60efb`  
		Last Modified: Mon, 20 Sep 2021 22:33:41 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a907f49c68ba7eef36c5b0ce07d61724656908933d8e2b2f23c2c15b9843cc`  
		Last Modified: Mon, 20 Sep 2021 22:33:39 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af01aa1cd1a5bbc107d55580bf40cbf2351309b3709aa661bf39bd92cc8038fe`  
		Last Modified: Mon, 20 Sep 2021 22:38:41 GMT  
		Size: 293.1 MB (293134182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba33f1bfc0910888203542fc61d1b07883e604bf741523706d6a132d99b25f0`  
		Last Modified: Mon, 20 Sep 2021 22:33:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a8b9d22a82d81780464084844c38823321543094a315c9d7b946b3026c316`  
		Last Modified: Mon, 20 Sep 2021 22:33:39 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607e27b4543dcbb46550899cc88aecdf74108566566b027a79126433b5dc2019`  
		Last Modified: Mon, 20 Sep 2021 22:33:38 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
