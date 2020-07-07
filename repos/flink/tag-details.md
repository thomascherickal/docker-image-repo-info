<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `flink`

-	[`flink:1.10`](#flink110)
-	[`flink:1.10.1`](#flink1101)
-	[`flink:1.10.1-scala_2.11`](#flink1101-scala_211)
-	[`flink:1.10.1-scala_2.12`](#flink1101-scala_212)
-	[`flink:1.10-scala_2.11`](#flink110-scala_211)
-	[`flink:1.10-scala_2.12`](#flink110-scala_212)
-	[`flink:1.11`](#flink111)
-	[`flink:1.11.0`](#flink1110)
-	[`flink:1.11.0-scala_2.11`](#flink1110-scala_211)
-	[`flink:1.11.0-scala_2.12`](#flink1110-scala_212)
-	[`flink:1.11-scala_2.11`](#flink111-scala_211)
-	[`flink:1.11-scala_2.12`](#flink111-scala_212)
-	[`flink:latest`](#flinklatest)
-	[`flink:scala_2.11`](#flinkscala_211)
-	[`flink:scala_2.12`](#flinkscala_212)

## `flink:1.10`

```console
$ docker pull flink@sha256:600185ea56904a349f013150e36d7fde9eddcd6fdc79c347cb0973d2e1e2d275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10` - linux; amd64

```console
$ docker pull flink@sha256:28d6cd6b7db46be5c0bf89478d4f86845bdd6bd4b8a1ba20ca6f57442c9a0ea6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395433590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d70764f1a40b0a67cf02cbd2cfb1869f0acddda639396409933944b9077463`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:31 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:33 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:10:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:10:57 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:10:57 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:10:57 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9544573d11b4d075a64f18b4bf8b6fc7127ca27ac8012d8ca4d03247a6d878`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb723504e2e807bdf3564fdb06d0584d123d2396884d27d8643a953cbc0158`  
		Last Modified: Wed, 10 Jun 2020 07:12:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabd3770dbca0e4498c2defa1dd6de1b62f55016a05946f8ea717fd59f03d20`  
		Last Modified: Wed, 10 Jun 2020 07:12:34 GMT  
		Size: 280.0 MB (279952956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99ec43ff140d74d9358b9d2fd63df5fce36b5098e46ef4b49d227f0364636c9`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.1`

```console
$ docker pull flink@sha256:600185ea56904a349f013150e36d7fde9eddcd6fdc79c347cb0973d2e1e2d275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.1` - linux; amd64

```console
$ docker pull flink@sha256:28d6cd6b7db46be5c0bf89478d4f86845bdd6bd4b8a1ba20ca6f57442c9a0ea6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395433590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d70764f1a40b0a67cf02cbd2cfb1869f0acddda639396409933944b9077463`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:31 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:33 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:10:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:10:57 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:10:57 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:10:57 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9544573d11b4d075a64f18b4bf8b6fc7127ca27ac8012d8ca4d03247a6d878`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb723504e2e807bdf3564fdb06d0584d123d2396884d27d8643a953cbc0158`  
		Last Modified: Wed, 10 Jun 2020 07:12:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabd3770dbca0e4498c2defa1dd6de1b62f55016a05946f8ea717fd59f03d20`  
		Last Modified: Wed, 10 Jun 2020 07:12:34 GMT  
		Size: 280.0 MB (279952956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99ec43ff140d74d9358b9d2fd63df5fce36b5098e46ef4b49d227f0364636c9`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.1-scala_2.11`

```console
$ docker pull flink@sha256:e411a769e9e52860427bef3894ca520ab83595e01c299b7e50ca27b24b660e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.1-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:ebddddfb8562eaab832492842202aa2ca8885648d5c553b0331d539215bfe21c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.7 MB (404725774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75decd703832d977f1bde63fcb55c23225948fa7afb28c7a12c1c19d78dae981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:05 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.11.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:05 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:05 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:06 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:06 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:08:23 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:08:24 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:08:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:08:24 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:08:24 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1498d066b76091a31077d148ef176f9f96c44b4bd6ee87aa10753da529da6`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1477089b7b94db43bc3b0dcb3c20a06d877089312029728ceb87d6b880d7793`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c083c5dc6501bf955c220a22f68559c3a2d364fedb5c80d7a8aef08d0052280b`  
		Last Modified: Wed, 10 Jun 2020 07:12:12 GMT  
		Size: 289.2 MB (289245140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e4b1118b66b87d16150143c0e18fe2ce61ee919cb91e7d7da6666985b190da`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.1-scala_2.12`

```console
$ docker pull flink@sha256:600185ea56904a349f013150e36d7fde9eddcd6fdc79c347cb0973d2e1e2d275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.1-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:28d6cd6b7db46be5c0bf89478d4f86845bdd6bd4b8a1ba20ca6f57442c9a0ea6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395433590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d70764f1a40b0a67cf02cbd2cfb1869f0acddda639396409933944b9077463`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:31 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:33 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:10:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:10:57 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:10:57 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:10:57 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9544573d11b4d075a64f18b4bf8b6fc7127ca27ac8012d8ca4d03247a6d878`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb723504e2e807bdf3564fdb06d0584d123d2396884d27d8643a953cbc0158`  
		Last Modified: Wed, 10 Jun 2020 07:12:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabd3770dbca0e4498c2defa1dd6de1b62f55016a05946f8ea717fd59f03d20`  
		Last Modified: Wed, 10 Jun 2020 07:12:34 GMT  
		Size: 280.0 MB (279952956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99ec43ff140d74d9358b9d2fd63df5fce36b5098e46ef4b49d227f0364636c9`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10-scala_2.11`

```console
$ docker pull flink@sha256:e411a769e9e52860427bef3894ca520ab83595e01c299b7e50ca27b24b660e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:ebddddfb8562eaab832492842202aa2ca8885648d5c553b0331d539215bfe21c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.7 MB (404725774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75decd703832d977f1bde63fcb55c23225948fa7afb28c7a12c1c19d78dae981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:05 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.11.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:05 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:05 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:06 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:06 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:08:23 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:08:24 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:08:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:08:24 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:08:24 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1498d066b76091a31077d148ef176f9f96c44b4bd6ee87aa10753da529da6`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1477089b7b94db43bc3b0dcb3c20a06d877089312029728ceb87d6b880d7793`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c083c5dc6501bf955c220a22f68559c3a2d364fedb5c80d7a8aef08d0052280b`  
		Last Modified: Wed, 10 Jun 2020 07:12:12 GMT  
		Size: 289.2 MB (289245140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e4b1118b66b87d16150143c0e18fe2ce61ee919cb91e7d7da6666985b190da`  
		Last Modified: Wed, 10 Jun 2020 07:11:55 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10-scala_2.12`

```console
$ docker pull flink@sha256:600185ea56904a349f013150e36d7fde9eddcd6fdc79c347cb0973d2e1e2d275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:28d6cd6b7db46be5c0bf89478d4f86845bdd6bd4b8a1ba20ca6f57442c9a0ea6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395433590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d70764f1a40b0a67cf02cbd2cfb1869f0acddda639396409933944b9077463`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.1/flink-1.10.1-bin-scala_2.12.tgz.asc GPG_KEY=D8D3D42E84C753CA5F170BDF93C07902771AB743 CHECK_GPG=true
# Wed, 10 Jun 2020 07:08:30 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 10 Jun 2020 07:08:31 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 07:08:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 10 Jun 2020 07:08:33 GMT
WORKDIR /opt/flink
# Wed, 10 Jun 2020 07:10:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 10 Jun 2020 07:10:57 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Wed, 10 Jun 2020 07:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 07:10:57 GMT
EXPOSE 6123 8081
# Wed, 10 Jun 2020 07:10:57 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9544573d11b4d075a64f18b4bf8b6fc7127ca27ac8012d8ca4d03247a6d878`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 4.6 KB (4603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb723504e2e807bdf3564fdb06d0584d123d2396884d27d8643a953cbc0158`  
		Last Modified: Wed, 10 Jun 2020 07:12:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebabd3770dbca0e4498c2defa1dd6de1b62f55016a05946f8ea717fd59f03d20`  
		Last Modified: Wed, 10 Jun 2020 07:12:34 GMT  
		Size: 280.0 MB (279952956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99ec43ff140d74d9358b9d2fd63df5fce36b5098e46ef4b49d227f0364636c9`  
		Last Modified: Wed, 10 Jun 2020 07:12:20 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.0`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.0` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.0-scala_2.11`

```console
$ docker pull flink@sha256:0d99087637fc0c20b69bb7d547d60196ff25a3d3a62cd5154fa564e421e33867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.0-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:c1c970af17530762f6ce6c9c958768e4472854ca6409113ed374d4f283d5dcbc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436675025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f741681e25121ed784593ebecbed358aed80e1a260bfb002ad82fd47d2b6d339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:19:58 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:19:59 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:19:59 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:20:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:20:20 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:20:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:20:21 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:20:21 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00b32772b310b687204c982ca7877a4cee761832a9e8629e3690f6fea4b344`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940a9e818f8c710c7075528c886cd553354f101be46d1666257f49cbe0f4d756`  
		Last Modified: Tue, 07 Jul 2020 18:21:52 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7745517fb4443ffa66f663b418ee9f328579d9add78d437cbe0d369f9fa3993`  
		Last Modified: Tue, 07 Jul 2020 18:22:11 GMT  
		Size: 321.2 MB (321194389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7507a67edeb49577bc12ecc1a7bb0585eaa556c6037d960c51113c14cf1ce6a0`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.0-scala_2.12`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.0-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.11`

```console
$ docker pull flink@sha256:0d99087637fc0c20b69bb7d547d60196ff25a3d3a62cd5154fa564e421e33867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:c1c970af17530762f6ce6c9c958768e4472854ca6409113ed374d4f283d5dcbc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436675025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f741681e25121ed784593ebecbed358aed80e1a260bfb002ad82fd47d2b6d339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:19:58 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:19:59 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:19:59 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:20:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:20:20 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:20:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:20:21 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:20:21 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00b32772b310b687204c982ca7877a4cee761832a9e8629e3690f6fea4b344`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940a9e818f8c710c7075528c886cd553354f101be46d1666257f49cbe0f4d756`  
		Last Modified: Tue, 07 Jul 2020 18:21:52 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7745517fb4443ffa66f663b418ee9f328579d9add78d437cbe0d369f9fa3993`  
		Last Modified: Tue, 07 Jul 2020 18:22:11 GMT  
		Size: 321.2 MB (321194389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7507a67edeb49577bc12ecc1a7bb0585eaa556c6037d960c51113c14cf1ce6a0`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.12`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:latest`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:latest` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.11`

```console
$ docker pull flink@sha256:0d99087637fc0c20b69bb7d547d60196ff25a3d3a62cd5154fa564e421e33867
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:c1c970af17530762f6ce6c9c958768e4472854ca6409113ed374d4f283d5dcbc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.7 MB (436675025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f741681e25121ed784593ebecbed358aed80e1a260bfb002ad82fd47d2b6d339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.11.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:19:58 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:19:58 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:19:59 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:19:59 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:20:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:20:20 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:20:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:20:21 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:20:21 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00b32772b310b687204c982ca7877a4cee761832a9e8629e3690f6fea4b344`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940a9e818f8c710c7075528c886cd553354f101be46d1666257f49cbe0f4d756`  
		Last Modified: Tue, 07 Jul 2020 18:21:52 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7745517fb4443ffa66f663b418ee9f328579d9add78d437cbe0d369f9fa3993`  
		Last Modified: Tue, 07 Jul 2020 18:22:11 GMT  
		Size: 321.2 MB (321194389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7507a67edeb49577bc12ecc1a7bb0585eaa556c6037d960c51113c14cf1ce6a0`  
		Last Modified: Tue, 07 Jul 2020 18:21:51 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.12`

```console
$ docker pull flink@sha256:ece7938888a23685d82bf78bf220df56188f94e25b9b13720e83e802276f1fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:730c5c639a2bf838935cae7971ddc50396d83df53a626a58d32fc0b1412175f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.3 MB (427293324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7226aebb7c0d5c848668f045d4e78fda083525ce42d44f538e05db4438ea0560`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 16:38:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:38:02 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 09 Jun 2020 16:39:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:39:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_VERSION=8u252
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Tue, 09 Jun 2020 16:39:26 GMT
ENV JAVA_URL_VERSION=8u252b09
# Tue, 09 Jun 2020 16:39:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 10 Jun 2020 07:07:19 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 07:07:19 GMT
ENV GOSU_VERSION=1.11
# Wed, 10 Jun 2020 07:07:20 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.0/flink-1.11.0-bin-scala_2.12.tgz.asc GPG_KEY=2DA85B93244FDFA19A6244500653C0A2CEA00D0E CHECK_GPG=true
# Tue, 07 Jul 2020 18:20:27 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 07 Jul 2020 18:20:28 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 18:20:28 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 07 Jul 2020 18:20:29 GMT
WORKDIR /opt/flink
# Tue, 07 Jul 2020 18:21:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 07 Jul 2020 18:21:30 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Tue, 07 Jul 2020 18:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Jul 2020 18:21:30 GMT
EXPOSE 6123 8081
# Tue, 07 Jul 2020 18:21:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a79816c3e1e5cdd064948818bbd2dbf38783031aeca1474a9a9b50c2d8e5e8`  
		Last Modified: Tue, 09 Jun 2020 16:45:04 GMT  
		Size: 5.5 MB (5529317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cc5cb1b833b9fa2dd445b932781d8863c0d63f6be2b546720f9c84599f56e`  
		Last Modified: Tue, 09 Jun 2020 16:46:49 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe2ea267c0c8cdd63751f91ef61f6acd2b6b6b72213118d58fd09dc2b6b49`  
		Last Modified: Tue, 09 Jun 2020 16:46:58 GMT  
		Size: 40.3 MB (40315760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff61193e0caad5af317650d5e0a80393ef07e9822cb2732ea52d712ac9a44a5`  
		Last Modified: Wed, 10 Jun 2020 07:11:13 GMT  
		Size: 531.0 KB (531048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0a599554406a47057c9b9e2770460426df97fc3203c0d3ba6a899dcb723c41`  
		Last Modified: Wed, 10 Jun 2020 07:11:12 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d33cd6f4f12932bfa75453fa7641fbc74bc3f8707e4e143cb402d1ff240ca`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a1b46e40f7d2c5ed5ee458e7dee010838c7a0249cbed62c077c47db71ee8d8`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc9f0dd070395d13f80e53afa01fdfbce879a92259b39b4a954517c3f1a633d`  
		Last Modified: Tue, 07 Jul 2020 18:22:34 GMT  
		Size: 311.8 MB (311812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c9d9c21c8ffd522a5f5ab69765aa8a2b8b8617138902111f3854c433f7a83`  
		Last Modified: Tue, 07 Jul 2020 18:22:17 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
