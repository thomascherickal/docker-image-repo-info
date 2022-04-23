<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cassandra`

-	[`cassandra:3`](#cassandra3)
-	[`cassandra:3.0`](#cassandra30)
-	[`cassandra:3.0.26`](#cassandra3026)
-	[`cassandra:3.11`](#cassandra311)
-	[`cassandra:3.11.12`](#cassandra31112)
-	[`cassandra:4`](#cassandra4)
-	[`cassandra:4.0`](#cassandra40)
-	[`cassandra:4.0.3`](#cassandra403)
-	[`cassandra:latest`](#cassandralatest)

## `cassandra:3`

```console
$ docker pull cassandra@sha256:2d796a23dd37295675fd71fa273b7ec365da68609f5d381abafcf3b5ebda0800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:3` - linux; amd64

```console
$ docker pull cassandra@sha256:7b4b4239970f21ccbe1fd5bd3ab062e008ca4ed45b516ae9447ccb0bb6519427
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129688132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2475f0fb7aaf3aec7dda8a9fa416e88cf9d91a96db02e4d74024bef7997853aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:04:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:04:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:04:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:50:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:52 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:53 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:51:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:51:08 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:51:08 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:51:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:51:09 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:51:09 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b1157d6084a2ea36096688a243ea6d05fc59b44b2331626849535196db689`  
		Last Modified: Fri, 22 Apr 2022 02:08:41 GMT  
		Size: 41.8 MB (41773808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94201e8045a2b75849b87376763eb19cd1ec004669a3d4821923f64259838bf`  
		Last Modified: Fri, 22 Apr 2022 02:08:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ea050078a67a35d2f11b500aa75b78bf0d6d85f91f14280a49c4a67c7fdc4`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609edbe68ee0c662e37d045a9ead6e3615bf900df2fdbc019d6f3f81d42e68e2`  
		Last Modified: Fri, 22 Apr 2022 08:52:08 GMT  
		Size: 9.5 MB (9520679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0b03034f96bab865bed901a6ffa503f19aa9170f1b72ad4eb7a74b54a4ac2`  
		Last Modified: Fri, 22 Apr 2022 08:52:07 GMT  
		Size: 1.3 MB (1316224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12f39ee7b906538ae17814627b38c201fd4cb40428565f73f4e72dd15dc6ef2`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 32.5 MB (32478053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3ff5172576b28266e0f4e8a2f14212bd0d4b9633c05e5e69754c26af2157b1`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da93bf58be51fe2b7584378d92f35f646a11623578698d53f9cc6a07f2018497`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:6dbd335e172d9c892580b3f129e9dea641f665c72e22e2ccb4cb0a49379dd559
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121137212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ddce1eae8230f1c6fbf15c3b73cc5558492a62eb65a2e204591b524141ab9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:17:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 23 Apr 2022 00:18:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:18:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:18:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 23 Apr 2022 06:52:34 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:52:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:52:54 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:53:14 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:53:15 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_VERSION=3.11.12
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Sat, 23 Apr 2022 06:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:53:46 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:53:46 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:53:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 23 Apr 2022 06:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:53:49 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:53:49 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b77390aa7e68829cfed8e84ca110bf8df1b62d07074bc4d3548e3b5a74837d`  
		Last Modified: Sat, 23 Apr 2022 00:27:24 GMT  
		Size: 39.5 MB (39508183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263bee161abb30a7eb910dfbbcfeb506170b373e07866388acb3647c3474e2d2`  
		Last Modified: Sat, 23 Apr 2022 00:27:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e95e7ee9157d74a18ed84c37a1b47f2625b8929778ee979293eaf5e073f97c`  
		Last Modified: Sat, 23 Apr 2022 06:56:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe4bbcbaa326c450337285613afdb3c8806fc8093778b4ba44d1e7cb3d12ae5`  
		Last Modified: Sat, 23 Apr 2022 06:56:17 GMT  
		Size: 8.9 MB (8900042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb14a5abcd9c1a92954d4da43bd1ed6d28ef179f47e49169fac4396e7b875e6d`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.3 MB (1270567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d708a7a3eb94c16aebce0d43acbcfe31c42f6dc907b9269c4bf02874bd4ab`  
		Last Modified: Sat, 23 Apr 2022 06:56:20 GMT  
		Size: 32.5 MB (32479942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d35607fb75fa026ebb07e465271ba0f21610d3de998fdb558a93e0b4fb626`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9ec8908d382740f1f1dd4520a14e4dab56e577b57763f1076c6ca1cda789f`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:31e240593eacecc2ae00f6a43f1209666c03e9cd372308587861e2ce4bc58b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126636878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc572898ab769ed4a42507072bc3d236e4d558563dae4412735fbf4a5e0a7c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:56:47 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:57:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:13:53 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:14:05 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:14:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:14:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:14:18 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:14:19 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:14:20 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:14:21 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:14:22 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:14:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:14:41 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:14:43 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:14:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:14:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:14:45 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:14:46 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241f218f4a9078a7dcbfc6fd6ed6877e46407b06b6221bc6206fab8af4c590b`  
		Last Modified: Fri, 22 Apr 2022 03:02:34 GMT  
		Size: 40.8 MB (40769834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3678ae378db153e8948d4ba589775345c50a90226740a49251dc8d98ee1ee6`  
		Last Modified: Fri, 22 Apr 2022 03:02:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcef3dfa8c549587028ddd3ff56002acc6fd571241dcd3e972d9343f1f5432`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90633b62b6e047a653abd913ae534c7a42aff79d96a012b69228446cec99fbfe`  
		Last Modified: Fri, 22 Apr 2022 08:16:12 GMT  
		Size: 9.6 MB (9550979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a6a6163139adc28bea3b154833e3d680c71f4ea7394be5f419c7e06c26eb0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.0 MB (1011031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceeb37adb1964398af2632b3de91c825a726badfc7175dc976a03e686df923d`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 32.2 MB (32236813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5582bb4dde880d1ea624a6dd47791f3807466941636befcdb69446e91e72a0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4a16bb56f8c1b161724cceeb1d2c334534d8042d016e8f0fc56664bbf9c3bc`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b7874b6138dc94865d6655e055e9b330414f87d5ebdb65a508dbe939361c698c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135686031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cee2a594026059e4161ae3507c7db2085a52fa19c5c16965e98ece6f0640af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:47:03 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 09:47:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:48:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:48:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 15:58:58 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 16:00:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 16:00:36 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 16:00:38 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 16:00:40 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 16:00:41 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 16:00:43 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 16:00:46 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 16:01:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 16:01:38 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 16:01:41 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 16:01:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 16:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:01:52 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 16:01:53 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc4da81b86f2d794067f5074f224a2816851960275189b2d3c178608853518`  
		Last Modified: Fri, 22 Apr 2022 09:58:55 GMT  
		Size: 41.2 MB (41162345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15824a78c37261d06cbabfff12b54690edcb179cce082b71f20b44471365c8`  
		Last Modified: Fri, 22 Apr 2022 09:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e184c002e7628b8689deb98ed5547310b9951736d421a5594701f0211bd826`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f04cbe05e83893ff0786818415db712edfee149c001723975b4fc6af9f4076`  
		Last Modified: Fri, 22 Apr 2022 16:04:33 GMT  
		Size: 10.3 MB (10310111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7690d4477b275d4157e369fe0d406e41dae39c995e0f10758abfc646ab9256`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 MB (1236781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b48765bc741bd95e551b022969d8c2fcadba3ad4f7c5f5dae01c761b59b837`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 32.5 MB (32478886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fc9ee9f9c0a0f4b7c5c4f826289ac5d97d2c39c859a866fe0919a74ec20cbe`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf83277e0853e4733bd15816971fc969409d794c8f0ae135e1b1b052fcb508`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.0`

```console
$ docker pull cassandra@sha256:2370e4dffd0ddee9bfc816b8dac863ed2828b2b6d2196f90ae1b346910638568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:3.0` - linux; amd64

```console
$ docker pull cassandra@sha256:5535de3aa0166f767a6e57b8f376323382cb11005b2e689ac60cc4c282714f6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124386720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9238ebd57db75d9798232f2497172ce7a0711bb899389b57976f1fa85ad45338`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:04:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:04:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:04:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:50:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:52 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:53 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:51:12 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 08:51:12 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 08:51:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:51:30 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:51:30 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:51:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:51:30 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:51:30 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b1157d6084a2ea36096688a243ea6d05fc59b44b2331626849535196db689`  
		Last Modified: Fri, 22 Apr 2022 02:08:41 GMT  
		Size: 41.8 MB (41773808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94201e8045a2b75849b87376763eb19cd1ec004669a3d4821923f64259838bf`  
		Last Modified: Fri, 22 Apr 2022 02:08:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ea050078a67a35d2f11b500aa75b78bf0d6d85f91f14280a49c4a67c7fdc4`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609edbe68ee0c662e37d045a9ead6e3615bf900df2fdbc019d6f3f81d42e68e2`  
		Last Modified: Fri, 22 Apr 2022 08:52:08 GMT  
		Size: 9.5 MB (9520679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0b03034f96bab865bed901a6ffa503f19aa9170f1b72ad4eb7a74b54a4ac2`  
		Last Modified: Fri, 22 Apr 2022 08:52:07 GMT  
		Size: 1.3 MB (1316224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41569460a89754a6e114eb26476c80288c6c76ab8de78509276cf1acb3b14427`  
		Last Modified: Fri, 22 Apr 2022 08:52:23 GMT  
		Size: 27.2 MB (27176638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3a452c0ca1b3d13e157d207d18ab54cf58c864be3979b0ab111db2f08927d6`  
		Last Modified: Fri, 22 Apr 2022 08:52:21 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b04ba31b9bdae2bf4e20bebdcd6898ebb578d786665e904d143e86b51713bd6`  
		Last Modified: Fri, 22 Apr 2022 08:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:461a512825cc8aa961de9dd109d10dda19579497ee2fb10efe102a707c973ebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115835949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2010bb920ffa9c676b298ab44c0b687004f24d439f7e481000d0ba40e6a424c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:17:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 23 Apr 2022 00:18:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:18:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:18:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 23 Apr 2022 06:52:34 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:52:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:52:54 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:53:14 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:53:15 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:54:07 GMT
ENV CASSANDRA_VERSION=3.0.26
# Sat, 23 Apr 2022 06:54:07 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Sat, 23 Apr 2022 06:54:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:54:39 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:54:40 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:54:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 23 Apr 2022 06:54:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:54:42 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:54:42 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b77390aa7e68829cfed8e84ca110bf8df1b62d07074bc4d3548e3b5a74837d`  
		Last Modified: Sat, 23 Apr 2022 00:27:24 GMT  
		Size: 39.5 MB (39508183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263bee161abb30a7eb910dfbbcfeb506170b373e07866388acb3647c3474e2d2`  
		Last Modified: Sat, 23 Apr 2022 00:27:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e95e7ee9157d74a18ed84c37a1b47f2625b8929778ee979293eaf5e073f97c`  
		Last Modified: Sat, 23 Apr 2022 06:56:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe4bbcbaa326c450337285613afdb3c8806fc8093778b4ba44d1e7cb3d12ae5`  
		Last Modified: Sat, 23 Apr 2022 06:56:17 GMT  
		Size: 8.9 MB (8900042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb14a5abcd9c1a92954d4da43bd1ed6d28ef179f47e49169fac4396e7b875e6d`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.3 MB (1270567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a343d34cc8043ffbeea2d56b2aed666b59121a84df795fd85431ac0850c3fe20`  
		Last Modified: Sat, 23 Apr 2022 06:56:45 GMT  
		Size: 27.2 MB (27178678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb0fd939cc37c467ea608d864215df9bf23232d8c4a33dd75f76f31cf78f35f`  
		Last Modified: Sat, 23 Apr 2022 06:56:36 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef815839ee8834a81a93554ed6ad864c9c3f04f1c24221f5e9e2f66a8e9d7b01`  
		Last Modified: Sat, 23 Apr 2022 06:56:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:8655a00b9e2d342c883b64a5141ce278d28313250721ced3fca543828cf82cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121335534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518d3ef0290a9008705033e76ea6c6971f4037809ab324c393a3f49d6a7504a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:56:47 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:57:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:13:53 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:14:05 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:14:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:14:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:14:18 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:14:19 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:14:20 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:14:53 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 08:14:54 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 08:15:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:15:16 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:15:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:15:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:15:20 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:15:21 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241f218f4a9078a7dcbfc6fd6ed6877e46407b06b6221bc6206fab8af4c590b`  
		Last Modified: Fri, 22 Apr 2022 03:02:34 GMT  
		Size: 40.8 MB (40769834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3678ae378db153e8948d4ba589775345c50a90226740a49251dc8d98ee1ee6`  
		Last Modified: Fri, 22 Apr 2022 03:02:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcef3dfa8c549587028ddd3ff56002acc6fd571241dcd3e972d9343f1f5432`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90633b62b6e047a653abd913ae534c7a42aff79d96a012b69228446cec99fbfe`  
		Last Modified: Fri, 22 Apr 2022 08:16:12 GMT  
		Size: 9.6 MB (9550979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a6a6163139adc28bea3b154833e3d680c71f4ea7394be5f419c7e06c26eb0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.0 MB (1011031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2093a9e4835da6785bcead1c0ca8da7a2f9e8e754f267b24ed0c394620314a6`  
		Last Modified: Fri, 22 Apr 2022 08:16:36 GMT  
		Size: 26.9 MB (26935470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd4df7be17dd8b1a81a01d7afff148634fec73a10bc9f530a99cb1388ae78f8`  
		Last Modified: Fri, 22 Apr 2022 08:16:33 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645fc07c02e8c315b2fda5d5def9a1970fcd0f17fd6d0dc5bb788b27ce1e4dda`  
		Last Modified: Fri, 22 Apr 2022 08:16:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:27c5c7450944e44d28e7502f15b7b0f100ca14a093939d7c29080086c021e7a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130384518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8619fcacf0580ae04c21b4a25e715af1a3dcbb29135ad8ffd1fb87489284e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:47:03 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 09:47:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:48:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:48:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 15:58:58 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 16:00:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 16:00:36 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 16:00:38 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 16:00:40 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 16:00:41 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 16:02:07 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 16:02:11 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 16:03:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 16:03:08 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 16:03:11 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 16:03:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 16:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:03:20 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 16:03:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc4da81b86f2d794067f5074f224a2816851960275189b2d3c178608853518`  
		Last Modified: Fri, 22 Apr 2022 09:58:55 GMT  
		Size: 41.2 MB (41162345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15824a78c37261d06cbabfff12b54690edcb179cce082b71f20b44471365c8`  
		Last Modified: Fri, 22 Apr 2022 09:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e184c002e7628b8689deb98ed5547310b9951736d421a5594701f0211bd826`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f04cbe05e83893ff0786818415db712edfee149c001723975b4fc6af9f4076`  
		Last Modified: Fri, 22 Apr 2022 16:04:33 GMT  
		Size: 10.3 MB (10310111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7690d4477b275d4157e369fe0d406e41dae39c995e0f10758abfc646ab9256`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 MB (1236781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0117c2360f1062593f95f576a6842c908b859cc42a7e5c2a6e2c86152813c4e4`  
		Last Modified: Fri, 22 Apr 2022 16:04:54 GMT  
		Size: 27.2 MB (27177369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310ef53427ce6ffc628ff813662fee750dc5f4b05414bb14486bf7594b3bd2ec`  
		Last Modified: Fri, 22 Apr 2022 16:04:51 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bdc54cdef0c09e93002e9cd4b6281f422fe66bf64193bd45569f123ecf77a6`  
		Last Modified: Fri, 22 Apr 2022 16:04:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.0.26`

```console
$ docker pull cassandra@sha256:2370e4dffd0ddee9bfc816b8dac863ed2828b2b6d2196f90ae1b346910638568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:3.0.26` - linux; amd64

```console
$ docker pull cassandra@sha256:5535de3aa0166f767a6e57b8f376323382cb11005b2e689ac60cc4c282714f6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124386720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9238ebd57db75d9798232f2497172ce7a0711bb899389b57976f1fa85ad45338`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:04:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:04:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:04:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:50:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:52 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:53 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:51:12 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 08:51:12 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 08:51:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:51:30 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:51:30 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:51:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:51:30 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:51:30 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b1157d6084a2ea36096688a243ea6d05fc59b44b2331626849535196db689`  
		Last Modified: Fri, 22 Apr 2022 02:08:41 GMT  
		Size: 41.8 MB (41773808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94201e8045a2b75849b87376763eb19cd1ec004669a3d4821923f64259838bf`  
		Last Modified: Fri, 22 Apr 2022 02:08:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ea050078a67a35d2f11b500aa75b78bf0d6d85f91f14280a49c4a67c7fdc4`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609edbe68ee0c662e37d045a9ead6e3615bf900df2fdbc019d6f3f81d42e68e2`  
		Last Modified: Fri, 22 Apr 2022 08:52:08 GMT  
		Size: 9.5 MB (9520679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0b03034f96bab865bed901a6ffa503f19aa9170f1b72ad4eb7a74b54a4ac2`  
		Last Modified: Fri, 22 Apr 2022 08:52:07 GMT  
		Size: 1.3 MB (1316224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41569460a89754a6e114eb26476c80288c6c76ab8de78509276cf1acb3b14427`  
		Last Modified: Fri, 22 Apr 2022 08:52:23 GMT  
		Size: 27.2 MB (27176638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3a452c0ca1b3d13e157d207d18ab54cf58c864be3979b0ab111db2f08927d6`  
		Last Modified: Fri, 22 Apr 2022 08:52:21 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b04ba31b9bdae2bf4e20bebdcd6898ebb578d786665e904d143e86b51713bd6`  
		Last Modified: Fri, 22 Apr 2022 08:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0.26` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:461a512825cc8aa961de9dd109d10dda19579497ee2fb10efe102a707c973ebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115835949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2010bb920ffa9c676b298ab44c0b687004f24d439f7e481000d0ba40e6a424c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:17:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 23 Apr 2022 00:18:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:18:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:18:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 23 Apr 2022 06:52:34 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:52:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:52:54 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:53:14 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:53:15 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:54:07 GMT
ENV CASSANDRA_VERSION=3.0.26
# Sat, 23 Apr 2022 06:54:07 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Sat, 23 Apr 2022 06:54:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:54:39 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:54:40 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:54:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 23 Apr 2022 06:54:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:54:42 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:54:42 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b77390aa7e68829cfed8e84ca110bf8df1b62d07074bc4d3548e3b5a74837d`  
		Last Modified: Sat, 23 Apr 2022 00:27:24 GMT  
		Size: 39.5 MB (39508183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263bee161abb30a7eb910dfbbcfeb506170b373e07866388acb3647c3474e2d2`  
		Last Modified: Sat, 23 Apr 2022 00:27:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e95e7ee9157d74a18ed84c37a1b47f2625b8929778ee979293eaf5e073f97c`  
		Last Modified: Sat, 23 Apr 2022 06:56:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe4bbcbaa326c450337285613afdb3c8806fc8093778b4ba44d1e7cb3d12ae5`  
		Last Modified: Sat, 23 Apr 2022 06:56:17 GMT  
		Size: 8.9 MB (8900042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb14a5abcd9c1a92954d4da43bd1ed6d28ef179f47e49169fac4396e7b875e6d`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.3 MB (1270567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a343d34cc8043ffbeea2d56b2aed666b59121a84df795fd85431ac0850c3fe20`  
		Last Modified: Sat, 23 Apr 2022 06:56:45 GMT  
		Size: 27.2 MB (27178678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb0fd939cc37c467ea608d864215df9bf23232d8c4a33dd75f76f31cf78f35f`  
		Last Modified: Sat, 23 Apr 2022 06:56:36 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef815839ee8834a81a93554ed6ad864c9c3f04f1c24221f5e9e2f66a8e9d7b01`  
		Last Modified: Sat, 23 Apr 2022 06:56:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0.26` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:8655a00b9e2d342c883b64a5141ce278d28313250721ced3fca543828cf82cff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121335534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518d3ef0290a9008705033e76ea6c6971f4037809ab324c393a3f49d6a7504a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:56:47 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:57:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:13:53 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:14:05 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:14:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:14:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:14:18 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:14:19 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:14:20 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:14:53 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 08:14:54 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 08:15:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:15:16 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:15:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:15:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:15:20 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:15:21 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241f218f4a9078a7dcbfc6fd6ed6877e46407b06b6221bc6206fab8af4c590b`  
		Last Modified: Fri, 22 Apr 2022 03:02:34 GMT  
		Size: 40.8 MB (40769834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3678ae378db153e8948d4ba589775345c50a90226740a49251dc8d98ee1ee6`  
		Last Modified: Fri, 22 Apr 2022 03:02:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcef3dfa8c549587028ddd3ff56002acc6fd571241dcd3e972d9343f1f5432`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90633b62b6e047a653abd913ae534c7a42aff79d96a012b69228446cec99fbfe`  
		Last Modified: Fri, 22 Apr 2022 08:16:12 GMT  
		Size: 9.6 MB (9550979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a6a6163139adc28bea3b154833e3d680c71f4ea7394be5f419c7e06c26eb0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.0 MB (1011031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2093a9e4835da6785bcead1c0ca8da7a2f9e8e754f267b24ed0c394620314a6`  
		Last Modified: Fri, 22 Apr 2022 08:16:36 GMT  
		Size: 26.9 MB (26935470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd4df7be17dd8b1a81a01d7afff148634fec73a10bc9f530a99cb1388ae78f8`  
		Last Modified: Fri, 22 Apr 2022 08:16:33 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645fc07c02e8c315b2fda5d5def9a1970fcd0f17fd6d0dc5bb788b27ce1e4dda`  
		Last Modified: Fri, 22 Apr 2022 08:16:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.0.26` - linux; ppc64le

```console
$ docker pull cassandra@sha256:27c5c7450944e44d28e7502f15b7b0f100ca14a093939d7c29080086c021e7a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130384518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8619fcacf0580ae04c21b4a25e715af1a3dcbb29135ad8ffd1fb87489284e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:47:03 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 09:47:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:48:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:48:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 15:58:58 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 16:00:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 16:00:36 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 16:00:38 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 16:00:40 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 16:00:41 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 16:02:07 GMT
ENV CASSANDRA_VERSION=3.0.26
# Fri, 22 Apr 2022 16:02:11 GMT
ENV CASSANDRA_SHA512=1f18094d0191d722371942d6046dcd0b70342c995800c277c822d81a2584c3b8d3f38d47f831b19d3ccf17b079a24540672998ba1b546d67594ff62618323c54
# Fri, 22 Apr 2022 16:03:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 16:03:08 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 16:03:11 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 16:03:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 16:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:03:20 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 16:03:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc4da81b86f2d794067f5074f224a2816851960275189b2d3c178608853518`  
		Last Modified: Fri, 22 Apr 2022 09:58:55 GMT  
		Size: 41.2 MB (41162345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15824a78c37261d06cbabfff12b54690edcb179cce082b71f20b44471365c8`  
		Last Modified: Fri, 22 Apr 2022 09:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e184c002e7628b8689deb98ed5547310b9951736d421a5594701f0211bd826`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f04cbe05e83893ff0786818415db712edfee149c001723975b4fc6af9f4076`  
		Last Modified: Fri, 22 Apr 2022 16:04:33 GMT  
		Size: 10.3 MB (10310111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7690d4477b275d4157e369fe0d406e41dae39c995e0f10758abfc646ab9256`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 MB (1236781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0117c2360f1062593f95f576a6842c908b859cc42a7e5c2a6e2c86152813c4e4`  
		Last Modified: Fri, 22 Apr 2022 16:04:54 GMT  
		Size: 27.2 MB (27177369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310ef53427ce6ffc628ff813662fee750dc5f4b05414bb14486bf7594b3bd2ec`  
		Last Modified: Fri, 22 Apr 2022 16:04:51 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bdc54cdef0c09e93002e9cd4b6281f422fe66bf64193bd45569f123ecf77a6`  
		Last Modified: Fri, 22 Apr 2022 16:04:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.11`

```console
$ docker pull cassandra@sha256:2d796a23dd37295675fd71fa273b7ec365da68609f5d381abafcf3b5ebda0800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:3.11` - linux; amd64

```console
$ docker pull cassandra@sha256:7b4b4239970f21ccbe1fd5bd3ab062e008ca4ed45b516ae9447ccb0bb6519427
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129688132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2475f0fb7aaf3aec7dda8a9fa416e88cf9d91a96db02e4d74024bef7997853aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:04:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:04:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:04:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:50:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:52 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:53 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:51:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:51:08 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:51:08 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:51:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:51:09 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:51:09 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b1157d6084a2ea36096688a243ea6d05fc59b44b2331626849535196db689`  
		Last Modified: Fri, 22 Apr 2022 02:08:41 GMT  
		Size: 41.8 MB (41773808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94201e8045a2b75849b87376763eb19cd1ec004669a3d4821923f64259838bf`  
		Last Modified: Fri, 22 Apr 2022 02:08:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ea050078a67a35d2f11b500aa75b78bf0d6d85f91f14280a49c4a67c7fdc4`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609edbe68ee0c662e37d045a9ead6e3615bf900df2fdbc019d6f3f81d42e68e2`  
		Last Modified: Fri, 22 Apr 2022 08:52:08 GMT  
		Size: 9.5 MB (9520679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0b03034f96bab865bed901a6ffa503f19aa9170f1b72ad4eb7a74b54a4ac2`  
		Last Modified: Fri, 22 Apr 2022 08:52:07 GMT  
		Size: 1.3 MB (1316224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12f39ee7b906538ae17814627b38c201fd4cb40428565f73f4e72dd15dc6ef2`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 32.5 MB (32478053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3ff5172576b28266e0f4e8a2f14212bd0d4b9633c05e5e69754c26af2157b1`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da93bf58be51fe2b7584378d92f35f646a11623578698d53f9cc6a07f2018497`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:6dbd335e172d9c892580b3f129e9dea641f665c72e22e2ccb4cb0a49379dd559
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121137212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ddce1eae8230f1c6fbf15c3b73cc5558492a62eb65a2e204591b524141ab9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:17:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 23 Apr 2022 00:18:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:18:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:18:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 23 Apr 2022 06:52:34 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:52:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:52:54 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:53:14 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:53:15 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_VERSION=3.11.12
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Sat, 23 Apr 2022 06:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:53:46 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:53:46 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:53:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 23 Apr 2022 06:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:53:49 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:53:49 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b77390aa7e68829cfed8e84ca110bf8df1b62d07074bc4d3548e3b5a74837d`  
		Last Modified: Sat, 23 Apr 2022 00:27:24 GMT  
		Size: 39.5 MB (39508183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263bee161abb30a7eb910dfbbcfeb506170b373e07866388acb3647c3474e2d2`  
		Last Modified: Sat, 23 Apr 2022 00:27:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e95e7ee9157d74a18ed84c37a1b47f2625b8929778ee979293eaf5e073f97c`  
		Last Modified: Sat, 23 Apr 2022 06:56:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe4bbcbaa326c450337285613afdb3c8806fc8093778b4ba44d1e7cb3d12ae5`  
		Last Modified: Sat, 23 Apr 2022 06:56:17 GMT  
		Size: 8.9 MB (8900042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb14a5abcd9c1a92954d4da43bd1ed6d28ef179f47e49169fac4396e7b875e6d`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.3 MB (1270567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d708a7a3eb94c16aebce0d43acbcfe31c42f6dc907b9269c4bf02874bd4ab`  
		Last Modified: Sat, 23 Apr 2022 06:56:20 GMT  
		Size: 32.5 MB (32479942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d35607fb75fa026ebb07e465271ba0f21610d3de998fdb558a93e0b4fb626`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9ec8908d382740f1f1dd4520a14e4dab56e577b57763f1076c6ca1cda789f`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:31e240593eacecc2ae00f6a43f1209666c03e9cd372308587861e2ce4bc58b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126636878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc572898ab769ed4a42507072bc3d236e4d558563dae4412735fbf4a5e0a7c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:56:47 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:57:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:13:53 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:14:05 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:14:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:14:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:14:18 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:14:19 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:14:20 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:14:21 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:14:22 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:14:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:14:41 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:14:43 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:14:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:14:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:14:45 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:14:46 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241f218f4a9078a7dcbfc6fd6ed6877e46407b06b6221bc6206fab8af4c590b`  
		Last Modified: Fri, 22 Apr 2022 03:02:34 GMT  
		Size: 40.8 MB (40769834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3678ae378db153e8948d4ba589775345c50a90226740a49251dc8d98ee1ee6`  
		Last Modified: Fri, 22 Apr 2022 03:02:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcef3dfa8c549587028ddd3ff56002acc6fd571241dcd3e972d9343f1f5432`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90633b62b6e047a653abd913ae534c7a42aff79d96a012b69228446cec99fbfe`  
		Last Modified: Fri, 22 Apr 2022 08:16:12 GMT  
		Size: 9.6 MB (9550979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a6a6163139adc28bea3b154833e3d680c71f4ea7394be5f419c7e06c26eb0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.0 MB (1011031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceeb37adb1964398af2632b3de91c825a726badfc7175dc976a03e686df923d`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 32.2 MB (32236813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5582bb4dde880d1ea624a6dd47791f3807466941636befcdb69446e91e72a0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4a16bb56f8c1b161724cceeb1d2c334534d8042d016e8f0fc56664bbf9c3bc`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b7874b6138dc94865d6655e055e9b330414f87d5ebdb65a508dbe939361c698c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135686031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cee2a594026059e4161ae3507c7db2085a52fa19c5c16965e98ece6f0640af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:47:03 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 09:47:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:48:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:48:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 15:58:58 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 16:00:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 16:00:36 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 16:00:38 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 16:00:40 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 16:00:41 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 16:00:43 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 16:00:46 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 16:01:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 16:01:38 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 16:01:41 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 16:01:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 16:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:01:52 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 16:01:53 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc4da81b86f2d794067f5074f224a2816851960275189b2d3c178608853518`  
		Last Modified: Fri, 22 Apr 2022 09:58:55 GMT  
		Size: 41.2 MB (41162345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15824a78c37261d06cbabfff12b54690edcb179cce082b71f20b44471365c8`  
		Last Modified: Fri, 22 Apr 2022 09:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e184c002e7628b8689deb98ed5547310b9951736d421a5594701f0211bd826`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f04cbe05e83893ff0786818415db712edfee149c001723975b4fc6af9f4076`  
		Last Modified: Fri, 22 Apr 2022 16:04:33 GMT  
		Size: 10.3 MB (10310111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7690d4477b275d4157e369fe0d406e41dae39c995e0f10758abfc646ab9256`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 MB (1236781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b48765bc741bd95e551b022969d8c2fcadba3ad4f7c5f5dae01c761b59b837`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 32.5 MB (32478886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fc9ee9f9c0a0f4b7c5c4f826289ac5d97d2c39c859a866fe0919a74ec20cbe`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf83277e0853e4733bd15816971fc969409d794c8f0ae135e1b1b052fcb508`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:3.11.12`

```console
$ docker pull cassandra@sha256:2d796a23dd37295675fd71fa273b7ec365da68609f5d381abafcf3b5ebda0800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:3.11.12` - linux; amd64

```console
$ docker pull cassandra@sha256:7b4b4239970f21ccbe1fd5bd3ab062e008ca4ed45b516ae9447ccb0bb6519427
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129688132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2475f0fb7aaf3aec7dda8a9fa416e88cf9d91a96db02e4d74024bef7997853aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:04:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:04:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:04:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:50:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:52 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:53 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:53 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:50:53 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:51:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:51:08 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:51:08 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:51:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:51:09 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:51:09 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b1157d6084a2ea36096688a243ea6d05fc59b44b2331626849535196db689`  
		Last Modified: Fri, 22 Apr 2022 02:08:41 GMT  
		Size: 41.8 MB (41773808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94201e8045a2b75849b87376763eb19cd1ec004669a3d4821923f64259838bf`  
		Last Modified: Fri, 22 Apr 2022 02:08:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17ea050078a67a35d2f11b500aa75b78bf0d6d85f91f14280a49c4a67c7fdc4`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609edbe68ee0c662e37d045a9ead6e3615bf900df2fdbc019d6f3f81d42e68e2`  
		Last Modified: Fri, 22 Apr 2022 08:52:08 GMT  
		Size: 9.5 MB (9520679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0b03034f96bab865bed901a6ffa503f19aa9170f1b72ad4eb7a74b54a4ac2`  
		Last Modified: Fri, 22 Apr 2022 08:52:07 GMT  
		Size: 1.3 MB (1316224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12f39ee7b906538ae17814627b38c201fd4cb40428565f73f4e72dd15dc6ef2`  
		Last Modified: Fri, 22 Apr 2022 08:52:09 GMT  
		Size: 32.5 MB (32478053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3ff5172576b28266e0f4e8a2f14212bd0d4b9633c05e5e69754c26af2157b1`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da93bf58be51fe2b7584378d92f35f646a11623578698d53f9cc6a07f2018497`  
		Last Modified: Fri, 22 Apr 2022 08:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11.12` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:6dbd335e172d9c892580b3f129e9dea641f665c72e22e2ccb4cb0a49379dd559
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121137212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ddce1eae8230f1c6fbf15c3b73cc5558492a62eb65a2e204591b524141ab9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:17:35 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 23 Apr 2022 00:18:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:18:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:18:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 23 Apr 2022 06:52:34 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:52:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:52:54 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:53:14 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:53:15 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:53:15 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_VERSION=3.11.12
# Sat, 23 Apr 2022 06:53:16 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Sat, 23 Apr 2022 06:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:53:46 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:53:46 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:53:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 23 Apr 2022 06:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:53:49 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:53:49 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b77390aa7e68829cfed8e84ca110bf8df1b62d07074bc4d3548e3b5a74837d`  
		Last Modified: Sat, 23 Apr 2022 00:27:24 GMT  
		Size: 39.5 MB (39508183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263bee161abb30a7eb910dfbbcfeb506170b373e07866388acb3647c3474e2d2`  
		Last Modified: Sat, 23 Apr 2022 00:27:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e95e7ee9157d74a18ed84c37a1b47f2625b8929778ee979293eaf5e073f97c`  
		Last Modified: Sat, 23 Apr 2022 06:56:11 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe4bbcbaa326c450337285613afdb3c8806fc8093778b4ba44d1e7cb3d12ae5`  
		Last Modified: Sat, 23 Apr 2022 06:56:17 GMT  
		Size: 8.9 MB (8900042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb14a5abcd9c1a92954d4da43bd1ed6d28ef179f47e49169fac4396e7b875e6d`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.3 MB (1270567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d708a7a3eb94c16aebce0d43acbcfe31c42f6dc907b9269c4bf02874bd4ab`  
		Last Modified: Sat, 23 Apr 2022 06:56:20 GMT  
		Size: 32.5 MB (32479942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d35607fb75fa026ebb07e465271ba0f21610d3de998fdb558a93e0b4fb626`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e9ec8908d382740f1f1dd4520a14e4dab56e577b57763f1076c6ca1cda789f`  
		Last Modified: Sat, 23 Apr 2022 06:56:10 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11.12` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:31e240593eacecc2ae00f6a43f1209666c03e9cd372308587861e2ce4bc58b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126636878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc572898ab769ed4a42507072bc3d236e4d558563dae4412735fbf4a5e0a7c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:56:47 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 02:57:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:16 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 08:13:53 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:14:05 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:14:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:14:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:14:18 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:14:19 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:14:20 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:14:21 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 08:14:22 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 08:14:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:14:41 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:14:43 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:14:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 08:14:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:14:45 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:14:46 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241f218f4a9078a7dcbfc6fd6ed6877e46407b06b6221bc6206fab8af4c590b`  
		Last Modified: Fri, 22 Apr 2022 03:02:34 GMT  
		Size: 40.8 MB (40769834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3678ae378db153e8948d4ba589775345c50a90226740a49251dc8d98ee1ee6`  
		Last Modified: Fri, 22 Apr 2022 03:02:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcef3dfa8c549587028ddd3ff56002acc6fd571241dcd3e972d9343f1f5432`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90633b62b6e047a653abd913ae534c7a42aff79d96a012b69228446cec99fbfe`  
		Last Modified: Fri, 22 Apr 2022 08:16:12 GMT  
		Size: 9.6 MB (9550979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a6a6163139adc28bea3b154833e3d680c71f4ea7394be5f419c7e06c26eb0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.0 MB (1011031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aceeb37adb1964398af2632b3de91c825a726badfc7175dc976a03e686df923d`  
		Last Modified: Fri, 22 Apr 2022 08:16:13 GMT  
		Size: 32.2 MB (32236813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5582bb4dde880d1ea624a6dd47791f3807466941636befcdb69446e91e72a0`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4a16bb56f8c1b161724cceeb1d2c334534d8042d016e8f0fc56664bbf9c3bc`  
		Last Modified: Fri, 22 Apr 2022 08:16:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:3.11.12` - linux; ppc64le

```console
$ docker pull cassandra@sha256:b7874b6138dc94865d6655e055e9b330414f87d5ebdb65a508dbe939361c698c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135686031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cee2a594026059e4161ae3507c7db2085a52fa19c5c16965e98ece6f0640af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:47:03 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 22 Apr 2022 09:47:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:48:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:48:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 22 Apr 2022 15:58:58 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:59:43 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 16:00:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 16:00:36 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 16:00:38 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 16:00:40 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 16:00:41 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 16:00:43 GMT
ENV CASSANDRA_VERSION=3.11.12
# Fri, 22 Apr 2022 16:00:46 GMT
ENV CASSANDRA_SHA512=788446e281353bd1bebab983702643a4a8a5ac39ae69d6e17c257793de7a9105884c2cd35a40873ad5a091b36cd916934ef2d51d1e347b729d5068fc54a54f01
# Fri, 22 Apr 2022 16:01:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 16:01:38 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 16:01:41 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 16:01:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 22 Apr 2022 16:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:01:52 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 16:01:53 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc4da81b86f2d794067f5074f224a2816851960275189b2d3c178608853518`  
		Last Modified: Fri, 22 Apr 2022 09:58:55 GMT  
		Size: 41.2 MB (41162345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15824a78c37261d06cbabfff12b54690edcb179cce082b71f20b44471365c8`  
		Last Modified: Fri, 22 Apr 2022 09:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e184c002e7628b8689deb98ed5547310b9951736d421a5594701f0211bd826`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f04cbe05e83893ff0786818415db712edfee149c001723975b4fc6af9f4076`  
		Last Modified: Fri, 22 Apr 2022 16:04:33 GMT  
		Size: 10.3 MB (10310111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7690d4477b275d4157e369fe0d406e41dae39c995e0f10758abfc646ab9256`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 MB (1236781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b48765bc741bd95e551b022969d8c2fcadba3ad4f7c5f5dae01c761b59b837`  
		Last Modified: Fri, 22 Apr 2022 16:04:34 GMT  
		Size: 32.5 MB (32478886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fc9ee9f9c0a0f4b7c5c4f826289ac5d97d2c39c859a866fe0919a74ec20cbe`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf83277e0853e4733bd15816971fc969409d794c8f0ae135e1b1b052fcb508`  
		Last Modified: Fri, 22 Apr 2022 16:04:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:4`

```console
$ docker pull cassandra@sha256:10b81fd1651dc824a861a2491f38f323867d57f89cc3c3ee217c6aa3fa9deac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:4` - linux; amd64

```console
$ docker pull cassandra@sha256:6c956be475bfabf184afcaddf0d2bff14974e84e3188cae0c0680ec25ae8397d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150122631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9126ab111ef3a970d4d288477eb7c09c4bd033963d2f50b8b6be8a0cf552795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:05:03 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:05:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:05:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:05:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:49:44 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:11 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:50:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:50:27 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:50:28 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:50:28 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:50:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472f4f0c5d6412755b08c96f99771c7aeb53b2208d7c34a03f9c7be592a8a412`  
		Last Modified: Fri, 22 Apr 2022 02:09:28 GMT  
		Size: 43.2 MB (43230162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8794c46632ab780fe47457f40fdcba994389c7cdf193ca9f20045b952c4254a`  
		Last Modified: Fri, 22 Apr 2022 02:09:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47881d4a1fabe1f84ade4b7b2b5e83d9dccc0518c1a2b98736f1b43474e6f7ac`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948e35f7d5620ca51d1bb2bf2124ae6c9ed19f1f02a291679ac821728c51b2e5`  
		Last Modified: Fri, 22 Apr 2022 08:51:49 GMT  
		Size: 10.9 MB (10945355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e840f2fffced47d9f18b06e615aac2044845ea0237532df46c3090c7a0cf15`  
		Last Modified: Fri, 22 Apr 2022 08:51:47 GMT  
		Size: 1.3 MB (1314656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9543e5c86498bd6ae98e35e25348b0cf60b209b58dbe0029ee331ca534f8dca`  
		Last Modified: Fri, 22 Apr 2022 08:51:50 GMT  
		Size: 50.0 MB (50033205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee30313d18303f5ab84483d3efe20359966097f412dbe02d714bbb6f308d1b`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8e93d50f69f1bb4048aeecdfd8ab7a2f65f1e791a295da9249b6b7b0e930e376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142241905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb79f8e9656b8e97b488d1507b072f1472d07bdf858d267ff156cbb756003037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:18:50 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Sat, 23 Apr 2022 00:19:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:19:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:19:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 23 Apr 2022 06:51:01 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:51:22 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:51:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:51:44 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:51:44 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:51:44 GMT
ENV CASSANDRA_VERSION=4.0.3
# Sat, 23 Apr 2022 06:51:45 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Sat, 23 Apr 2022 06:52:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:52:18 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:52:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:52:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:52:19 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:52:19 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3816979cbf0a5b65f6da29ca65af9f3bdfe0dce61eb75a3daaf96cdf3bf42791`  
		Last Modified: Sat, 23 Apr 2022 00:29:33 GMT  
		Size: 41.9 MB (41850617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd40ec25539822a665bd5e20865612d0ec0e12212533dd8919921592074e2d75`  
		Last Modified: Sat, 23 Apr 2022 00:29:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06decb73aa6eaa8db4515647e8266d51bac0eefe701760671a91c1c954d855f3`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0177dcb1d65cd67c10536b392a85a68f0c85efbb66a5c5ea514f9239ece8146f`  
		Last Modified: Sat, 23 Apr 2022 06:55:42 GMT  
		Size: 10.1 MB (10109376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636efa7c9e3a7ae1e95545df47f3b72d854fb335b3feaaa978f55a8694e3340c`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.3 MB (1268657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ba6fbfa3fd70486f891d469bd517df00320fd179e2205c3a01b07c30e059b`  
		Last Modified: Sat, 23 Apr 2022 06:55:50 GMT  
		Size: 50.0 MB (50034896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592fa509d02bb8b1631cc0877fecc69a2e75c54d14eb5dca54d49c2ea32f36fd`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7c3b440dd0ceff9056a993cb8a6397ad3a8fc109f213a0a490028a592ae8c858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146448981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d6527257e9f5da3be4bfc0f4af35a91e795eb61be78d813cd17643fc1b3150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:57:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:57:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:12:40 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:12:52 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:13:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:13:05 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:13:06 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:13:07 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:13:08 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:13:09 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:13:10 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:13:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:13:34 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:13:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:13:37 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:13:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec453ac99a9939a498000b4312da74d702ea3ae510b1c61e2b2ba6ab1705d75`  
		Last Modified: Fri, 22 Apr 2022 03:03:27 GMT  
		Size: 41.6 MB (41572364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091800aef8bea9c75d3ed17faa03c050e35d951671879d52ee8508abbe4854c`  
		Last Modified: Fri, 22 Apr 2022 03:03:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d57fb0144ee6d91a5b072a12d9b2e815316493291abd7c7a7767559957ff6`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb2132c85ad7ee0a5b963f79af4e5987d6f2d89d10162357c15ed1e47bfa07`  
		Last Modified: Fri, 22 Apr 2022 08:15:52 GMT  
		Size: 11.0 MB (11006911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd29123be44f6edd5c4f49221d60d59a69c5574e68aea2b244db6fcac8351f5a`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.0 MB (1009494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1db89cbed1286548fb7719f3662bc5821ff4918b13479bb90abb2abfd0b05d9`  
		Last Modified: Fri, 22 Apr 2022 08:15:53 GMT  
		Size: 49.8 MB (49792111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14286a91c6cf52fae51a79306dc02bb8abbc9a93b252c8ff921c6d6e68f7ef4`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4` - linux; ppc64le

```console
$ docker pull cassandra@sha256:64cb3ab7190cfe7e7cb1f580442f6d871b72200dd836ad7cea63435cc588e3bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.4 MB (152367981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385968731a52d3893f043bf02b6b29a43685759a30845159509824dc711549e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:48:21 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 09:49:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:49:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:49:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 15:55:46 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 15:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 15:57:07 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 15:57:09 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 15:57:14 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 15:57:18 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 15:57:20 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 15:57:23 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 15:58:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 15:58:31 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 15:58:33 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 15:58:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 15:58:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 15:58:39 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f243acf481bce9a21733f17f85e0d8ef7c1c1923824328a0db51dd225812e72`  
		Last Modified: Fri, 22 Apr 2022 10:00:02 GMT  
		Size: 38.6 MB (38640564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17138c478baa866391090a242e73ea987187d533a8dc86ca759970d9626b74e2`  
		Last Modified: Fri, 22 Apr 2022 09:59:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f0ce23c1783f30c6b14618830c14bb3bd572e7e58ca74ffc3b0ebafb1904d`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566987a573e9d87a66f4c7008e0a04d809b6c765760483eef83f274fdf5b47a8`  
		Last Modified: Fri, 22 Apr 2022 16:04:09 GMT  
		Size: 12.0 MB (11960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e3288e09eb34be7e49a553d3c855d91a4ff8cc544bbca0cf36c28ae8ebbd0`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 MB (1235042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94e5d84893916eb8e94b4c5ec10e41202cfd77f9906e4ca0ed7b12737de3e0`  
		Last Modified: Fri, 22 Apr 2022 16:04:11 GMT  
		Size: 50.0 MB (50034135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed2c23ad707dcc0e3b3c3e4fe66967db87f02663bb9b8d6fac3507cfa1067a`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:4.0`

```console
$ docker pull cassandra@sha256:10b81fd1651dc824a861a2491f38f323867d57f89cc3c3ee217c6aa3fa9deac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:4.0` - linux; amd64

```console
$ docker pull cassandra@sha256:6c956be475bfabf184afcaddf0d2bff14974e84e3188cae0c0680ec25ae8397d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150122631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9126ab111ef3a970d4d288477eb7c09c4bd033963d2f50b8b6be8a0cf552795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:05:03 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:05:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:05:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:05:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:49:44 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:11 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:50:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:50:27 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:50:28 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:50:28 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:50:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472f4f0c5d6412755b08c96f99771c7aeb53b2208d7c34a03f9c7be592a8a412`  
		Last Modified: Fri, 22 Apr 2022 02:09:28 GMT  
		Size: 43.2 MB (43230162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8794c46632ab780fe47457f40fdcba994389c7cdf193ca9f20045b952c4254a`  
		Last Modified: Fri, 22 Apr 2022 02:09:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47881d4a1fabe1f84ade4b7b2b5e83d9dccc0518c1a2b98736f1b43474e6f7ac`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948e35f7d5620ca51d1bb2bf2124ae6c9ed19f1f02a291679ac821728c51b2e5`  
		Last Modified: Fri, 22 Apr 2022 08:51:49 GMT  
		Size: 10.9 MB (10945355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e840f2fffced47d9f18b06e615aac2044845ea0237532df46c3090c7a0cf15`  
		Last Modified: Fri, 22 Apr 2022 08:51:47 GMT  
		Size: 1.3 MB (1314656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9543e5c86498bd6ae98e35e25348b0cf60b209b58dbe0029ee331ca534f8dca`  
		Last Modified: Fri, 22 Apr 2022 08:51:50 GMT  
		Size: 50.0 MB (50033205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee30313d18303f5ab84483d3efe20359966097f412dbe02d714bbb6f308d1b`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8e93d50f69f1bb4048aeecdfd8ab7a2f65f1e791a295da9249b6b7b0e930e376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142241905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb79f8e9656b8e97b488d1507b072f1472d07bdf858d267ff156cbb756003037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:18:50 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Sat, 23 Apr 2022 00:19:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:19:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:19:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 23 Apr 2022 06:51:01 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:51:22 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:51:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:51:44 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:51:44 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:51:44 GMT
ENV CASSANDRA_VERSION=4.0.3
# Sat, 23 Apr 2022 06:51:45 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Sat, 23 Apr 2022 06:52:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:52:18 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:52:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:52:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:52:19 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:52:19 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3816979cbf0a5b65f6da29ca65af9f3bdfe0dce61eb75a3daaf96cdf3bf42791`  
		Last Modified: Sat, 23 Apr 2022 00:29:33 GMT  
		Size: 41.9 MB (41850617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd40ec25539822a665bd5e20865612d0ec0e12212533dd8919921592074e2d75`  
		Last Modified: Sat, 23 Apr 2022 00:29:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06decb73aa6eaa8db4515647e8266d51bac0eefe701760671a91c1c954d855f3`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0177dcb1d65cd67c10536b392a85a68f0c85efbb66a5c5ea514f9239ece8146f`  
		Last Modified: Sat, 23 Apr 2022 06:55:42 GMT  
		Size: 10.1 MB (10109376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636efa7c9e3a7ae1e95545df47f3b72d854fb335b3feaaa978f55a8694e3340c`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.3 MB (1268657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ba6fbfa3fd70486f891d469bd517df00320fd179e2205c3a01b07c30e059b`  
		Last Modified: Sat, 23 Apr 2022 06:55:50 GMT  
		Size: 50.0 MB (50034896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592fa509d02bb8b1631cc0877fecc69a2e75c54d14eb5dca54d49c2ea32f36fd`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7c3b440dd0ceff9056a993cb8a6397ad3a8fc109f213a0a490028a592ae8c858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146448981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d6527257e9f5da3be4bfc0f4af35a91e795eb61be78d813cd17643fc1b3150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:57:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:57:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:12:40 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:12:52 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:13:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:13:05 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:13:06 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:13:07 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:13:08 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:13:09 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:13:10 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:13:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:13:34 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:13:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:13:37 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:13:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec453ac99a9939a498000b4312da74d702ea3ae510b1c61e2b2ba6ab1705d75`  
		Last Modified: Fri, 22 Apr 2022 03:03:27 GMT  
		Size: 41.6 MB (41572364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091800aef8bea9c75d3ed17faa03c050e35d951671879d52ee8508abbe4854c`  
		Last Modified: Fri, 22 Apr 2022 03:03:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d57fb0144ee6d91a5b072a12d9b2e815316493291abd7c7a7767559957ff6`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb2132c85ad7ee0a5b963f79af4e5987d6f2d89d10162357c15ed1e47bfa07`  
		Last Modified: Fri, 22 Apr 2022 08:15:52 GMT  
		Size: 11.0 MB (11006911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd29123be44f6edd5c4f49221d60d59a69c5574e68aea2b244db6fcac8351f5a`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.0 MB (1009494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1db89cbed1286548fb7719f3662bc5821ff4918b13479bb90abb2abfd0b05d9`  
		Last Modified: Fri, 22 Apr 2022 08:15:53 GMT  
		Size: 49.8 MB (49792111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14286a91c6cf52fae51a79306dc02bb8abbc9a93b252c8ff921c6d6e68f7ef4`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:64cb3ab7190cfe7e7cb1f580442f6d871b72200dd836ad7cea63435cc588e3bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.4 MB (152367981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385968731a52d3893f043bf02b6b29a43685759a30845159509824dc711549e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:48:21 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 09:49:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:49:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:49:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 15:55:46 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 15:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 15:57:07 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 15:57:09 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 15:57:14 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 15:57:18 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 15:57:20 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 15:57:23 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 15:58:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 15:58:31 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 15:58:33 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 15:58:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 15:58:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 15:58:39 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f243acf481bce9a21733f17f85e0d8ef7c1c1923824328a0db51dd225812e72`  
		Last Modified: Fri, 22 Apr 2022 10:00:02 GMT  
		Size: 38.6 MB (38640564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17138c478baa866391090a242e73ea987187d533a8dc86ca759970d9626b74e2`  
		Last Modified: Fri, 22 Apr 2022 09:59:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f0ce23c1783f30c6b14618830c14bb3bd572e7e58ca74ffc3b0ebafb1904d`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566987a573e9d87a66f4c7008e0a04d809b6c765760483eef83f274fdf5b47a8`  
		Last Modified: Fri, 22 Apr 2022 16:04:09 GMT  
		Size: 12.0 MB (11960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e3288e09eb34be7e49a553d3c855d91a4ff8cc544bbca0cf36c28ae8ebbd0`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 MB (1235042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94e5d84893916eb8e94b4c5ec10e41202cfd77f9906e4ca0ed7b12737de3e0`  
		Last Modified: Fri, 22 Apr 2022 16:04:11 GMT  
		Size: 50.0 MB (50034135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed2c23ad707dcc0e3b3c3e4fe66967db87f02663bb9b8d6fac3507cfa1067a`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:4.0.3`

```console
$ docker pull cassandra@sha256:10b81fd1651dc824a861a2491f38f323867d57f89cc3c3ee217c6aa3fa9deac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:4.0.3` - linux; amd64

```console
$ docker pull cassandra@sha256:6c956be475bfabf184afcaddf0d2bff14974e84e3188cae0c0680ec25ae8397d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150122631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9126ab111ef3a970d4d288477eb7c09c4bd033963d2f50b8b6be8a0cf552795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:05:03 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:05:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:05:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:05:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:49:44 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:11 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:50:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:50:27 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:50:28 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:50:28 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:50:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472f4f0c5d6412755b08c96f99771c7aeb53b2208d7c34a03f9c7be592a8a412`  
		Last Modified: Fri, 22 Apr 2022 02:09:28 GMT  
		Size: 43.2 MB (43230162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8794c46632ab780fe47457f40fdcba994389c7cdf193ca9f20045b952c4254a`  
		Last Modified: Fri, 22 Apr 2022 02:09:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47881d4a1fabe1f84ade4b7b2b5e83d9dccc0518c1a2b98736f1b43474e6f7ac`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948e35f7d5620ca51d1bb2bf2124ae6c9ed19f1f02a291679ac821728c51b2e5`  
		Last Modified: Fri, 22 Apr 2022 08:51:49 GMT  
		Size: 10.9 MB (10945355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e840f2fffced47d9f18b06e615aac2044845ea0237532df46c3090c7a0cf15`  
		Last Modified: Fri, 22 Apr 2022 08:51:47 GMT  
		Size: 1.3 MB (1314656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9543e5c86498bd6ae98e35e25348b0cf60b209b58dbe0029ee331ca534f8dca`  
		Last Modified: Fri, 22 Apr 2022 08:51:50 GMT  
		Size: 50.0 MB (50033205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee30313d18303f5ab84483d3efe20359966097f412dbe02d714bbb6f308d1b`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0.3` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8e93d50f69f1bb4048aeecdfd8ab7a2f65f1e791a295da9249b6b7b0e930e376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142241905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb79f8e9656b8e97b488d1507b072f1472d07bdf858d267ff156cbb756003037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:18:50 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Sat, 23 Apr 2022 00:19:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:19:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:19:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 23 Apr 2022 06:51:01 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:51:22 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:51:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:51:44 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:51:44 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:51:44 GMT
ENV CASSANDRA_VERSION=4.0.3
# Sat, 23 Apr 2022 06:51:45 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Sat, 23 Apr 2022 06:52:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:52:18 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:52:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:52:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:52:19 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:52:19 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3816979cbf0a5b65f6da29ca65af9f3bdfe0dce61eb75a3daaf96cdf3bf42791`  
		Last Modified: Sat, 23 Apr 2022 00:29:33 GMT  
		Size: 41.9 MB (41850617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd40ec25539822a665bd5e20865612d0ec0e12212533dd8919921592074e2d75`  
		Last Modified: Sat, 23 Apr 2022 00:29:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06decb73aa6eaa8db4515647e8266d51bac0eefe701760671a91c1c954d855f3`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0177dcb1d65cd67c10536b392a85a68f0c85efbb66a5c5ea514f9239ece8146f`  
		Last Modified: Sat, 23 Apr 2022 06:55:42 GMT  
		Size: 10.1 MB (10109376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636efa7c9e3a7ae1e95545df47f3b72d854fb335b3feaaa978f55a8694e3340c`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.3 MB (1268657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ba6fbfa3fd70486f891d469bd517df00320fd179e2205c3a01b07c30e059b`  
		Last Modified: Sat, 23 Apr 2022 06:55:50 GMT  
		Size: 50.0 MB (50034896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592fa509d02bb8b1631cc0877fecc69a2e75c54d14eb5dca54d49c2ea32f36fd`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0.3` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7c3b440dd0ceff9056a993cb8a6397ad3a8fc109f213a0a490028a592ae8c858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146448981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d6527257e9f5da3be4bfc0f4af35a91e795eb61be78d813cd17643fc1b3150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:57:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:57:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:12:40 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:12:52 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:13:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:13:05 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:13:06 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:13:07 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:13:08 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:13:09 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:13:10 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:13:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:13:34 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:13:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:13:37 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:13:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec453ac99a9939a498000b4312da74d702ea3ae510b1c61e2b2ba6ab1705d75`  
		Last Modified: Fri, 22 Apr 2022 03:03:27 GMT  
		Size: 41.6 MB (41572364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091800aef8bea9c75d3ed17faa03c050e35d951671879d52ee8508abbe4854c`  
		Last Modified: Fri, 22 Apr 2022 03:03:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d57fb0144ee6d91a5b072a12d9b2e815316493291abd7c7a7767559957ff6`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb2132c85ad7ee0a5b963f79af4e5987d6f2d89d10162357c15ed1e47bfa07`  
		Last Modified: Fri, 22 Apr 2022 08:15:52 GMT  
		Size: 11.0 MB (11006911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd29123be44f6edd5c4f49221d60d59a69c5574e68aea2b244db6fcac8351f5a`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.0 MB (1009494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1db89cbed1286548fb7719f3662bc5821ff4918b13479bb90abb2abfd0b05d9`  
		Last Modified: Fri, 22 Apr 2022 08:15:53 GMT  
		Size: 49.8 MB (49792111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14286a91c6cf52fae51a79306dc02bb8abbc9a93b252c8ff921c6d6e68f7ef4`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:4.0.3` - linux; ppc64le

```console
$ docker pull cassandra@sha256:64cb3ab7190cfe7e7cb1f580442f6d871b72200dd836ad7cea63435cc588e3bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.4 MB (152367981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385968731a52d3893f043bf02b6b29a43685759a30845159509824dc711549e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:48:21 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 09:49:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:49:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:49:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 15:55:46 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 15:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 15:57:07 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 15:57:09 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 15:57:14 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 15:57:18 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 15:57:20 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 15:57:23 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 15:58:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 15:58:31 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 15:58:33 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 15:58:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 15:58:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 15:58:39 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f243acf481bce9a21733f17f85e0d8ef7c1c1923824328a0db51dd225812e72`  
		Last Modified: Fri, 22 Apr 2022 10:00:02 GMT  
		Size: 38.6 MB (38640564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17138c478baa866391090a242e73ea987187d533a8dc86ca759970d9626b74e2`  
		Last Modified: Fri, 22 Apr 2022 09:59:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f0ce23c1783f30c6b14618830c14bb3bd572e7e58ca74ffc3b0ebafb1904d`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566987a573e9d87a66f4c7008e0a04d809b6c765760483eef83f274fdf5b47a8`  
		Last Modified: Fri, 22 Apr 2022 16:04:09 GMT  
		Size: 12.0 MB (11960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e3288e09eb34be7e49a553d3c855d91a4ff8cc544bbca0cf36c28ae8ebbd0`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 MB (1235042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94e5d84893916eb8e94b4c5ec10e41202cfd77f9906e4ca0ed7b12737de3e0`  
		Last Modified: Fri, 22 Apr 2022 16:04:11 GMT  
		Size: 50.0 MB (50034135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed2c23ad707dcc0e3b3c3e4fe66967db87f02663bb9b8d6fac3507cfa1067a`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cassandra:latest`

```console
$ docker pull cassandra@sha256:10b81fd1651dc824a861a2491f38f323867d57f89cc3c3ee217c6aa3fa9deac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:latest` - linux; amd64

```console
$ docker pull cassandra@sha256:6c956be475bfabf184afcaddf0d2bff14974e84e3188cae0c0680ec25ae8397d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150122631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9126ab111ef3a970d4d288477eb7c09c4bd033963d2f50b8b6be8a0cf552795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:04:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:05:03 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:05:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:05:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:05:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:49:44 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:50:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:50:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:50:11 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:50:11 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:50:11 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:50:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:50:27 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:50:28 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:50:28 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:50:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11e2aa9202b3c11a943dfa8adc2bef4462ab2165124b84051d10250faff2a0`  
		Last Modified: Fri, 22 Apr 2022 02:08:16 GMT  
		Size: 16.0 MB (16030117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472f4f0c5d6412755b08c96f99771c7aeb53b2208d7c34a03f9c7be592a8a412`  
		Last Modified: Fri, 22 Apr 2022 02:09:28 GMT  
		Size: 43.2 MB (43230162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8794c46632ab780fe47457f40fdcba994389c7cdf193ca9f20045b952c4254a`  
		Last Modified: Fri, 22 Apr 2022 02:09:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47881d4a1fabe1f84ade4b7b2b5e83d9dccc0518c1a2b98736f1b43474e6f7ac`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948e35f7d5620ca51d1bb2bf2124ae6c9ed19f1f02a291679ac821728c51b2e5`  
		Last Modified: Fri, 22 Apr 2022 08:51:49 GMT  
		Size: 10.9 MB (10945355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e840f2fffced47d9f18b06e615aac2044845ea0237532df46c3090c7a0cf15`  
		Last Modified: Fri, 22 Apr 2022 08:51:47 GMT  
		Size: 1.3 MB (1314656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9543e5c86498bd6ae98e35e25348b0cf60b209b58dbe0029ee331ca534f8dca`  
		Last Modified: Fri, 22 Apr 2022 08:51:50 GMT  
		Size: 50.0 MB (50033205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee30313d18303f5ab84483d3efe20359966097f412dbe02d714bbb6f308d1b`  
		Last Modified: Fri, 22 Apr 2022 08:51:46 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8e93d50f69f1bb4048aeecdfd8ab7a2f65f1e791a295da9249b6b7b0e930e376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142241905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb79f8e9656b8e97b488d1507b072f1472d07bdf858d267ff156cbb756003037`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 00:16:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 23 Apr 2022 00:17:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 00:18:50 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Sat, 23 Apr 2022 00:19:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 23 Apr 2022 00:19:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 00:19:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 23 Apr 2022 06:51:01 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Sat, 23 Apr 2022 06:51:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Sat, 23 Apr 2022 06:51:22 GMT
ENV GOSU_VERSION=1.12
# Sat, 23 Apr 2022 06:51:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 23 Apr 2022 06:51:43 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 23 Apr 2022 06:51:44 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Apr 2022 06:51:44 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Sat, 23 Apr 2022 06:51:44 GMT
ENV CASSANDRA_VERSION=4.0.3
# Sat, 23 Apr 2022 06:51:45 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Sat, 23 Apr 2022 06:52:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Sat, 23 Apr 2022 06:52:18 GMT
VOLUME [/var/lib/cassandra]
# Sat, 23 Apr 2022 06:52:18 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Sat, 23 Apr 2022 06:52:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 23 Apr 2022 06:52:19 GMT
EXPOSE 7000 7001 7199 9042 9160
# Sat, 23 Apr 2022 06:52:19 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3370d7b9d77ae5385f189dfcf90d988f7c40b2805c83edeff9d58de940f5135`  
		Last Modified: Sat, 23 Apr 2022 00:26:13 GMT  
		Size: 14.9 MB (14901158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3816979cbf0a5b65f6da29ca65af9f3bdfe0dce61eb75a3daaf96cdf3bf42791`  
		Last Modified: Sat, 23 Apr 2022 00:29:33 GMT  
		Size: 41.9 MB (41850617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd40ec25539822a665bd5e20865612d0ec0e12212533dd8919921592074e2d75`  
		Last Modified: Sat, 23 Apr 2022 00:29:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06decb73aa6eaa8db4515647e8266d51bac0eefe701760671a91c1c954d855f3`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0177dcb1d65cd67c10536b392a85a68f0c85efbb66a5c5ea514f9239ece8146f`  
		Last Modified: Sat, 23 Apr 2022 06:55:42 GMT  
		Size: 10.1 MB (10109376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636efa7c9e3a7ae1e95545df47f3b72d854fb335b3feaaa978f55a8694e3340c`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.3 MB (1268657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ba6fbfa3fd70486f891d469bd517df00320fd179e2205c3a01b07c30e059b`  
		Last Modified: Sat, 23 Apr 2022 06:55:50 GMT  
		Size: 50.0 MB (50034896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592fa509d02bb8b1631cc0877fecc69a2e75c54d14eb5dca54d49c2ea32f36fd`  
		Last Modified: Sat, 23 Apr 2022 06:55:35 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7c3b440dd0ceff9056a993cb8a6397ad3a8fc109f213a0a490028a592ae8c858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146448981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d6527257e9f5da3be4bfc0f4af35a91e795eb61be78d813cd17643fc1b3150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:56:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:56:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:57:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 02:57:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:57:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:57:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 08:12:40 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 08:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 08:12:52 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 08:13:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 08:13:05 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 08:13:06 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 08:13:07 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 08:13:08 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 08:13:09 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 08:13:10 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 08:13:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 08:13:34 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 08:13:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 08:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 08:13:37 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 08:13:38 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89015ff109b922c48ff7f1847b2e63f33dc54bd022e11f479dbed2eb7fb5da0`  
		Last Modified: Fri, 22 Apr 2022 03:02:05 GMT  
		Size: 15.9 MB (15895876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec453ac99a9939a498000b4312da74d702ea3ae510b1c61e2b2ba6ab1705d75`  
		Last Modified: Fri, 22 Apr 2022 03:03:27 GMT  
		Size: 41.6 MB (41572364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091800aef8bea9c75d3ed17faa03c050e35d951671879d52ee8508abbe4854c`  
		Last Modified: Fri, 22 Apr 2022 03:03:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d57fb0144ee6d91a5b072a12d9b2e815316493291abd7c7a7767559957ff6`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb2132c85ad7ee0a5b963f79af4e5987d6f2d89d10162357c15ed1e47bfa07`  
		Last Modified: Fri, 22 Apr 2022 08:15:52 GMT  
		Size: 11.0 MB (11006911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd29123be44f6edd5c4f49221d60d59a69c5574e68aea2b244db6fcac8351f5a`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.0 MB (1009494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1db89cbed1286548fb7719f3662bc5821ff4918b13479bb90abb2abfd0b05d9`  
		Last Modified: Fri, 22 Apr 2022 08:15:53 GMT  
		Size: 49.8 MB (49792111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14286a91c6cf52fae51a79306dc02bb8abbc9a93b252c8ff921c6d6e68f7ef4`  
		Last Modified: Fri, 22 Apr 2022 08:15:49 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; ppc64le

```console
$ docker pull cassandra@sha256:64cb3ab7190cfe7e7cb1f580442f6d871b72200dd836ad7cea63435cc588e3bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.4 MB (152367981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385968731a52d3893f043bf02b6b29a43685759a30845159509824dc711549e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:46:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:48:21 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 22 Apr 2022 09:49:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:49:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:49:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 15:55:46 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Fri, 22 Apr 2022 15:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Fri, 22 Apr 2022 15:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 22 Apr 2022 15:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 15:57:07 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Fri, 22 Apr 2022 15:57:09 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Fri, 22 Apr 2022 15:57:14 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 15:57:18 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Fri, 22 Apr 2022 15:57:20 GMT
ENV CASSANDRA_VERSION=4.0.3
# Fri, 22 Apr 2022 15:57:23 GMT
ENV CASSANDRA_SHA512=b328a6bed9bf2d92f1e44a540bf1d800e26163257ca8e69d6f43ca792aeefe5bacf61b6e5bf2cf7233e34a168ab19de96a52fb3fe82304b7749fde2d7baa81d9
# Fri, 22 Apr 2022 15:58:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Fri, 22 Apr 2022 15:58:31 GMT
VOLUME [/var/lib/cassandra]
# Fri, 22 Apr 2022 15:58:33 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Fri, 22 Apr 2022 15:58:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 15:58:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Fri, 22 Apr 2022 15:58:39 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56b8d6fd0bb34b3c200e96dec3af60f79a6f302365ccc050f056b1d5993a3`  
		Last Modified: Fri, 22 Apr 2022 09:58:22 GMT  
		Size: 17.2 MB (17204271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f243acf481bce9a21733f17f85e0d8ef7c1c1923824328a0db51dd225812e72`  
		Last Modified: Fri, 22 Apr 2022 10:00:02 GMT  
		Size: 38.6 MB (38640564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17138c478baa866391090a242e73ea987187d533a8dc86ca759970d9626b74e2`  
		Last Modified: Fri, 22 Apr 2022 09:59:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54f0ce23c1783f30c6b14618830c14bb3bd572e7e58ca74ffc3b0ebafb1904d`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566987a573e9d87a66f4c7008e0a04d809b6c765760483eef83f274fdf5b47a8`  
		Last Modified: Fri, 22 Apr 2022 16:04:09 GMT  
		Size: 12.0 MB (11960446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e3288e09eb34be7e49a553d3c855d91a4ff8cc544bbca0cf36c28ae8ebbd0`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 MB (1235042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e94e5d84893916eb8e94b4c5ec10e41202cfd77f9906e4ca0ed7b12737de3e0`  
		Last Modified: Fri, 22 Apr 2022 16:04:11 GMT  
		Size: 50.0 MB (50034135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ed2c23ad707dcc0e3b3c3e4fe66967db87f02663bb9b8d6fac3507cfa1067a`  
		Last Modified: Fri, 22 Apr 2022 16:04:06 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
