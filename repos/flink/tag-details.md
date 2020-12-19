<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `flink`

-	[`flink:1.10`](#flink110)
-	[`flink:1.10.2`](#flink1102)
-	[`flink:1.10.2-scala_2.11`](#flink1102-scala_211)
-	[`flink:1.10.2-scala_2.12`](#flink1102-scala_212)
-	[`flink:1.10-scala_2.11`](#flink110-scala_211)
-	[`flink:1.10-scala_2.12`](#flink110-scala_212)
-	[`flink:1.11`](#flink111)
-	[`flink:1.11.3`](#flink1113)
-	[`flink:1.11.3-java11`](#flink1113-java11)
-	[`flink:1.11.3-java8`](#flink1113-java8)
-	[`flink:1.11.3-scala_2.11`](#flink1113-scala_211)
-	[`flink:1.11.3-scala_2.11-java11`](#flink1113-scala_211-java11)
-	[`flink:1.11.3-scala_2.11-java8`](#flink1113-scala_211-java8)
-	[`flink:1.11.3-scala_2.12`](#flink1113-scala_212)
-	[`flink:1.11.3-scala_2.12-java11`](#flink1113-scala_212-java11)
-	[`flink:1.11.3-scala_2.12-java8`](#flink1113-scala_212-java8)
-	[`flink:1.11-java11`](#flink111-java11)
-	[`flink:1.11-java8`](#flink111-java8)
-	[`flink:1.11-scala_2.11`](#flink111-scala_211)
-	[`flink:1.11-scala_2.11-java11`](#flink111-scala_211-java11)
-	[`flink:1.11-scala_2.11-java8`](#flink111-scala_211-java8)
-	[`flink:1.11-scala_2.12`](#flink111-scala_212)
-	[`flink:1.11-scala_2.12-java11`](#flink111-scala_212-java11)
-	[`flink:1.11-scala_2.12-java8`](#flink111-scala_212-java8)

## `flink:1.10`

```console
$ docker pull flink@sha256:c6ee4be967ca86d8d99bdfc18fcaf84bbd18bf7a23c389919bfb9afdc1cb084b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10` - linux; amd64

```console
$ docker pull flink@sha256:b3c67697b022518d7883c750d9b80085ae5146ee5fd77932c6e8dc2e263e1cf6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396696411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eafb4efa8034de7d1810d902ea4847094930b19317211b9f6c95fcc6334cb9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:46:33 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:46:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:46:34 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:01 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:01 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:02 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:02 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57212cf7bba3d7f400712ed99da7632ccdbf368a3cf9a7419b76db8582365083`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5ad4475dafc4ceab5fc0e544de9d6d28fdb1d304f58af2fd36882c0d7b7bc`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c53333ce4f79cbaac4364c019626d7fdde7fa2d9ff27c241327a324afe63637`  
		Last Modified: Fri, 11 Sep 2020 04:49:44 GMT  
		Size: 281.2 MB (281190205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d05ccc3c14bd8df7e6387889e3e53834c60bd52f94569cd5ed144913e7452`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.2`

```console
$ docker pull flink@sha256:c6ee4be967ca86d8d99bdfc18fcaf84bbd18bf7a23c389919bfb9afdc1cb084b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.2` - linux; amd64

```console
$ docker pull flink@sha256:b3c67697b022518d7883c750d9b80085ae5146ee5fd77932c6e8dc2e263e1cf6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396696411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eafb4efa8034de7d1810d902ea4847094930b19317211b9f6c95fcc6334cb9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:46:33 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:46:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:46:34 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:01 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:01 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:02 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:02 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57212cf7bba3d7f400712ed99da7632ccdbf368a3cf9a7419b76db8582365083`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5ad4475dafc4ceab5fc0e544de9d6d28fdb1d304f58af2fd36882c0d7b7bc`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c53333ce4f79cbaac4364c019626d7fdde7fa2d9ff27c241327a324afe63637`  
		Last Modified: Fri, 11 Sep 2020 04:49:44 GMT  
		Size: 281.2 MB (281190205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d05ccc3c14bd8df7e6387889e3e53834c60bd52f94569cd5ed144913e7452`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.2-scala_2.11`

```console
$ docker pull flink@sha256:0c9f448249e0ceb331ed4ea0c368b843f3f3d940ae9eaab23b195b301492546d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.2-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:77f2af67da0b9ca9a6b69d6f8d5259df598a49339e78ec084ff36707a3db7317
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.0 MB (405988064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c8c9b966c51d16d4629fd4de8206816679a133e9cc32c180567e41b2d8bc4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:47:07 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.11.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:47:07 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:47:07 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:47:08 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:47:08 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:26 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:26 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:27 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:27 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777ee5505a72d04496dbb2d3b776b2877c21ef54112a8a1ea35870716e4be12b`  
		Last Modified: Fri, 11 Sep 2020 04:49:53 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0af3679def1d9983914fd173cb884d890d388e3cd90ebeb5bb7ded929673cf7`  
		Last Modified: Fri, 11 Sep 2020 04:49:52 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ef95fc0cdaa2ae092cb7b5193b020d9325fe0f9edb8933115d87123b893c5f`  
		Last Modified: Fri, 11 Sep 2020 04:50:08 GMT  
		Size: 290.5 MB (290481858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb1be3dddbe8a3f30c6d63574e63d75245dcc3751a107b694df8a7b010cb77`  
		Last Modified: Fri, 11 Sep 2020 04:49:53 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10.2-scala_2.12`

```console
$ docker pull flink@sha256:c6ee4be967ca86d8d99bdfc18fcaf84bbd18bf7a23c389919bfb9afdc1cb084b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10.2-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:b3c67697b022518d7883c750d9b80085ae5146ee5fd77932c6e8dc2e263e1cf6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396696411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eafb4efa8034de7d1810d902ea4847094930b19317211b9f6c95fcc6334cb9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:46:33 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:46:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:46:34 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:01 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:01 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:02 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:02 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57212cf7bba3d7f400712ed99da7632ccdbf368a3cf9a7419b76db8582365083`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5ad4475dafc4ceab5fc0e544de9d6d28fdb1d304f58af2fd36882c0d7b7bc`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c53333ce4f79cbaac4364c019626d7fdde7fa2d9ff27c241327a324afe63637`  
		Last Modified: Fri, 11 Sep 2020 04:49:44 GMT  
		Size: 281.2 MB (281190205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d05ccc3c14bd8df7e6387889e3e53834c60bd52f94569cd5ed144913e7452`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10-scala_2.11`

```console
$ docker pull flink@sha256:0c9f448249e0ceb331ed4ea0c368b843f3f3d940ae9eaab23b195b301492546d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:77f2af67da0b9ca9a6b69d6f8d5259df598a49339e78ec084ff36707a3db7317
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.0 MB (405988064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c8c9b966c51d16d4629fd4de8206816679a133e9cc32c180567e41b2d8bc4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:47:07 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.11.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:47:07 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:47:07 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:47:08 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:47:08 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:26 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:26 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:27 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:27 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777ee5505a72d04496dbb2d3b776b2877c21ef54112a8a1ea35870716e4be12b`  
		Last Modified: Fri, 11 Sep 2020 04:49:53 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0af3679def1d9983914fd173cb884d890d388e3cd90ebeb5bb7ded929673cf7`  
		Last Modified: Fri, 11 Sep 2020 04:49:52 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ef95fc0cdaa2ae092cb7b5193b020d9325fe0f9edb8933115d87123b893c5f`  
		Last Modified: Fri, 11 Sep 2020 04:50:08 GMT  
		Size: 290.5 MB (290481858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb1be3dddbe8a3f30c6d63574e63d75245dcc3751a107b694df8a7b010cb77`  
		Last Modified: Fri, 11 Sep 2020 04:49:53 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.10-scala_2.12`

```console
$ docker pull flink@sha256:c6ee4be967ca86d8d99bdfc18fcaf84bbd18bf7a23c389919bfb9afdc1cb084b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.10-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:b3c67697b022518d7883c750d9b80085ae5146ee5fd77932c6e8dc2e263e1cf6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396696411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eafb4efa8034de7d1810d902ea4847094930b19317211b9f6c95fcc6334cb9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 07:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:04:51 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 07:06:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 10 Sep 2020 07:06:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 07:06:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 10 Sep 2020 07:06:16 GMT
ENV JAVA_VERSION=8u265
# Thu, 10 Sep 2020 07:06:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 11 Sep 2020 04:39:48 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Fri, 11 Sep 2020 04:39:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 11 Sep 2020 04:39:50 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.10.2/flink-1.10.2-bin-scala_2.12.tgz.asc GPG_KEY=C63E230EFFF519A5BBF2C9AE6767487CD505859C CHECK_GPG=true
# Fri, 11 Sep 2020 04:46:32 GMT
ENV FLINK_HOME=/opt/flink
# Fri, 11 Sep 2020 04:46:33 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 04:46:33 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Fri, 11 Sep 2020 04:46:34 GMT
WORKDIR /opt/flink
# Fri, 11 Sep 2020 04:47:01 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Fri, 11 Sep 2020 04:47:01 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Fri, 11 Sep 2020 04:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Sep 2020 04:47:02 GMT
EXPOSE 6123 8081
# Fri, 11 Sep 2020 04:47:02 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9777c2d5c29a7fd4b5c4efe0fa2ad6176ca9c5430163ca0c620d94eca56baae`  
		Last Modified: Thu, 10 Sep 2020 07:13:52 GMT  
		Size: 5.5 MB (5529417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9248106993db7bc5baf0074c4304fce24d8101cc2046349605cdc01be0d3a92a`  
		Last Modified: Thu, 10 Sep 2020 07:15:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f74ab5b5b3ee2a4b98345c100cb380be8b776c69c9f3f92b9a1170d3227ce92`  
		Last Modified: Thu, 10 Sep 2020 07:15:33 GMT  
		Size: 40.3 MB (40334785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ec319497407f530849074f16a373c8a94499623c409fbbbfbb750f15e2e47f`  
		Last Modified: Fri, 11 Sep 2020 04:47:48 GMT  
		Size: 531.1 KB (531074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66f47ca7e4db1dbb44a4105fdb65753ece62c8b0b454faf905f4fea4d3b9e4`  
		Last Modified: Fri, 11 Sep 2020 04:47:47 GMT  
		Size: 900.5 KB (900515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57212cf7bba3d7f400712ed99da7632ccdbf368a3cf9a7419b76db8582365083`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a5ad4475dafc4ceab5fc0e544de9d6d28fdb1d304f58af2fd36882c0d7b7bc`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c53333ce4f79cbaac4364c019626d7fdde7fa2d9ff27c241327a324afe63637`  
		Last Modified: Fri, 11 Sep 2020 04:49:44 GMT  
		Size: 281.2 MB (281190205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d05ccc3c14bd8df7e6387889e3e53834c60bd52f94569cd5ed144913e7452`  
		Last Modified: Fri, 11 Sep 2020 04:49:29 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-java11`

```console
$ docker pull flink@sha256:6276b278217017a65b3632d521e6f293065f055945b178e3e85168695271c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-java11` - linux; amd64

```console
$ docker pull flink@sha256:a02e5e8336c275da924769499862f4bd8049d827e7bc8b6ca62a399acb6f4be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.8 MB (426809826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0787fcd6113a7d3062473840c90f10b1af71260d7768393c858615ea24dc4b6b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:13 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:15 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:48 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:48 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:49 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:49 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab288ad208a698f88d3a3ceae960e8ffdd51ef3a979b6edc689731e7816f1a1b`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 4.6 KB (4609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ad24dd4401cf5c4c55068bad3f8ea6b139a0212372f37c3a7d547e93c5f7fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:43 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef83e8841a33e61d0e378326d55cbf4b915d799e569577bb57e56cda598f1`  
		Last Modified: Sat, 19 Dec 2020 01:30:00 GMT  
		Size: 309.5 MB (309509151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedfaa733a8d4d46bc40ee2b5a5f821d6459dcba08de49d1aea41ca985a00ff`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-java8`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-java8` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.11`

```console
$ docker pull flink@sha256:d21e46232183324a1ca9bb8790097448fab4d697f5919382d183528aed197068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:fc30e623a42027647d4d6a5c5b96643f6b26f3eac71336759bd9b6ea32a312e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.4 MB (435367619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c27efc2392a3eb764fde2659dba2f8c4180f9398a7c81b0a325793a2d549b9d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:20:40 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:20:41 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:20:41 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:03 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:04 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d002a6600a11f9d1c454d5293db79ee24187f8889428b7c24af1340ef9d40`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a51ae47c862eb03fb9e04fde1490ffda6b6719397dad6af0dffd73fd60379b`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170c9e5ac01e4eb99a79d6839d76e16b59e3357b8b98d75fc497d4520e8fc7c6`  
		Last Modified: Sat, 19 Dec 2020 01:29:34 GMT  
		Size: 318.9 MB (318892160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e985d0eda4f59f6f657a51300a6be87218b008c7f6672765528d1064d5936`  
		Last Modified: Sat, 19 Dec 2020 01:29:17 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.11-java11`

```console
$ docker pull flink@sha256:1220a80ba9a12e71ec10973d59802382f7ca175b9d33e59869245d882f86da0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:3e4827be85be8f8b896302eaed59ef96e8f31b431d36eab5e6e5c70b7f19b880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.2 MB (436192844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f18672721716103ead86e85dae7bd3361df0e93bcf749a1a8dad91147eef1a1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:19:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:19:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:19:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:19:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:19:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:20:28 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:20:28 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:20:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:20:29 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:20:29 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ab7b9138b6f07f3699d9d7d810d1eed4765d56d36e1187146fcf594d2aef6a`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b4a5473c7d516f55647a108dcad11fc9bf684bcc1cdccebca10c0d1122f4c`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ec06225d071e2e5a96ce2ce97d8b5f8f6ecf75f0219f01e28f1aa9d2257fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:09 GMT  
		Size: 318.9 MB (318892170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c3cca4e04426b7d595f040d3442a302cefc6d1363cc637b61d5b1fef9c8202`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.11-java8`

```console
$ docker pull flink@sha256:d21e46232183324a1ca9bb8790097448fab4d697f5919382d183528aed197068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:fc30e623a42027647d4d6a5c5b96643f6b26f3eac71336759bd9b6ea32a312e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.4 MB (435367619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c27efc2392a3eb764fde2659dba2f8c4180f9398a7c81b0a325793a2d549b9d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:20:40 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:20:41 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:20:41 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:03 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:04 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d002a6600a11f9d1c454d5293db79ee24187f8889428b7c24af1340ef9d40`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a51ae47c862eb03fb9e04fde1490ffda6b6719397dad6af0dffd73fd60379b`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170c9e5ac01e4eb99a79d6839d76e16b59e3357b8b98d75fc497d4520e8fc7c6`  
		Last Modified: Sat, 19 Dec 2020 01:29:34 GMT  
		Size: 318.9 MB (318892160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e985d0eda4f59f6f657a51300a6be87218b008c7f6672765528d1064d5936`  
		Last Modified: Sat, 19 Dec 2020 01:29:17 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.12`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.12-java11`

```console
$ docker pull flink@sha256:6276b278217017a65b3632d521e6f293065f055945b178e3e85168695271c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:a02e5e8336c275da924769499862f4bd8049d827e7bc8b6ca62a399acb6f4be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.8 MB (426809826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0787fcd6113a7d3062473840c90f10b1af71260d7768393c858615ea24dc4b6b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:13 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:15 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:48 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:48 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:49 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:49 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab288ad208a698f88d3a3ceae960e8ffdd51ef3a979b6edc689731e7816f1a1b`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 4.6 KB (4609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ad24dd4401cf5c4c55068bad3f8ea6b139a0212372f37c3a7d547e93c5f7fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:43 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef83e8841a33e61d0e378326d55cbf4b915d799e569577bb57e56cda598f1`  
		Last Modified: Sat, 19 Dec 2020 01:30:00 GMT  
		Size: 309.5 MB (309509151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedfaa733a8d4d46bc40ee2b5a5f821d6459dcba08de49d1aea41ca985a00ff`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11.3-scala_2.12-java8`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11.3-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-java11`

```console
$ docker pull flink@sha256:6276b278217017a65b3632d521e6f293065f055945b178e3e85168695271c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:a02e5e8336c275da924769499862f4bd8049d827e7bc8b6ca62a399acb6f4be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.8 MB (426809826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0787fcd6113a7d3062473840c90f10b1af71260d7768393c858615ea24dc4b6b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:13 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:15 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:48 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:48 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:49 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:49 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab288ad208a698f88d3a3ceae960e8ffdd51ef3a979b6edc689731e7816f1a1b`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 4.6 KB (4609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ad24dd4401cf5c4c55068bad3f8ea6b139a0212372f37c3a7d547e93c5f7fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:43 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef83e8841a33e61d0e378326d55cbf4b915d799e569577bb57e56cda598f1`  
		Last Modified: Sat, 19 Dec 2020 01:30:00 GMT  
		Size: 309.5 MB (309509151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedfaa733a8d4d46bc40ee2b5a5f821d6459dcba08de49d1aea41ca985a00ff`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-java8`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.11`

```console
$ docker pull flink@sha256:d21e46232183324a1ca9bb8790097448fab4d697f5919382d183528aed197068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:fc30e623a42027647d4d6a5c5b96643f6b26f3eac71336759bd9b6ea32a312e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.4 MB (435367619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c27efc2392a3eb764fde2659dba2f8c4180f9398a7c81b0a325793a2d549b9d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:20:40 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:20:41 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:20:41 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:03 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:04 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d002a6600a11f9d1c454d5293db79ee24187f8889428b7c24af1340ef9d40`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a51ae47c862eb03fb9e04fde1490ffda6b6719397dad6af0dffd73fd60379b`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170c9e5ac01e4eb99a79d6839d76e16b59e3357b8b98d75fc497d4520e8fc7c6`  
		Last Modified: Sat, 19 Dec 2020 01:29:34 GMT  
		Size: 318.9 MB (318892160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e985d0eda4f59f6f657a51300a6be87218b008c7f6672765528d1064d5936`  
		Last Modified: Sat, 19 Dec 2020 01:29:17 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.11-java11`

```console
$ docker pull flink@sha256:1220a80ba9a12e71ec10973d59802382f7ca175b9d33e59869245d882f86da0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:3e4827be85be8f8b896302eaed59ef96e8f31b431d36eab5e6e5c70b7f19b880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.2 MB (436192844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f18672721716103ead86e85dae7bd3361df0e93bcf749a1a8dad91147eef1a1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:19:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:19:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:19:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:19:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:19:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:20:28 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:20:28 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:20:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:20:29 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:20:29 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ab7b9138b6f07f3699d9d7d810d1eed4765d56d36e1187146fcf594d2aef6a`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b4a5473c7d516f55647a108dcad11fc9bf684bcc1cdccebca10c0d1122f4c`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ec06225d071e2e5a96ce2ce97d8b5f8f6ecf75f0219f01e28f1aa9d2257fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:09 GMT  
		Size: 318.9 MB (318892170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c3cca4e04426b7d595f040d3442a302cefc6d1363cc637b61d5b1fef9c8202`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.11-java8`

```console
$ docker pull flink@sha256:d21e46232183324a1ca9bb8790097448fab4d697f5919382d183528aed197068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:fc30e623a42027647d4d6a5c5b96643f6b26f3eac71336759bd9b6ea32a312e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.4 MB (435367619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c27efc2392a3eb764fde2659dba2f8c4180f9398a7c81b0a325793a2d549b9d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.11.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:20:40 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:20:40 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:20:41 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:20:41 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:03 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:04 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d002a6600a11f9d1c454d5293db79ee24187f8889428b7c24af1340ef9d40`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 4.6 KB (4606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a51ae47c862eb03fb9e04fde1490ffda6b6719397dad6af0dffd73fd60379b`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170c9e5ac01e4eb99a79d6839d76e16b59e3357b8b98d75fc497d4520e8fc7c6`  
		Last Modified: Sat, 19 Dec 2020 01:29:34 GMT  
		Size: 318.9 MB (318892160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1e985d0eda4f59f6f657a51300a6be87218b008c7f6672765528d1064d5936`  
		Last Modified: Sat, 19 Dec 2020 01:29:17 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.12`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.12-java11`

```console
$ docker pull flink@sha256:6276b278217017a65b3632d521e6f293065f055945b178e3e85168695271c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:a02e5e8336c275da924769499862f4bd8049d827e7bc8b6ca62a399acb6f4be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.8 MB (426809826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0787fcd6113a7d3062473840c90f10b1af71260d7768393c858615ea24dc4b6b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:51:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 18 Dec 2020 04:51:55 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:51:56 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:51:56 GMT
ENV JAVA_VERSION=11.0.9.1
# Fri, 18 Dec 2020 04:52:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jre_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sat, 19 Dec 2020 01:19:51 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:19:52 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:19:53 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:13 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:13 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:15 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:21:48 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:21:48 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:21:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:21:49 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:21:49 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d2caa1e13fb5df4906bc20241449d7d115741c4c33cbe0337340bb7531209`  
		Last Modified: Fri, 18 Dec 2020 04:57:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cfa5e23220e25fa0c3290bc0f6fc757b639f0a5b4c09c00c794b50d92090e7`  
		Last Modified: Fri, 18 Dec 2020 04:57:47 GMT  
		Size: 42.1 MB (42126682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5cbd8321236a6832c8d0aafe6010d51d712dcdc0baa16386c8cfb8d45a04d9`  
		Last Modified: Sat, 19 Dec 2020 01:28:53 GMT  
		Size: 531.2 KB (531175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc4974c779d9636c535f4b4602b11032b40920e1ee2fcfd38d2de00978bea0d`  
		Last Modified: Sat, 19 Dec 2020 01:28:51 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab288ad208a698f88d3a3ceae960e8ffdd51ef3a979b6edc689731e7816f1a1b`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 4.6 KB (4609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ad24dd4401cf5c4c55068bad3f8ea6b139a0212372f37c3a7d547e93c5f7fa`  
		Last Modified: Sat, 19 Dec 2020 01:29:43 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aef83e8841a33e61d0e378326d55cbf4b915d799e569577bb57e56cda598f1`  
		Last Modified: Sat, 19 Dec 2020 01:30:00 GMT  
		Size: 309.5 MB (309509151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedfaa733a8d4d46bc40ee2b5a5f821d6459dcba08de49d1aea41ca985a00ff`  
		Last Modified: Sat, 19 Dec 2020 01:29:42 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.11-scala_2.12-java8`

```console
$ docker pull flink@sha256:82e04ef668d2b91e970fef00db92891aed64af2d5187eb9c4638150316c3d882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `flink:1.11-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:325df14ada99b5e32d97754d45d24937bfac3b678ca0a279fd19656d0a735b65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.0 MB (425984569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5001f234db8672070effb752794a38e60147bb0eb3d7e26fdd5a22c302a8fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Dec 2020 04:51:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Dec 2020 04:51:54 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 18 Dec 2020 04:52:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:52:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 18 Dec 2020 04:52:29 GMT
ENV JAVA_VERSION=8u275
# Fri, 18 Dec 2020 04:52:33 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_linux_8u275b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Dec 2020 01:20:38 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base;   rm -rf /var/lib/apt/lists/*
# Sat, 19 Dec 2020 01:20:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 19 Dec 2020 01:20:39 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Sat, 19 Dec 2020 01:21:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.11.3/flink-1.11.3-bin-scala_2.12.tgz.asc GPG_KEY=F8E419AA0B60C28879E876859DFF40967ABFC5A4 CHECK_GPG=true
# Sat, 19 Dec 2020 01:21:54 GMT
ENV FLINK_HOME=/opt/flink
# Sat, 19 Dec 2020 01:21:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Dec 2020 01:21:55 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Sat, 19 Dec 2020 01:21:55 GMT
WORKDIR /opt/flink
# Sat, 19 Dec 2020 01:27:43 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Sat, 19 Dec 2020 01:27:43 GMT
COPY file:5118b9265b7774ef32131b2cbf42fd9bf26c640be3ebb42b4972a3ae8ed5125e in / 
# Sat, 19 Dec 2020 01:27:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 19 Dec 2020 01:27:44 GMT
EXPOSE 6123 8081
# Sat, 19 Dec 2020 01:27:44 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e99843d3bcab27c3a36aa6cc7d0d7f1282ecdadeb1f186f69e53f15c0263e`  
		Last Modified: Fri, 18 Dec 2020 04:57:41 GMT  
		Size: 5.5 MB (5529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7eeb2d7da8b5545cadd3ce94df315cd84389b225bbdb477d89bcca374051c`  
		Last Modified: Fri, 18 Dec 2020 04:58:28 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8832bda5b3e9729f02d98d5b2e762990c5c13cae3f1308f142b75510578ae851`  
		Last Modified: Fri, 18 Dec 2020 04:58:35 GMT  
		Size: 41.3 MB (41301526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a64047c53e156fdec8b7dd36e788deacbcb03cb9015de2c6c45ebe4eafb43`  
		Last Modified: Sat, 19 Dec 2020 01:29:18 GMT  
		Size: 531.1 KB (531117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bad2f332174dae953d968755a3100ab86c28284a353d1d567bac9648b3119f`  
		Last Modified: Sat, 19 Dec 2020 01:29:16 GMT  
		Size: 900.5 KB (900512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77f011798d86eaec1b66ff80e1d527d33c49ec79c47b762a87ab0beac370523`  
		Last Modified: Sat, 19 Dec 2020 01:30:10 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f996af57b1190a7ef78c7c71da50a2900836e34a38725377f98ee51b7776588`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9730bcb83c48a0282f79cdc7690b24e3ba4dbe68f8a0e045bdf78c1b762b3a1f`  
		Last Modified: Sat, 19 Dec 2020 01:30:26 GMT  
		Size: 309.5 MB (309509109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5b814e9f7d7c0b5abbaf93088708b1d77f897ae8ac486ab9b1a5cd53bb54d`  
		Last Modified: Sat, 19 Dec 2020 01:30:09 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
