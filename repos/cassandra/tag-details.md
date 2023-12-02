<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cassandra`

-	[`cassandra:3`](#cassandra3)
-	[`cassandra:3.0`](#cassandra30)
-	[`cassandra:3.0.29`](#cassandra3029)
-	[`cassandra:3.11`](#cassandra311)
-	[`cassandra:3.11.16`](#cassandra31116)
-	[`cassandra:4`](#cassandra4)
-	[`cassandra:4.0`](#cassandra40)
-	[`cassandra:4.0.11`](#cassandra4011)
-	[`cassandra:4.1`](#cassandra41)
-	[`cassandra:4.1.3`](#cassandra413)
-	[`cassandra:5`](#cassandra5)
-	[`cassandra:5.0`](#cassandra50)
-	[`cassandra:5.0-alpha2`](#cassandra50-alpha2)
-	[`cassandra:latest`](#cassandralatest)

## `cassandra:3`

```console
$ docker pull cassandra@sha256:5ed40beccc441bfe2c92e34f77f85ea4cdb715ce3580db4f3dbb36b91c269a91
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `cassandra:3` - linux; amd64

```console
$ docker pull cassandra@sha256:0d1bc6bb301d65ac9e6d73db66e4917e20d3839120ae67bb2a2bfce485d828ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129282302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e54a193f218f067ed8b55fc7dfd4a011af7cbbbbe50905d07ec2569af303795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4241c3cdc52ee7f775d335ffcb8d963485f199febc690674ba3ccaa77d3e2a5`  
		Last Modified: Sat, 02 Dec 2023 02:04:08 GMT  
		Size: 41.9 MB (41859127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a10156a9e03d1fca1fcd43e32a20a1d167252ae7541aecd574b434bb290d3a60`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c346f95791868709d38488a14ea95739281acbd48a11a99b59fdb605e0dc7b7a`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15d171c8e9d4ca134db32442d3a8a993add09d01cfe7880b2c61907ea5fbef9b`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:233818e806d9e56db856a57eacf34d53604642a6b9f99ec9b67f0f2923bd396a`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 9.5 MB (9518587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b010d84521348cbc6a3f5b77ee7c7856fcb0ca47f6b6dafe681704a3c5d2648`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.1 MB (1099988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:828e728899969d374bd4b99929a609ff246e4993e036331a9dce0430fd2a1de9`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 31.3 MB (31296438 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4533533cf3bd3383c2f38ed7930e34081ae60b7e556c898fb090263f24bfbaa`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.2 KB (1226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:590be63dd82c42469d22d262a572aa0039cfdbb2fee9666a5168af5ca0930ada`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3` - unknown; unknown

```console
$ docker pull cassandra@sha256:06f1395b1461c62b396aeb3ac192ae766d46fdd9cf9033c8e3db44425e559781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3707920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31380b54407e8849332d97bddd2f28659533aebdb0aa0533027da01e709f2ea4`

```dockerfile
```

-	Layers:
	-	`sha256:0fb384eda8f2d11e1fc96f54f2032c20eba63beb20d79c18420db0911ea4b59b`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 3.7 MB (3669007 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18bea3a8a82a82ea743d45112c868c5d7c836df05336e444edec5a1f6afbe3b2`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 38.9 KB (38913 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:a6bd569e0d12b6b8155875873a502957b8ffd2777628a91448188cd078cf67d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121062583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b49c0d64542addfe590dce7859e8960ce069173dd49f639bbec46d9b94e852`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add34357f4f4858d18f0a5bd6092a9c1bd7674b662698b850394d4d0af210905`  
		Last Modified: Sat, 02 Dec 2023 06:57:05 GMT  
		Size: 39.6 MB (39568969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9052de6ef0a399bdc1c5744c4964cc14e0667484a5207dda98457f223cd9457f`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a205bfdec17294941dbef5f1d11eaadfc3e61410195d13f16913b490c97ed5bd`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19537ca6e2aba26690dc6a9c04f40faa6930c24187c68c73a7b94f4cca29b08f`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ad32ae6b291e0844576f4b49d31d70aa4971b61d92bf595440bc44b52fe86c8`  
		Last Modified: Sat, 02 Dec 2023 08:56:25 GMT  
		Size: 8.9 MB (8865665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6ca144df34f09f11ce7e0013464923d061207ef4bad316d8bf8350de304ad8e`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 1.1 MB (1067806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41bf2a99a0eaf16e6f4db46434da577f028fa4415019eb2febfc4b43fbf7f04c`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 31.3 MB (31296841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02bff7b2151d3fe757b1374f7aad705dc2d01d976e8e262d01b445ec43d8d7bc`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e2bb2487bee034ff72cfcb92456f165947623fb7ad2323b02661632af2e5fca`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3` - unknown; unknown

```console
$ docker pull cassandra@sha256:8a9b098e5219fb8bdbb8c400cee674725756b27d31d9e98d6e05c5be14b9c6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3713972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f94e26f9669ec6e02cc835a3651c21b8a3d95ecd67cfe0b3dabaa6312658ea4`

```dockerfile
```

-	Layers:
	-	`sha256:a8d165be04a1f375503d4009d5b23d3d1a6d4caa7faf10b8bb3df56059e4407f`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 3.7 MB (3674945 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b2a479fdbfa2a473bf307cffede5558799dfc87a1b084d2663ba838eb6db715e`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 39.0 KB (39027 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7a074295daa3d1fb9b0749262bafad146fafad9569f2476a2e8e3b694f126cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126709329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce0e5d221894c15e028a9c86d719250c938d29d4174bf9a9d13b89031175a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b65be34d922977c68b3d2922ba5a28a8a1bb81f103182ce981f6ab54c443fc5`  
		Last Modified: Thu, 02 Nov 2023 01:40:59 GMT  
		Size: 40.8 MB (40844004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4852ce151327f164d04a7d792edf8bba87cfaa7a568f7dd64b4989a4190acc6f`  
		Last Modified: Thu, 02 Nov 2023 01:40:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:feb88cebfe26dac8dd830f6d817b5af4d1a784626de1421e73809166b0ad0a4f`  
		Last Modified: Thu, 02 Nov 2023 01:40:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dab0a4accad0bcba0edcfa4c5e57d0860cae6cdd65db8eb5923a0b6880a36b`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd4e3e4873dac6a6d2e4d6049850f00465fb3524000ee1c34f0b9a7693925bb`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 9.6 MB (9565067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6165b2a52b0a055c89b91d3940c8e81d1fef56ed5f49b12b9ddf9a2aab8cd3`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 1.0 MB (1031614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0e1de43786638ced434127a37e4f1949b91ddf97d878b2155bc932d484c2f09`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 31.3 MB (31296951 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c62a9d034e2be7e58e3681eb33792ab28e8652fd3842c21083951d115fb9c57`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef62c7b8c551fe1b38007a2950a61543bc9ccb580ce5eb4b57d35c3cdb79b39c`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3` - unknown; unknown

```console
$ docker pull cassandra@sha256:3dee2ea9f11cd69d4027e628908f5a11e993316504b746a337b53859fe85fe6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3706248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168a6c52b663eee89fa12440877cece484c9a0c68671528a9853d1967f201f9`

```dockerfile
```

-	Layers:
	-	`sha256:daaf8b077ce233f1baba71015a7ff6d699f27b06036111a016273e7ea0804411`  
		Last Modified: Wed, 08 Nov 2023 20:49:41 GMT  
		Size: 3.7 MB (3667329 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbbe75ba8586cd329dc851782e83e014df3e9b9e3a1ab7f3ba863611104932f0`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 38.9 KB (38919 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3` - linux; ppc64le

```console
$ docker pull cassandra@sha256:6a02b22ece20fd5791027a8e9100cdd47883f090c8f58a3c132921eaf695b3ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135504958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e0aa0075c5caa4b1fb1ed5eb889893d04f973cd0aa9ab2e3e2abcb9efbf631`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef48306773a0bdb363186b810d0120257d5d9b862a91388325edee347e4eaeac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 41.2 MB (41237488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b604ea7b5a801e6fef16fc68700da7e8f9ede4a116e199399284fc273d5e8792`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29fe6621f51b45ac766fcc71879785583559b67c63b92035f9c1458c190aa712`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9766c328340ea6206d9db8b4d46ec2e8261673a71504f9b22b04816f806244`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b80acea86df127da3fcf79b0c3e6a15b6588937aa9ed6b8d72d9d7fed59f509`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 10.4 MB (10416603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:825aa4f8a66075aa42f61fe42d2683dd0283f7c197804ecb401ca7a8a1006622`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 1.0 MB (1021075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48e9e39560c8b3397be4a57e6bf5cf9587e3a401d973567df428459a8b5ef8f0`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 31.3 MB (31296915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2598fe8eae0c7566de980f63734f002fc2e6865a5aa5afc08051c01201e22c16`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f55f77d18a0ab492638b5cd48bb16b69c211aa1ccd3d0188c98485a24fd5bdbc`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3` - unknown; unknown

```console
$ docker pull cassandra@sha256:a068794206fcc445464ca2e7e2f03405182209c0c60b3a946000ef844d9c5d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3711839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742713831342bbf726faf951ed4b6183e2304e05740459a87dd484f101d32c6c`

```dockerfile
```

-	Layers:
	-	`sha256:1541064450810e38d5e14b62583d573dbf5ef75628f9332201f87184ac901795`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 3.7 MB (3672883 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3435498f728770adcdb573144fa40329ab0159edbfa3653efb24f59a417c8bd1`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 39.0 KB (38956 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:3.0`

```console
$ docker pull cassandra@sha256:472a5f3f49ac146a0ea78e5288fe435873fa58eeeca9f6f9f5d419d872db48fa
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `cassandra:3.0` - linux; amd64

```console
$ docker pull cassandra@sha256:326b8799a6fac75cd5b276a748e9072824f32482d27e40e10eb7c9a7a7e25c17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124933744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8ed7176bc97913c770c40cc62681ebacd4ab760837a0ce0c34fde59799c491`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4241c3cdc52ee7f775d335ffcb8d963485f199febc690674ba3ccaa77d3e2a5`  
		Last Modified: Sat, 02 Dec 2023 02:04:08 GMT  
		Size: 41.9 MB (41859127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a10156a9e03d1fca1fcd43e32a20a1d167252ae7541aecd574b434bb290d3a60`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c346f95791868709d38488a14ea95739281acbd48a11a99b59fdb605e0dc7b7a`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bfa426e39b9a834a8ad8bd2803732e8d8ed4b28c149e97794494da0004e5668`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7971b7bba1df9dc69907481aa73a9dca77fac284ce518c97cd9c6f0069b1ac29`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 9.5 MB (9518545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65070291dd76764a344f1aa73c2b0e67102c8a0775e0dfa406858f65274f588c`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.1 MB (1100005 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ab94741c5675fbfd0ba2c564b5bc369d2651b6b8ab417bc30ff3b0bbcbc936c`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 26.9 MB (26947907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6b7ce6104955f8fd4543917e89b7235d681ab391e6e45f8490b55bbc4c67240`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 1.2 KB (1226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0a91060250a78143b35f83d0f7aed82fae41c9f8fb50843b154a0de5a27895c`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:b2a54d97f2c215b673ee68bd90fd3e3a14b9f7e656155c3d2fe15c6151368353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3701071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c51d9af794621ba0f44f6bde405b8d298c6763da804c6052e120f41d673425d`

```dockerfile
```

-	Layers:
	-	`sha256:d2cb00a0ae9985b3785aae7445aa0a2878d0cabb0f961a0e498c53c5ef475d2a`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 3.7 MB (3662439 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:38d3b628a8d20f74c0b1c3c528e42ee16220a56a483dfcd610d89983879f88f3`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 38.6 KB (38632 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:61177c59106e88db2e226d07835d693484974b3049924e4e309152be0a96f310
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116714144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98e3a61eebbd7fbdb435d4f924e650e001df536f82f89d42176b3e2c3de610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add34357f4f4858d18f0a5bd6092a9c1bd7674b662698b850394d4d0af210905`  
		Last Modified: Sat, 02 Dec 2023 06:57:05 GMT  
		Size: 39.6 MB (39568969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9052de6ef0a399bdc1c5744c4964cc14e0667484a5207dda98457f223cd9457f`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a205bfdec17294941dbef5f1d11eaadfc3e61410195d13f16913b490c97ed5bd`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19537ca6e2aba26690dc6a9c04f40faa6930c24187c68c73a7b94f4cca29b08f`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ad32ae6b291e0844576f4b49d31d70aa4971b61d92bf595440bc44b52fe86c8`  
		Last Modified: Sat, 02 Dec 2023 08:56:25 GMT  
		Size: 8.9 MB (8865665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6ca144df34f09f11ce7e0013464923d061207ef4bad316d8bf8350de304ad8e`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 1.1 MB (1067806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ee5e7025243b66f7ee28cfae197234989a1e29942aeaf397cad287adeaa806a`  
		Last Modified: Sat, 02 Dec 2023 08:57:15 GMT  
		Size: 26.9 MB (26948404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53c8770fae0f48ecc96ad952a34c409aba2a69b3f31c5585e79ce77744a1d26`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d333db6fae6a7ec0443f575fbc262a3ed1f8e4f3d614c7d00f97f914318c2c9`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:12cff8858e12596edae8dffe5e761305a778a55c494f5c4cc7b4c882a0b71f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3706290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d6edc8a204fec0afdeb2be298add05bb43b0775e820c886ccd7156f7a8347f`

```dockerfile
```

-	Layers:
	-	`sha256:e7af363af5ccfd98e611238807efe2e7def55aff91eaf809175e22f9831218e0`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 3.7 MB (3668369 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ca99c5e565117e312f7066e1c9df9f1406e59374ff74ea8109e1a852d6ac722b`  
		Last Modified: Sat, 02 Dec 2023 08:57:13 GMT  
		Size: 37.9 KB (37921 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:d37dc460daac657099401038f503f9c1e87c9508c1852f6394b1970be7da4823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122360780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcc8bd4c4a817ef0acdaafcc5babc24c8fef921a0be7ca3779f11dfab4b95af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b65be34d922977c68b3d2922ba5a28a8a1bb81f103182ce981f6ab54c443fc5`  
		Last Modified: Thu, 02 Nov 2023 01:40:59 GMT  
		Size: 40.8 MB (40844004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4852ce151327f164d04a7d792edf8bba87cfaa7a568f7dd64b4989a4190acc6f`  
		Last Modified: Thu, 02 Nov 2023 01:40:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:feb88cebfe26dac8dd830f6d817b5af4d1a784626de1421e73809166b0ad0a4f`  
		Last Modified: Thu, 02 Nov 2023 01:40:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dab0a4accad0bcba0edcfa4c5e57d0860cae6cdd65db8eb5923a0b6880a36b`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd4e3e4873dac6a6d2e4d6049850f00465fb3524000ee1c34f0b9a7693925bb`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 9.6 MB (9565067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6165b2a52b0a055c89b91d3940c8e81d1fef56ed5f49b12b9ddf9a2aab8cd3`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 1.0 MB (1031614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2437a79910c5edab107f1efa184b8d0990fb2b9c11543f4e0d7d9a247abdd51f`  
		Last Modified: Wed, 08 Nov 2023 20:50:20 GMT  
		Size: 26.9 MB (26948405 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e573abec3152ee2832f8071f8b614f15b7f612a9c2c5702753afa4277e5360c5`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7593cd69555903246ff22311584e8a55147b49e81bd7e78dbf3493dffe357b28`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:188c9134a6d02fd670ae3e13a9a01a49d3f2ddcb89e424efe908fc5f4586cc5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3698658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83abf62114031d68deb8e806c476f7a0c22ded9438b98b2b7b83b320d37bf5a`

```dockerfile
```

-	Layers:
	-	`sha256:87b60530c46c9d25870e4cbd3ebdf462bd8cc0fe7d5c4d27dfad3bd5eb9f1e9a`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 3.7 MB (3660837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ea34aac0eb4d2621eb0fee7a372386eb57e7f5510a6c552c7e4193098c63938c`  
		Last Modified: Wed, 08 Nov 2023 20:50:18 GMT  
		Size: 37.8 KB (37821 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:d22a9f8a0b87244722d401829797c8557167128b551ba0cff8347c47d3dc4f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131156533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f28b9ae24ba56f699f0bfeec4407d0eea05e019de74c86c003c2f8cad62b88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef48306773a0bdb363186b810d0120257d5d9b862a91388325edee347e4eaeac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 41.2 MB (41237488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b604ea7b5a801e6fef16fc68700da7e8f9ede4a116e199399284fc273d5e8792`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29fe6621f51b45ac766fcc71879785583559b67c63b92035f9c1458c190aa712`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9766c328340ea6206d9db8b4d46ec2e8261673a71504f9b22b04816f806244`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b80acea86df127da3fcf79b0c3e6a15b6588937aa9ed6b8d72d9d7fed59f509`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 10.4 MB (10416603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:825aa4f8a66075aa42f61fe42d2683dd0283f7c197804ecb401ca7a8a1006622`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 1.0 MB (1021075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c2590434990b220776953fcb8df7eae1c07d59943f2795d8bf6aece0d61189b`  
		Last Modified: Sat, 02 Dec 2023 11:54:08 GMT  
		Size: 26.9 MB (26948492 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92ff16e60aeadaf2d79c2676b52d2cc7e85a318192d6b527d0c502c6dc289ce1`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2190f9cf0fcc2a46c4a87c84fcf826e4448c8a12f193f7c87e55c4a346853bc`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:b307c277df80b12300e0ff5e0377557c9bde739a6f7487f2147df5f0fb0fef1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3704163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3169b66ca473b3f3a8403d4db44d30d5a1ce4bcd754b2748e3fbaf14d2de335e`

```dockerfile
```

-	Layers:
	-	`sha256:6abd13797052b01aadb7864788adad9d8e032679d439a861c912e0d9b31525bd`  
		Last Modified: Sat, 02 Dec 2023 11:54:03 GMT  
		Size: 3.7 MB (3666309 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc59ff613021401c253a620ee2d29997024f0107348070246239c05cf4c4164e`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 37.9 KB (37854 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:3.0.29`

```console
$ docker pull cassandra@sha256:472a5f3f49ac146a0ea78e5288fe435873fa58eeeca9f6f9f5d419d872db48fa
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `cassandra:3.0.29` - linux; amd64

```console
$ docker pull cassandra@sha256:326b8799a6fac75cd5b276a748e9072824f32482d27e40e10eb7c9a7a7e25c17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124933744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8ed7176bc97913c770c40cc62681ebacd4ab760837a0ce0c34fde59799c491`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4241c3cdc52ee7f775d335ffcb8d963485f199febc690674ba3ccaa77d3e2a5`  
		Last Modified: Sat, 02 Dec 2023 02:04:08 GMT  
		Size: 41.9 MB (41859127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a10156a9e03d1fca1fcd43e32a20a1d167252ae7541aecd574b434bb290d3a60`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c346f95791868709d38488a14ea95739281acbd48a11a99b59fdb605e0dc7b7a`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bfa426e39b9a834a8ad8bd2803732e8d8ed4b28c149e97794494da0004e5668`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7971b7bba1df9dc69907481aa73a9dca77fac284ce518c97cd9c6f0069b1ac29`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 9.5 MB (9518545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65070291dd76764a344f1aa73c2b0e67102c8a0775e0dfa406858f65274f588c`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.1 MB (1100005 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ab94741c5675fbfd0ba2c564b5bc369d2651b6b8ab417bc30ff3b0bbcbc936c`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 26.9 MB (26947907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6b7ce6104955f8fd4543917e89b7235d681ab391e6e45f8490b55bbc4c67240`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 1.2 KB (1226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0a91060250a78143b35f83d0f7aed82fae41c9f8fb50843b154a0de5a27895c`  
		Last Modified: Sat, 02 Dec 2023 03:12:29 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0.29` - unknown; unknown

```console
$ docker pull cassandra@sha256:b2a54d97f2c215b673ee68bd90fd3e3a14b9f7e656155c3d2fe15c6151368353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3701071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c51d9af794621ba0f44f6bde405b8d298c6763da804c6052e120f41d673425d`

```dockerfile
```

-	Layers:
	-	`sha256:d2cb00a0ae9985b3785aae7445aa0a2878d0cabb0f961a0e498c53c5ef475d2a`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 3.7 MB (3662439 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:38d3b628a8d20f74c0b1c3c528e42ee16220a56a483dfcd610d89983879f88f3`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 38.6 KB (38632 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0.29` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:61177c59106e88db2e226d07835d693484974b3049924e4e309152be0a96f310
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116714144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98e3a61eebbd7fbdb435d4f924e650e001df536f82f89d42176b3e2c3de610f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add34357f4f4858d18f0a5bd6092a9c1bd7674b662698b850394d4d0af210905`  
		Last Modified: Sat, 02 Dec 2023 06:57:05 GMT  
		Size: 39.6 MB (39568969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9052de6ef0a399bdc1c5744c4964cc14e0667484a5207dda98457f223cd9457f`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a205bfdec17294941dbef5f1d11eaadfc3e61410195d13f16913b490c97ed5bd`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19537ca6e2aba26690dc6a9c04f40faa6930c24187c68c73a7b94f4cca29b08f`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ad32ae6b291e0844576f4b49d31d70aa4971b61d92bf595440bc44b52fe86c8`  
		Last Modified: Sat, 02 Dec 2023 08:56:25 GMT  
		Size: 8.9 MB (8865665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6ca144df34f09f11ce7e0013464923d061207ef4bad316d8bf8350de304ad8e`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 1.1 MB (1067806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ee5e7025243b66f7ee28cfae197234989a1e29942aeaf397cad287adeaa806a`  
		Last Modified: Sat, 02 Dec 2023 08:57:15 GMT  
		Size: 26.9 MB (26948404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53c8770fae0f48ecc96ad952a34c409aba2a69b3f31c5585e79ce77744a1d26`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d333db6fae6a7ec0443f575fbc262a3ed1f8e4f3d614c7d00f97f914318c2c9`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0.29` - unknown; unknown

```console
$ docker pull cassandra@sha256:12cff8858e12596edae8dffe5e761305a778a55c494f5c4cc7b4c882a0b71f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3706290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d6edc8a204fec0afdeb2be298add05bb43b0775e820c886ccd7156f7a8347f`

```dockerfile
```

-	Layers:
	-	`sha256:e7af363af5ccfd98e611238807efe2e7def55aff91eaf809175e22f9831218e0`  
		Last Modified: Sat, 02 Dec 2023 08:57:14 GMT  
		Size: 3.7 MB (3668369 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ca99c5e565117e312f7066e1c9df9f1406e59374ff74ea8109e1a852d6ac722b`  
		Last Modified: Sat, 02 Dec 2023 08:57:13 GMT  
		Size: 37.9 KB (37921 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0.29` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:d37dc460daac657099401038f503f9c1e87c9508c1852f6394b1970be7da4823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122360780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcc8bd4c4a817ef0acdaafcc5babc24c8fef921a0be7ca3779f11dfab4b95af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b65be34d922977c68b3d2922ba5a28a8a1bb81f103182ce981f6ab54c443fc5`  
		Last Modified: Thu, 02 Nov 2023 01:40:59 GMT  
		Size: 40.8 MB (40844004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4852ce151327f164d04a7d792edf8bba87cfaa7a568f7dd64b4989a4190acc6f`  
		Last Modified: Thu, 02 Nov 2023 01:40:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:feb88cebfe26dac8dd830f6d817b5af4d1a784626de1421e73809166b0ad0a4f`  
		Last Modified: Thu, 02 Nov 2023 01:40:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dab0a4accad0bcba0edcfa4c5e57d0860cae6cdd65db8eb5923a0b6880a36b`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd4e3e4873dac6a6d2e4d6049850f00465fb3524000ee1c34f0b9a7693925bb`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 9.6 MB (9565067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6165b2a52b0a055c89b91d3940c8e81d1fef56ed5f49b12b9ddf9a2aab8cd3`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 1.0 MB (1031614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2437a79910c5edab107f1efa184b8d0990fb2b9c11543f4e0d7d9a247abdd51f`  
		Last Modified: Wed, 08 Nov 2023 20:50:20 GMT  
		Size: 26.9 MB (26948405 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e573abec3152ee2832f8071f8b614f15b7f612a9c2c5702753afa4277e5360c5`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7593cd69555903246ff22311584e8a55147b49e81bd7e78dbf3493dffe357b28`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0.29` - unknown; unknown

```console
$ docker pull cassandra@sha256:188c9134a6d02fd670ae3e13a9a01a49d3f2ddcb89e424efe908fc5f4586cc5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3698658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83abf62114031d68deb8e806c476f7a0c22ded9438b98b2b7b83b320d37bf5a`

```dockerfile
```

-	Layers:
	-	`sha256:87b60530c46c9d25870e4cbd3ebdf462bd8cc0fe7d5c4d27dfad3bd5eb9f1e9a`  
		Last Modified: Wed, 08 Nov 2023 20:50:19 GMT  
		Size: 3.7 MB (3660837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ea34aac0eb4d2621eb0fee7a372386eb57e7f5510a6c552c7e4193098c63938c`  
		Last Modified: Wed, 08 Nov 2023 20:50:18 GMT  
		Size: 37.8 KB (37821 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.0.29` - linux; ppc64le

```console
$ docker pull cassandra@sha256:d22a9f8a0b87244722d401829797c8557167128b551ba0cff8347c47d3dc4f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131156533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f28b9ae24ba56f699f0bfeec4407d0eea05e019de74c86c003c2f8cad62b88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 15 May 2023 20:24:10 GMT
ARG RELEASE
# Mon, 15 May 2023 20:24:10 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 15 May 2023 20:24:10 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 15 May 2023 20:24:10 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 15 May 2023 20:24:10 GMT
CMD ["/bin/bash"]
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 15 May 2023 20:24:10 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Mon, 15 May 2023 20:24:10 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV GOSU_VERSION=1.16
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 15 May 2023 20:24:10 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 20:24:10 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_VERSION=3.0.29
# Mon, 15 May 2023 20:24:10 GMT
ENV CASSANDRA_SHA512=31515e20fb1356ae8cf277c52954ea711c4e158f852cd8bee096775f1f0a2b6847fe972d4755f061b45578f7ed688237b8ead84b38c77bcccfd6f8c022db520b
# Mon, 15 May 2023 20:24:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; 			sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 			grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 15 May 2023 20:24:10 GMT
VOLUME [/var/lib/cassandra]
# Mon, 15 May 2023 20:24:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 15 May 2023 20:24:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Mon, 15 May 2023 20:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 20:24:10 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 15 May 2023 20:24:10 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef48306773a0bdb363186b810d0120257d5d9b862a91388325edee347e4eaeac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 41.2 MB (41237488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b604ea7b5a801e6fef16fc68700da7e8f9ede4a116e199399284fc273d5e8792`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29fe6621f51b45ac766fcc71879785583559b67c63b92035f9c1458c190aa712`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9766c328340ea6206d9db8b4d46ec2e8261673a71504f9b22b04816f806244`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b80acea86df127da3fcf79b0c3e6a15b6588937aa9ed6b8d72d9d7fed59f509`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 10.4 MB (10416603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:825aa4f8a66075aa42f61fe42d2683dd0283f7c197804ecb401ca7a8a1006622`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 1.0 MB (1021075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c2590434990b220776953fcb8df7eae1c07d59943f2795d8bf6aece0d61189b`  
		Last Modified: Sat, 02 Dec 2023 11:54:08 GMT  
		Size: 26.9 MB (26948492 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92ff16e60aeadaf2d79c2676b52d2cc7e85a318192d6b527d0c502c6dc289ce1`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2190f9cf0fcc2a46c4a87c84fcf826e4448c8a12f193f7c87e55c4a346853bc`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.0.29` - unknown; unknown

```console
$ docker pull cassandra@sha256:b307c277df80b12300e0ff5e0377557c9bde739a6f7487f2147df5f0fb0fef1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3704163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3169b66ca473b3f3a8403d4db44d30d5a1ce4bcd754b2748e3fbaf14d2de335e`

```dockerfile
```

-	Layers:
	-	`sha256:6abd13797052b01aadb7864788adad9d8e032679d439a861c912e0d9b31525bd`  
		Last Modified: Sat, 02 Dec 2023 11:54:03 GMT  
		Size: 3.7 MB (3666309 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc59ff613021401c253a620ee2d29997024f0107348070246239c05cf4c4164e`  
		Last Modified: Sat, 02 Dec 2023 11:54:02 GMT  
		Size: 37.9 KB (37854 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:3.11`

```console
$ docker pull cassandra@sha256:5ed40beccc441bfe2c92e34f77f85ea4cdb715ce3580db4f3dbb36b91c269a91
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `cassandra:3.11` - linux; amd64

```console
$ docker pull cassandra@sha256:0d1bc6bb301d65ac9e6d73db66e4917e20d3839120ae67bb2a2bfce485d828ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129282302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e54a193f218f067ed8b55fc7dfd4a011af7cbbbbe50905d07ec2569af303795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4241c3cdc52ee7f775d335ffcb8d963485f199febc690674ba3ccaa77d3e2a5`  
		Last Modified: Sat, 02 Dec 2023 02:04:08 GMT  
		Size: 41.9 MB (41859127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a10156a9e03d1fca1fcd43e32a20a1d167252ae7541aecd574b434bb290d3a60`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c346f95791868709d38488a14ea95739281acbd48a11a99b59fdb605e0dc7b7a`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15d171c8e9d4ca134db32442d3a8a993add09d01cfe7880b2c61907ea5fbef9b`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:233818e806d9e56db856a57eacf34d53604642a6b9f99ec9b67f0f2923bd396a`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 9.5 MB (9518587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b010d84521348cbc6a3f5b77ee7c7856fcb0ca47f6b6dafe681704a3c5d2648`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.1 MB (1099988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:828e728899969d374bd4b99929a609ff246e4993e036331a9dce0430fd2a1de9`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 31.3 MB (31296438 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4533533cf3bd3383c2f38ed7930e34081ae60b7e556c898fb090263f24bfbaa`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.2 KB (1226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:590be63dd82c42469d22d262a572aa0039cfdbb2fee9666a5168af5ca0930ada`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:06f1395b1461c62b396aeb3ac192ae766d46fdd9cf9033c8e3db44425e559781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3707920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31380b54407e8849332d97bddd2f28659533aebdb0aa0533027da01e709f2ea4`

```dockerfile
```

-	Layers:
	-	`sha256:0fb384eda8f2d11e1fc96f54f2032c20eba63beb20d79c18420db0911ea4b59b`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 3.7 MB (3669007 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18bea3a8a82a82ea743d45112c868c5d7c836df05336e444edec5a1f6afbe3b2`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 38.9 KB (38913 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:a6bd569e0d12b6b8155875873a502957b8ffd2777628a91448188cd078cf67d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121062583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b49c0d64542addfe590dce7859e8960ce069173dd49f639bbec46d9b94e852`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add34357f4f4858d18f0a5bd6092a9c1bd7674b662698b850394d4d0af210905`  
		Last Modified: Sat, 02 Dec 2023 06:57:05 GMT  
		Size: 39.6 MB (39568969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9052de6ef0a399bdc1c5744c4964cc14e0667484a5207dda98457f223cd9457f`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a205bfdec17294941dbef5f1d11eaadfc3e61410195d13f16913b490c97ed5bd`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19537ca6e2aba26690dc6a9c04f40faa6930c24187c68c73a7b94f4cca29b08f`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ad32ae6b291e0844576f4b49d31d70aa4971b61d92bf595440bc44b52fe86c8`  
		Last Modified: Sat, 02 Dec 2023 08:56:25 GMT  
		Size: 8.9 MB (8865665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6ca144df34f09f11ce7e0013464923d061207ef4bad316d8bf8350de304ad8e`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 1.1 MB (1067806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41bf2a99a0eaf16e6f4db46434da577f028fa4415019eb2febfc4b43fbf7f04c`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 31.3 MB (31296841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02bff7b2151d3fe757b1374f7aad705dc2d01d976e8e262d01b445ec43d8d7bc`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e2bb2487bee034ff72cfcb92456f165947623fb7ad2323b02661632af2e5fca`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:8a9b098e5219fb8bdbb8c400cee674725756b27d31d9e98d6e05c5be14b9c6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3713972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f94e26f9669ec6e02cc835a3651c21b8a3d95ecd67cfe0b3dabaa6312658ea4`

```dockerfile
```

-	Layers:
	-	`sha256:a8d165be04a1f375503d4009d5b23d3d1a6d4caa7faf10b8bb3df56059e4407f`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 3.7 MB (3674945 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b2a479fdbfa2a473bf307cffede5558799dfc87a1b084d2663ba838eb6db715e`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 39.0 KB (39027 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7a074295daa3d1fb9b0749262bafad146fafad9569f2476a2e8e3b694f126cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126709329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce0e5d221894c15e028a9c86d719250c938d29d4174bf9a9d13b89031175a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b65be34d922977c68b3d2922ba5a28a8a1bb81f103182ce981f6ab54c443fc5`  
		Last Modified: Thu, 02 Nov 2023 01:40:59 GMT  
		Size: 40.8 MB (40844004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4852ce151327f164d04a7d792edf8bba87cfaa7a568f7dd64b4989a4190acc6f`  
		Last Modified: Thu, 02 Nov 2023 01:40:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:feb88cebfe26dac8dd830f6d817b5af4d1a784626de1421e73809166b0ad0a4f`  
		Last Modified: Thu, 02 Nov 2023 01:40:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dab0a4accad0bcba0edcfa4c5e57d0860cae6cdd65db8eb5923a0b6880a36b`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd4e3e4873dac6a6d2e4d6049850f00465fb3524000ee1c34f0b9a7693925bb`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 9.6 MB (9565067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6165b2a52b0a055c89b91d3940c8e81d1fef56ed5f49b12b9ddf9a2aab8cd3`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 1.0 MB (1031614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0e1de43786638ced434127a37e4f1949b91ddf97d878b2155bc932d484c2f09`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 31.3 MB (31296951 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c62a9d034e2be7e58e3681eb33792ab28e8652fd3842c21083951d115fb9c57`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef62c7b8c551fe1b38007a2950a61543bc9ccb580ce5eb4b57d35c3cdb79b39c`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:3dee2ea9f11cd69d4027e628908f5a11e993316504b746a337b53859fe85fe6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3706248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168a6c52b663eee89fa12440877cece484c9a0c68671528a9853d1967f201f9`

```dockerfile
```

-	Layers:
	-	`sha256:daaf8b077ce233f1baba71015a7ff6d699f27b06036111a016273e7ea0804411`  
		Last Modified: Wed, 08 Nov 2023 20:49:41 GMT  
		Size: 3.7 MB (3667329 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbbe75ba8586cd329dc851782e83e014df3e9b9e3a1ab7f3ba863611104932f0`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 38.9 KB (38919 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11` - linux; ppc64le

```console
$ docker pull cassandra@sha256:6a02b22ece20fd5791027a8e9100cdd47883f090c8f58a3c132921eaf695b3ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135504958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e0aa0075c5caa4b1fb1ed5eb889893d04f973cd0aa9ab2e3e2abcb9efbf631`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef48306773a0bdb363186b810d0120257d5d9b862a91388325edee347e4eaeac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 41.2 MB (41237488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b604ea7b5a801e6fef16fc68700da7e8f9ede4a116e199399284fc273d5e8792`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29fe6621f51b45ac766fcc71879785583559b67c63b92035f9c1458c190aa712`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9766c328340ea6206d9db8b4d46ec2e8261673a71504f9b22b04816f806244`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b80acea86df127da3fcf79b0c3e6a15b6588937aa9ed6b8d72d9d7fed59f509`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 10.4 MB (10416603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:825aa4f8a66075aa42f61fe42d2683dd0283f7c197804ecb401ca7a8a1006622`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 1.0 MB (1021075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48e9e39560c8b3397be4a57e6bf5cf9587e3a401d973567df428459a8b5ef8f0`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 31.3 MB (31296915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2598fe8eae0c7566de980f63734f002fc2e6865a5aa5afc08051c01201e22c16`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f55f77d18a0ab492638b5cd48bb16b69c211aa1ccd3d0188c98485a24fd5bdbc`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:a068794206fcc445464ca2e7e2f03405182209c0c60b3a946000ef844d9c5d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3711839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742713831342bbf726faf951ed4b6183e2304e05740459a87dd484f101d32c6c`

```dockerfile
```

-	Layers:
	-	`sha256:1541064450810e38d5e14b62583d573dbf5ef75628f9332201f87184ac901795`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 3.7 MB (3672883 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3435498f728770adcdb573144fa40329ab0159edbfa3653efb24f59a417c8bd1`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 39.0 KB (38956 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:3.11.16`

```console
$ docker pull cassandra@sha256:5ed40beccc441bfe2c92e34f77f85ea4cdb715ce3580db4f3dbb36b91c269a91
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `cassandra:3.11.16` - linux; amd64

```console
$ docker pull cassandra@sha256:0d1bc6bb301d65ac9e6d73db66e4917e20d3839120ae67bb2a2bfce485d828ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129282302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e54a193f218f067ed8b55fc7dfd4a011af7cbbbbe50905d07ec2569af303795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4241c3cdc52ee7f775d335ffcb8d963485f199febc690674ba3ccaa77d3e2a5`  
		Last Modified: Sat, 02 Dec 2023 02:04:08 GMT  
		Size: 41.9 MB (41859127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a10156a9e03d1fca1fcd43e32a20a1d167252ae7541aecd574b434bb290d3a60`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c346f95791868709d38488a14ea95739281acbd48a11a99b59fdb605e0dc7b7a`  
		Last Modified: Sat, 02 Dec 2023 02:04:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15d171c8e9d4ca134db32442d3a8a993add09d01cfe7880b2c61907ea5fbef9b`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:233818e806d9e56db856a57eacf34d53604642a6b9f99ec9b67f0f2923bd396a`  
		Last Modified: Sat, 02 Dec 2023 03:12:27 GMT  
		Size: 9.5 MB (9518587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b010d84521348cbc6a3f5b77ee7c7856fcb0ca47f6b6dafe681704a3c5d2648`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.1 MB (1099988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:828e728899969d374bd4b99929a609ff246e4993e036331a9dce0430fd2a1de9`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 31.3 MB (31296438 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4533533cf3bd3383c2f38ed7930e34081ae60b7e556c898fb090263f24bfbaa`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 1.2 KB (1226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:590be63dd82c42469d22d262a572aa0039cfdbb2fee9666a5168af5ca0930ada`  
		Last Modified: Sat, 02 Dec 2023 03:12:28 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11.16` - unknown; unknown

```console
$ docker pull cassandra@sha256:06f1395b1461c62b396aeb3ac192ae766d46fdd9cf9033c8e3db44425e559781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3707920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31380b54407e8849332d97bddd2f28659533aebdb0aa0533027da01e709f2ea4`

```dockerfile
```

-	Layers:
	-	`sha256:0fb384eda8f2d11e1fc96f54f2032c20eba63beb20d79c18420db0911ea4b59b`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 3.7 MB (3669007 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18bea3a8a82a82ea743d45112c868c5d7c836df05336e444edec5a1f6afbe3b2`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 38.9 KB (38913 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11.16` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:a6bd569e0d12b6b8155875873a502957b8ffd2777628a91448188cd078cf67d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121062583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b49c0d64542addfe590dce7859e8960ce069173dd49f639bbec46d9b94e852`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add34357f4f4858d18f0a5bd6092a9c1bd7674b662698b850394d4d0af210905`  
		Last Modified: Sat, 02 Dec 2023 06:57:05 GMT  
		Size: 39.6 MB (39568969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9052de6ef0a399bdc1c5744c4964cc14e0667484a5207dda98457f223cd9457f`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a205bfdec17294941dbef5f1d11eaadfc3e61410195d13f16913b490c97ed5bd`  
		Last Modified: Sat, 02 Dec 2023 06:57:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19537ca6e2aba26690dc6a9c04f40faa6930c24187c68c73a7b94f4cca29b08f`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ad32ae6b291e0844576f4b49d31d70aa4971b61d92bf595440bc44b52fe86c8`  
		Last Modified: Sat, 02 Dec 2023 08:56:25 GMT  
		Size: 8.9 MB (8865665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6ca144df34f09f11ce7e0013464923d061207ef4bad316d8bf8350de304ad8e`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 1.1 MB (1067806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41bf2a99a0eaf16e6f4db46434da577f028fa4415019eb2febfc4b43fbf7f04c`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 31.3 MB (31296841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02bff7b2151d3fe757b1374f7aad705dc2d01d976e8e262d01b445ec43d8d7bc`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e2bb2487bee034ff72cfcb92456f165947623fb7ad2323b02661632af2e5fca`  
		Last Modified: Sat, 02 Dec 2023 08:56:26 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11.16` - unknown; unknown

```console
$ docker pull cassandra@sha256:8a9b098e5219fb8bdbb8c400cee674725756b27d31d9e98d6e05c5be14b9c6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3713972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f94e26f9669ec6e02cc835a3651c21b8a3d95ecd67cfe0b3dabaa6312658ea4`

```dockerfile
```

-	Layers:
	-	`sha256:a8d165be04a1f375503d4009d5b23d3d1a6d4caa7faf10b8bb3df56059e4407f`  
		Last Modified: Sat, 02 Dec 2023 08:56:24 GMT  
		Size: 3.7 MB (3674945 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b2a479fdbfa2a473bf307cffede5558799dfc87a1b084d2663ba838eb6db715e`  
		Last Modified: Sat, 02 Dec 2023 08:56:23 GMT  
		Size: 39.0 KB (39027 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11.16` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:7a074295daa3d1fb9b0749262bafad146fafad9569f2476a2e8e3b694f126cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126709329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ce0e5d221894c15e028a9c86d719250c938d29d4174bf9a9d13b89031175a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b65be34d922977c68b3d2922ba5a28a8a1bb81f103182ce981f6ab54c443fc5`  
		Last Modified: Thu, 02 Nov 2023 01:40:59 GMT  
		Size: 40.8 MB (40844004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4852ce151327f164d04a7d792edf8bba87cfaa7a568f7dd64b4989a4190acc6f`  
		Last Modified: Thu, 02 Nov 2023 01:40:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:feb88cebfe26dac8dd830f6d817b5af4d1a784626de1421e73809166b0ad0a4f`  
		Last Modified: Thu, 02 Nov 2023 01:40:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dab0a4accad0bcba0edcfa4c5e57d0860cae6cdd65db8eb5923a0b6880a36b`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dd4e3e4873dac6a6d2e4d6049850f00465fb3524000ee1c34f0b9a7693925bb`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 9.6 MB (9565067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6165b2a52b0a055c89b91d3940c8e81d1fef56ed5f49b12b9ddf9a2aab8cd3`  
		Last Modified: Wed, 08 Nov 2023 20:49:42 GMT  
		Size: 1.0 MB (1031614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0e1de43786638ced434127a37e4f1949b91ddf97d878b2155bc932d484c2f09`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 31.3 MB (31296951 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c62a9d034e2be7e58e3681eb33792ab28e8652fd3842c21083951d115fb9c57`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef62c7b8c551fe1b38007a2950a61543bc9ccb580ce5eb4b57d35c3cdb79b39c`  
		Last Modified: Wed, 08 Nov 2023 20:49:43 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11.16` - unknown; unknown

```console
$ docker pull cassandra@sha256:3dee2ea9f11cd69d4027e628908f5a11e993316504b746a337b53859fe85fe6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3706248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168a6c52b663eee89fa12440877cece484c9a0c68671528a9853d1967f201f9`

```dockerfile
```

-	Layers:
	-	`sha256:daaf8b077ce233f1baba71015a7ff6d699f27b06036111a016273e7ea0804411`  
		Last Modified: Wed, 08 Nov 2023 20:49:41 GMT  
		Size: 3.7 MB (3667329 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbbe75ba8586cd329dc851782e83e014df3e9b9e3a1ab7f3ba863611104932f0`  
		Last Modified: Wed, 08 Nov 2023 20:49:40 GMT  
		Size: 38.9 KB (38919 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:3.11.16` - linux; ppc64le

```console
$ docker pull cassandra@sha256:6a02b22ece20fd5791027a8e9100cdd47883f090c8f58a3c132921eaf695b3ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135504958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e0aa0075c5caa4b1fb1ed5eb889893d04f973cd0aa9ab2e3e2abcb9efbf631`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sun, 20 Aug 2023 14:24:17 GMT
ARG RELEASE
# Sun, 20 Aug 2023 14:24:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sun, 20 Aug 2023 14:24:17 GMT
LABEL org.opencontainers.image.version=20.04
# Sun, 20 Aug 2023 14:24:17 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["/bin/bash"]
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sun, 20 Aug 2023 14:24:17 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37b997f12cd572da979283fccafec9ba903041a209605b50fcb46cc34f1a9917';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='91d31027da0d985be3549714389593d9e0da3da5057d87e3831c7c538b9a2a0f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='877953bfabcdbcd000c11364d806456ca579a921085de2ca942280ebe168cac2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='0ecb0aeb54fb9d3c9e1a7ea411490127e8e298d93219fafc4dd6051a5b74671f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java -version"; java -version;     echo "Complete."
# Sun, 20 Aug 2023 14:24:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GOSU_VERSION=1.16
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sun, 20 Aug 2023 14:24:17 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Aug 2023 14:24:17 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_VERSION=3.11.16
# Sun, 20 Aug 2023 14:24:17 GMT
ENV CASSANDRA_SHA512=5bc76508fec8ff9d4fcfa3c53b0c9550ef37ad771e568b2634df2ba5377c378237c968f1d2bfb1078ecc30c034aea63b4c481826bb9ac26536f1f4f336cd8286
# Sun, 20 Aug 2023 14:24:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
VOLUME [/var/lib/cassandra]
# Sun, 20 Aug 2023 14:24:17 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat # buildkit
# Sun, 20 Aug 2023 14:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Aug 2023 14:24:17 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sun, 20 Aug 2023 14:24:17 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef48306773a0bdb363186b810d0120257d5d9b862a91388325edee347e4eaeac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 41.2 MB (41237488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b604ea7b5a801e6fef16fc68700da7e8f9ede4a116e199399284fc273d5e8792`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29fe6621f51b45ac766fcc71879785583559b67c63b92035f9c1458c190aa712`  
		Last Modified: Sat, 02 Dec 2023 06:15:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9766c328340ea6206d9db8b4d46ec2e8261673a71504f9b22b04816f806244`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b80acea86df127da3fcf79b0c3e6a15b6588937aa9ed6b8d72d9d7fed59f509`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 10.4 MB (10416603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:825aa4f8a66075aa42f61fe42d2683dd0283f7c197804ecb401ca7a8a1006622`  
		Last Modified: Sat, 02 Dec 2023 11:52:58 GMT  
		Size: 1.0 MB (1021075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48e9e39560c8b3397be4a57e6bf5cf9587e3a401d973567df428459a8b5ef8f0`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 31.3 MB (31296915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2598fe8eae0c7566de980f63734f002fc2e6865a5aa5afc08051c01201e22c16`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f55f77d18a0ab492638b5cd48bb16b69c211aa1ccd3d0188c98485a24fd5bdbc`  
		Last Modified: Sat, 02 Dec 2023 11:52:59 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:3.11.16` - unknown; unknown

```console
$ docker pull cassandra@sha256:a068794206fcc445464ca2e7e2f03405182209c0c60b3a946000ef844d9c5d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3711839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742713831342bbf726faf951ed4b6183e2304e05740459a87dd484f101d32c6c`

```dockerfile
```

-	Layers:
	-	`sha256:1541064450810e38d5e14b62583d573dbf5ef75628f9332201f87184ac901795`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 3.7 MB (3672883 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3435498f728770adcdb573144fa40329ab0159edbfa3653efb24f59a417c8bd1`  
		Last Modified: Sat, 02 Dec 2023 11:52:57 GMT  
		Size: 39.0 KB (38956 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:4`

```console
$ docker pull cassandra@sha256:e7f2a92533f24b3656aa1179df92cf95b7d16e45fa87f93fb7809cac757fd98a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:4` - linux; amd64

```console
$ docker pull cassandra@sha256:599be9b5e23f91edbc43598f7df994b53993d82ae65c2cc1aba9f0e5fa2af8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154749016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597c6621fd1dfe8ca2dafb7c39c3b6c113626cdfe8f7740708b6939b7936e2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6c48cef298b986e7cfd235b365ca20053fde3138d661e80c29fb4e0daa1fa88`  
		Last Modified: Sat, 02 Dec 2023 02:05:26 GMT  
		Size: 47.1 MB (47068582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b90bdd07aa688f6123bcef53bbaaf699cd0104995994b90787214abe494d2df`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa13e718ec7250f1c09858061de443dfd506a5c40a422d0586e57366a5dfada4`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed2030023c7b0aedadaa1f81c9305e6e17e83438572ec0884fb8b468f53b97db`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a9483292d0e0e03f0e6a4e628bc0b9dffb74b04fbf62e823ca3802e9cde789`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 10.9 MB (10934074 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:273a18c34b61cfe3e13656ced1129dcd8b59aa4013bd5c92a0cd0b44bd3b7a81`  
		Last Modified: Sat, 02 Dec 2023 03:12:37 GMT  
		Size: 1.1 MB (1098343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdd8f9e8894a325ee0a006affc7c485435db3076d4688cf1db04cf7b44e0fa9`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 50.1 MB (50139981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39c8fc1b3f62bcbcf45b2747bd2c71ace02f0e12b38bdb7d0707d957ebadfe3e`  
		Last Modified: Sat, 02 Dec 2023 03:12:38 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4` - unknown; unknown

```console
$ docker pull cassandra@sha256:996e0b0ef4446c0b10211489243681082f32635d8284f35f95c08e8cfe6ae040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc707d98d06138a1b15c81acec547ab76f41d9675f0e725062c1a67e0429ba3`

```dockerfile
```

-	Layers:
	-	`sha256:75341ea69fa2e930371db5f52ba7d03b30eab1a350ede59146677b62f622e2b7`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 3.6 MB (3590619 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6a00958cf9b8b16a6b18db001d4f649b0d940bce4cc639966bde0df1a492b3dc`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:bd55cb2c5542fba3670f0bb97a1d891d1c5580e9c572b63571f6768f5bebeec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146789764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d571f6a6cc6de91e550b452c934b01334beffffe5e54416391402e3d981121d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba8e2d5a27a6f19d95e0d48c8b46050091977649696cd2bffea1dd999165fa5`  
		Last Modified: Sat, 02 Dec 2023 08:54:23 GMT  
		Size: 50.1 MB (50139985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77ce296b72ba77e2e0a97284a8296cbb1a93ccbb47873c29add5967cf17372c8`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4` - unknown; unknown

```console
$ docker pull cassandra@sha256:60353c59bf2d27bac4c7e40068eb2be4fdcea6cf592f761202d7037b14a28d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ccf3e8bd1a704391344aae44680381ef16c2f9847e103fce64bed7cf472e04`

```dockerfile
```

-	Layers:
	-	`sha256:6b4e8c116b1c79c683c4d4329c5604e86a3cb22e3f0e14025cf3a1971d9176ff`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 3.6 MB (3593168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2d1eacf167d8b9538eb88ffa5b093294596e6c1ccfb93fc68cced66c574bdf7f`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 35.9 KB (35943 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:671ca9e4502d9c4610d70a75dd89aad2fb978d857dd9d8cbf15898c24e4e41f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151549151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fbb6df3072279264dfacef20ef26bc4157dd42e0134e0e7aacf99e893b7d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618ed61375ad4ec28a60723592784630c1740b36bc1e51769d4cab526a6d470a`  
		Last Modified: Wed, 08 Nov 2023 20:48:07 GMT  
		Size: 50.1 MB (50140404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba328d234a6c49ef77b6d558287d991b0c334b56092ce2165b9cb35a90bf2f88`  
		Last Modified: Wed, 08 Nov 2023 20:48:06 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4` - unknown; unknown

```console
$ docker pull cassandra@sha256:fd55b5fe315ab770069bd723ad63e038d68555c561a085a711b3ec4960c1dff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e95d1a907519ab9b3b4ef8de3b8403142b4cdf784cf40f98357826917a9fd1`

```dockerfile
```

-	Layers:
	-	`sha256:f5339eaaebcb07de07edaefb75b525956aba9c84655e49318b7e5465823f63de`  
		Last Modified: Wed, 08 Nov 2023 20:48:03 GMT  
		Size: 3.6 MB (3588824 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3ed069f5af5414019f7adb776abc070089c5c3a636c7e4e79a11e5f10a2228d`  
		Last Modified: Wed, 08 Nov 2023 20:48:02 GMT  
		Size: 35.8 KB (35843 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4` - linux; ppc64le

```console
$ docker pull cassandra@sha256:2e00f17e016a0ab7f15a51a8f05db126e4512cfe47e4e338414da5bb16b5c070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157156297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe2187cc8815dfec5c975bf5dfe77d1771eca06815db09d1c423af140e1e96d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f5989c4f51757083ecf4641b1b1c8b47378c8043684aedb5b3f3bcf53ec8738`  
		Last Modified: Sat, 02 Dec 2023 11:49:55 GMT  
		Size: 50.1 MB (50140526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:301a3e7b38e70f4f91567e3fa68d2e9a752231249b614a148cf8d21d61571925`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4` - unknown; unknown

```console
$ docker pull cassandra@sha256:69c3892fe7b764e2154499f4c016c7fce8ef2a3ffd30a54626c28dc939bee07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3631363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c45757d0ee664484346541a0967e3e426806d3c433cc12363d4f5bf1d3e0fae`

```dockerfile
```

-	Layers:
	-	`sha256:b730485c156a4a5ad12daae6484e74c2908b3989cefcacd5e36f704a9d1aaacf`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 3.6 MB (3595485 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:71a4973360d71e82a1baeae222df96977c574aa680252dccdab7ae20def3345e`  
		Last Modified: Sat, 02 Dec 2023 11:49:50 GMT  
		Size: 35.9 KB (35878 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4` - linux; s390x

```console
$ docker pull cassandra@sha256:9cae9e71a3c6db9658f6dd2b3c2163b78b0aa2dfa377b056b90f6be9fb50cc82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146408991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22d4507e9ea63b5e629d3e9a6120804528992a62485ef99c2154a3f3f1d58a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb2427e317a97aa7ccb7d36ba59346312147854f43bcd2b5478d38adc1b291ab`  
		Last Modified: Sat, 02 Dec 2023 10:09:43 GMT  
		Size: 50.1 MB (50140276 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6e2ea4958ce34dd014bacd369996f0bd3b08d1396f66ca38895fbb8306fa4a0`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4` - unknown; unknown

```console
$ docker pull cassandra@sha256:1577eaee8a20ab5cb3a2f92627bedad241c302ec72cd17a86b71ae57ef1f585a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52e0bae3fcd76dfd29cd9bbe33535478a42af46a7de318e5821a337d40060c0`

```dockerfile
```

-	Layers:
	-	`sha256:f502d9205a82eac738351ebd7f9768c88303d3a0e1c4f6acdefe4b24afc3300c`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 3.6 MB (3591665 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:08e9697cd0098392496fcb0ea480b3cad6e8de850a8abcb6a6050ab76ea0fd72`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:4.0`

```console
$ docker pull cassandra@sha256:cbf120c53f6139e9ce083f0b6e5caeeda512a37bc1a3ee5f681e1f21b75d87c0
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:4.0` - linux; amd64

```console
$ docker pull cassandra@sha256:ed8b06994e41f008a05b23483a8405f732531d4bb84fffe481b9682e1acf3661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154460792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f7a144100e271ec852070ceaf55ee01d5a4d95efeafccfa43e482f32688784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa209e79be14e7f0a79b6018ffeb98dfc7ace47267179474d49f3f047b1552e`  
		Last Modified: Mon, 30 Oct 2023 23:32:31 GMT  
		Size: 16.9 MB (16919533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3b10c5302cf62ee18806a97827d6dc331c281c16f7d3496abf368280a1c1e8`  
		Last Modified: Mon, 30 Oct 2023 23:34:20 GMT  
		Size: 47.1 MB (47068264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b138106695bf6d98648ae91cf8293d297c26af0f601864023eb1dfd88b8a47ae`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c6299c5a72111f9ebe3fb933f64b55022e8280a731493f48ce4bdf3896bf2c1`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b9a6018ddfda968517981de6842a128a9a462a2952574b2de4b6cca5b88a88a`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe38c47d4f14184cdcd87abee4036fa501a5229a2730909e174132b0d952daac`  
		Last Modified: Wed, 08 Nov 2023 20:23:32 GMT  
		Size: 11.0 MB (10951908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e3aadac6827049cb68baf66196b4c9fdb3ccd97de0e5b066600d7a9f3f203dc`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 1.1 MB (1098269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a1989f99711ae5c97a05c874eee815aeeb955463bbcf0d8e817252cde21e428`  
		Last Modified: Wed, 08 Nov 2023 20:23:34 GMT  
		Size: 49.8 MB (49838280 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c078b383496e21bce664fc832e48c15bec9a7f31095eac155f7b8d80ffe7d9db`  
		Last Modified: Wed, 08 Nov 2023 20:23:32 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:7b4bfb7d313b3169171203aea5aefb6e66d398b409e7a36bf084f6eda4c7cbdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3621938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c03d0e826d3c0f85eda3d8eddc2db653354cfeb043b7df0539c6d30f97b2d6a`

```dockerfile
```

-	Layers:
	-	`sha256:c1d60644219978b8c07325a17a56956b0da3f2280fe12a666f5921985c2d2879`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 3.6 MB (3586699 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:97812f17b356234474a780863de3f922363f818b18b8c478b8192b5b63fc1240`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 35.2 KB (35239 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8682ee77895ad2bba9bb23006de51fca224fdc0bc1d684f87166995ee2c28161
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146488319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4724253e7717df474399e0286873a8f9b2a02f0682c680f673cf8136b2891f2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c122b9284b34fb0949ab27793957e65a3d3793405e0b5b70a7fffdae2ab5a894`  
		Last Modified: Sat, 02 Dec 2023 08:55:16 GMT  
		Size: 49.8 MB (49838540 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b66885b1a67cfe59e61f9e6b85cae95dd9ca0a7dfb1b57af3655d4cae979f92`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:89f9252fd8b73fc27e72e2d015d5a5a91e8b714f443441c6f2249b54929939fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab263d948f4adbe8182c36f219ecf92eadb40e76c52445e8385195e63e87458`

```dockerfile
```

-	Layers:
	-	`sha256:c7f9d46596cd1ade5df2ea1f05ddf4523017a1f837d1a1df2ea698243824db4f`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 3.6 MB (3591497 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:24dc7328e2225e7ae06953895c4aba0445a94de11753a9fb7d47db2f0c000bf4`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 34.5 KB (34515 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:538d1eeb4441930316cf21e36e96f078c5c3e219f742dcc87eee13929a659d3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151247650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9322854ac277e2a60cbbac4e51b3200ccfa60a70a0b5ef47f2723c34156d1807`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9915bfd01b32ac7f2b9d5fe43effa57cc071cfcbe52d2ee05f05dba4fd91869c`  
		Last Modified: Wed, 08 Nov 2023 20:48:46 GMT  
		Size: 49.8 MB (49838903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d4f34fb4fcc8096e37b351cb9426d5ef555d3fa2541237702fb4a1a6226c481`  
		Last Modified: Wed, 08 Nov 2023 20:48:43 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:e41b936db72a4a5fbbcda200ab149269a2b5f10fe1b0e5b6a05793beda1f1b37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3621511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2259cdb5a91e73da0d22e8a0ce6efa4c825a0c882930be4a391d5a05f00c1fb`

```dockerfile
```

-	Layers:
	-	`sha256:3189665335e68fbacd41f0a1c576ac97eaca408234bd1dee26a4b4a9a6e4774d`  
		Last Modified: Wed, 08 Nov 2023 20:48:43 GMT  
		Size: 3.6 MB (3587083 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e7a660562004d9df8f7ff273f3c03294e06f43c18deafe3de5fef28f3bf83056`  
		Last Modified: Wed, 08 Nov 2023 20:48:42 GMT  
		Size: 34.4 KB (34428 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:c0a15b44eee70c770f274c2ffc843d6e00db7b9a49e6b3b21b46b24d92f25c5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156854797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a664e790f5d697639148fec60278d5b092b9b58261c2a8f8e7ec63fd30d1198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69543b579dd15e87d3669d5b367e6ce07ab4bab33649abcf9e6345112fd1ec94`  
		Last Modified: Sat, 02 Dec 2023 11:51:12 GMT  
		Size: 49.8 MB (49839024 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00dc74132d2861c36804c8fac32af72c01fa897713a069a76af360fa8eb26757`  
		Last Modified: Sat, 02 Dec 2023 11:51:11 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:782f5bc5724b1e663ea86a36a7e95d56d7779e64a729935f383105001d67d804
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3628272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870bbecab4a42d0d7079a17a6f17d073f868008f3a08e086740413998ba559fb`

```dockerfile
```

-	Layers:
	-	`sha256:77631e80ebce3c735749007a6704cc6a49131054f7de58977cc2a2cbfe1931be`  
		Last Modified: Sat, 02 Dec 2023 11:51:11 GMT  
		Size: 3.6 MB (3593818 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c70610668f0a11c851e8693d6af93f6a0daeadcb4517d6dae84feb8a683325b4`  
		Last Modified: Sat, 02 Dec 2023 11:51:10 GMT  
		Size: 34.5 KB (34454 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0` - linux; s390x

```console
$ docker pull cassandra@sha256:def4c346f31082e65ca0741e74dd5220746ff3d3f6fff87b69aead0215696a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146107321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7acb5210d8ab0b4279c86edc3d7fdcdb1e87ffbd91a9e881e672740f585c4d80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fb781ea85ac2d1347911f725863e8f611b81143a2cc34a94500e014e393875d`  
		Last Modified: Sat, 02 Dec 2023 10:15:30 GMT  
		Size: 49.8 MB (49838610 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bac97c70315be996cae1ecd1034d3fc08f16c4803c06498dfdb314ec0eace320`  
		Last Modified: Sat, 02 Dec 2023 10:15:29 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:673a5cea69e98fc0eaeed3f0e5da9fa50e4a98f5c420bf95465be0b6064ea3f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccde0719058583245106e9c376d3887e258c769303ca8b0141cc4de41d3a067d`

```dockerfile
```

-	Layers:
	-	`sha256:b1fde12f40e853e71758f7c2a817da0b91576173583504d203ead3a5311cf97a`  
		Last Modified: Sat, 02 Dec 2023 10:15:28 GMT  
		Size: 3.6 MB (3590010 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b3339456a55efc5337e1e122628de16f02e5a6808ff023d2294c1b2d6b5835c8`  
		Last Modified: Sat, 02 Dec 2023 10:15:28 GMT  
		Size: 34.4 KB (34422 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:4.0.11`

```console
$ docker pull cassandra@sha256:cbf120c53f6139e9ce083f0b6e5caeeda512a37bc1a3ee5f681e1f21b75d87c0
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:4.0.11` - linux; amd64

```console
$ docker pull cassandra@sha256:ed8b06994e41f008a05b23483a8405f732531d4bb84fffe481b9682e1acf3661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154460792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9f7a144100e271ec852070ceaf55ee01d5a4d95efeafccfa43e482f32688784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa209e79be14e7f0a79b6018ffeb98dfc7ace47267179474d49f3f047b1552e`  
		Last Modified: Mon, 30 Oct 2023 23:32:31 GMT  
		Size: 16.9 MB (16919533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3b10c5302cf62ee18806a97827d6dc331c281c16f7d3496abf368280a1c1e8`  
		Last Modified: Mon, 30 Oct 2023 23:34:20 GMT  
		Size: 47.1 MB (47068264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b138106695bf6d98648ae91cf8293d297c26af0f601864023eb1dfd88b8a47ae`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c6299c5a72111f9ebe3fb933f64b55022e8280a731493f48ce4bdf3896bf2c1`  
		Last Modified: Mon, 30 Oct 2023 23:34:13 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b9a6018ddfda968517981de6842a128a9a462a2952574b2de4b6cca5b88a88a`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe38c47d4f14184cdcd87abee4036fa501a5229a2730909e174132b0d952daac`  
		Last Modified: Wed, 08 Nov 2023 20:23:32 GMT  
		Size: 11.0 MB (10951908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e3aadac6827049cb68baf66196b4c9fdb3ccd97de0e5b066600d7a9f3f203dc`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 1.1 MB (1098269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a1989f99711ae5c97a05c874eee815aeeb955463bbcf0d8e817252cde21e428`  
		Last Modified: Wed, 08 Nov 2023 20:23:34 GMT  
		Size: 49.8 MB (49838280 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c078b383496e21bce664fc832e48c15bec9a7f31095eac155f7b8d80ffe7d9db`  
		Last Modified: Wed, 08 Nov 2023 20:23:32 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:7b4bfb7d313b3169171203aea5aefb6e66d398b409e7a36bf084f6eda4c7cbdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3621938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c03d0e826d3c0f85eda3d8eddc2db653354cfeb043b7df0539c6d30f97b2d6a`

```dockerfile
```

-	Layers:
	-	`sha256:c1d60644219978b8c07325a17a56956b0da3f2280fe12a666f5921985c2d2879`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 3.6 MB (3586699 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:97812f17b356234474a780863de3f922363f818b18b8c478b8192b5b63fc1240`  
		Last Modified: Wed, 08 Nov 2023 20:23:31 GMT  
		Size: 35.2 KB (35239 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0.11` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:8682ee77895ad2bba9bb23006de51fca224fdc0bc1d684f87166995ee2c28161
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146488319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4724253e7717df474399e0286873a8f9b2a02f0682c680f673cf8136b2891f2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c122b9284b34fb0949ab27793957e65a3d3793405e0b5b70a7fffdae2ab5a894`  
		Last Modified: Sat, 02 Dec 2023 08:55:16 GMT  
		Size: 49.8 MB (49838540 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b66885b1a67cfe59e61f9e6b85cae95dd9ca0a7dfb1b57af3655d4cae979f92`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:89f9252fd8b73fc27e72e2d015d5a5a91e8b714f443441c6f2249b54929939fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab263d948f4adbe8182c36f219ecf92eadb40e76c52445e8385195e63e87458`

```dockerfile
```

-	Layers:
	-	`sha256:c7f9d46596cd1ade5df2ea1f05ddf4523017a1f837d1a1df2ea698243824db4f`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 3.6 MB (3591497 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:24dc7328e2225e7ae06953895c4aba0445a94de11753a9fb7d47db2f0c000bf4`  
		Last Modified: Sat, 02 Dec 2023 08:55:14 GMT  
		Size: 34.5 KB (34515 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0.11` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:538d1eeb4441930316cf21e36e96f078c5c3e219f742dcc87eee13929a659d3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151247650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9322854ac277e2a60cbbac4e51b3200ccfa60a70a0b5ef47f2723c34156d1807`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9915bfd01b32ac7f2b9d5fe43effa57cc071cfcbe52d2ee05f05dba4fd91869c`  
		Last Modified: Wed, 08 Nov 2023 20:48:46 GMT  
		Size: 49.8 MB (49838903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d4f34fb4fcc8096e37b351cb9426d5ef555d3fa2541237702fb4a1a6226c481`  
		Last Modified: Wed, 08 Nov 2023 20:48:43 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:e41b936db72a4a5fbbcda200ab149269a2b5f10fe1b0e5b6a05793beda1f1b37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3621511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2259cdb5a91e73da0d22e8a0ce6efa4c825a0c882930be4a391d5a05f00c1fb`

```dockerfile
```

-	Layers:
	-	`sha256:3189665335e68fbacd41f0a1c576ac97eaca408234bd1dee26a4b4a9a6e4774d`  
		Last Modified: Wed, 08 Nov 2023 20:48:43 GMT  
		Size: 3.6 MB (3587083 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e7a660562004d9df8f7ff273f3c03294e06f43c18deafe3de5fef28f3bf83056`  
		Last Modified: Wed, 08 Nov 2023 20:48:42 GMT  
		Size: 34.4 KB (34428 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0.11` - linux; ppc64le

```console
$ docker pull cassandra@sha256:c0a15b44eee70c770f274c2ffc843d6e00db7b9a49e6b3b21b46b24d92f25c5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156854797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a664e790f5d697639148fec60278d5b092b9b58261c2a8f8e7ec63fd30d1198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69543b579dd15e87d3669d5b367e6ce07ab4bab33649abcf9e6345112fd1ec94`  
		Last Modified: Sat, 02 Dec 2023 11:51:12 GMT  
		Size: 49.8 MB (49839024 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00dc74132d2861c36804c8fac32af72c01fa897713a069a76af360fa8eb26757`  
		Last Modified: Sat, 02 Dec 2023 11:51:11 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:782f5bc5724b1e663ea86a36a7e95d56d7779e64a729935f383105001d67d804
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3628272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870bbecab4a42d0d7079a17a6f17d073f868008f3a08e086740413998ba559fb`

```dockerfile
```

-	Layers:
	-	`sha256:77631e80ebce3c735749007a6704cc6a49131054f7de58977cc2a2cbfe1931be`  
		Last Modified: Sat, 02 Dec 2023 11:51:11 GMT  
		Size: 3.6 MB (3593818 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c70610668f0a11c851e8693d6af93f6a0daeadcb4517d6dae84feb8a683325b4`  
		Last Modified: Sat, 02 Dec 2023 11:51:10 GMT  
		Size: 34.5 KB (34454 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.0.11` - linux; s390x

```console
$ docker pull cassandra@sha256:def4c346f31082e65ca0741e74dd5220746ff3d3f6fff87b69aead0215696a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146107321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7acb5210d8ab0b4279c86edc3d7fdcdb1e87ffbd91a9e881e672740f585c4d80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Wed, 04 Oct 2023 14:24:23 GMT
ARG RELEASE
# Wed, 04 Oct 2023 14:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 14:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 04 Oct 2023 14:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["/bin/bash"]
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Wed, 04 Oct 2023 14:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Wed, 04 Oct 2023 14:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GOSU_VERSION=1.16
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Wed, 04 Oct 2023 14:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 14:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_VERSION=4.0.11
# Wed, 04 Oct 2023 14:24:23 GMT
ENV CASSANDRA_SHA512=92bd35819e86927709add1075023af5aed93d42e0115bfa6b675b15e93b31bffa6fd3b9ff95a403bb9650ec417a0567ac776c88b56fe373938451746bbc64a50
# Wed, 04 Oct 2023 14:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
VOLUME [/var/lib/cassandra]
# Wed, 04 Oct 2023 14:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Wed, 04 Oct 2023 14:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fb781ea85ac2d1347911f725863e8f611b81143a2cc34a94500e014e393875d`  
		Last Modified: Sat, 02 Dec 2023 10:15:30 GMT  
		Size: 49.8 MB (49838610 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bac97c70315be996cae1ecd1034d3fc08f16c4803c06498dfdb314ec0eace320`  
		Last Modified: Sat, 02 Dec 2023 10:15:29 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.0.11` - unknown; unknown

```console
$ docker pull cassandra@sha256:673a5cea69e98fc0eaeed3f0e5da9fa50e4a98f5c420bf95465be0b6064ea3f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccde0719058583245106e9c376d3887e258c769303ca8b0141cc4de41d3a067d`

```dockerfile
```

-	Layers:
	-	`sha256:b1fde12f40e853e71758f7c2a817da0b91576173583504d203ead3a5311cf97a`  
		Last Modified: Sat, 02 Dec 2023 10:15:28 GMT  
		Size: 3.6 MB (3590010 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b3339456a55efc5337e1e122628de16f02e5a6808ff023d2294c1b2d6b5835c8`  
		Last Modified: Sat, 02 Dec 2023 10:15:28 GMT  
		Size: 34.4 KB (34422 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:4.1`

```console
$ docker pull cassandra@sha256:e7f2a92533f24b3656aa1179df92cf95b7d16e45fa87f93fb7809cac757fd98a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:4.1` - linux; amd64

```console
$ docker pull cassandra@sha256:599be9b5e23f91edbc43598f7df994b53993d82ae65c2cc1aba9f0e5fa2af8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154749016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597c6621fd1dfe8ca2dafb7c39c3b6c113626cdfe8f7740708b6939b7936e2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6c48cef298b986e7cfd235b365ca20053fde3138d661e80c29fb4e0daa1fa88`  
		Last Modified: Sat, 02 Dec 2023 02:05:26 GMT  
		Size: 47.1 MB (47068582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b90bdd07aa688f6123bcef53bbaaf699cd0104995994b90787214abe494d2df`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa13e718ec7250f1c09858061de443dfd506a5c40a422d0586e57366a5dfada4`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed2030023c7b0aedadaa1f81c9305e6e17e83438572ec0884fb8b468f53b97db`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a9483292d0e0e03f0e6a4e628bc0b9dffb74b04fbf62e823ca3802e9cde789`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 10.9 MB (10934074 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:273a18c34b61cfe3e13656ced1129dcd8b59aa4013bd5c92a0cd0b44bd3b7a81`  
		Last Modified: Sat, 02 Dec 2023 03:12:37 GMT  
		Size: 1.1 MB (1098343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdd8f9e8894a325ee0a006affc7c485435db3076d4688cf1db04cf7b44e0fa9`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 50.1 MB (50139981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39c8fc1b3f62bcbcf45b2747bd2c71ace02f0e12b38bdb7d0707d957ebadfe3e`  
		Last Modified: Sat, 02 Dec 2023 03:12:38 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1` - unknown; unknown

```console
$ docker pull cassandra@sha256:996e0b0ef4446c0b10211489243681082f32635d8284f35f95c08e8cfe6ae040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc707d98d06138a1b15c81acec547ab76f41d9675f0e725062c1a67e0429ba3`

```dockerfile
```

-	Layers:
	-	`sha256:75341ea69fa2e930371db5f52ba7d03b30eab1a350ede59146677b62f622e2b7`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 3.6 MB (3590619 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6a00958cf9b8b16a6b18db001d4f649b0d940bce4cc639966bde0df1a492b3dc`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:bd55cb2c5542fba3670f0bb97a1d891d1c5580e9c572b63571f6768f5bebeec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146789764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d571f6a6cc6de91e550b452c934b01334beffffe5e54416391402e3d981121d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba8e2d5a27a6f19d95e0d48c8b46050091977649696cd2bffea1dd999165fa5`  
		Last Modified: Sat, 02 Dec 2023 08:54:23 GMT  
		Size: 50.1 MB (50139985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77ce296b72ba77e2e0a97284a8296cbb1a93ccbb47873c29add5967cf17372c8`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1` - unknown; unknown

```console
$ docker pull cassandra@sha256:60353c59bf2d27bac4c7e40068eb2be4fdcea6cf592f761202d7037b14a28d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ccf3e8bd1a704391344aae44680381ef16c2f9847e103fce64bed7cf472e04`

```dockerfile
```

-	Layers:
	-	`sha256:6b4e8c116b1c79c683c4d4329c5604e86a3cb22e3f0e14025cf3a1971d9176ff`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 3.6 MB (3593168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2d1eacf167d8b9538eb88ffa5b093294596e6c1ccfb93fc68cced66c574bdf7f`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 35.9 KB (35943 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:671ca9e4502d9c4610d70a75dd89aad2fb978d857dd9d8cbf15898c24e4e41f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151549151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fbb6df3072279264dfacef20ef26bc4157dd42e0134e0e7aacf99e893b7d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618ed61375ad4ec28a60723592784630c1740b36bc1e51769d4cab526a6d470a`  
		Last Modified: Wed, 08 Nov 2023 20:48:07 GMT  
		Size: 50.1 MB (50140404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba328d234a6c49ef77b6d558287d991b0c334b56092ce2165b9cb35a90bf2f88`  
		Last Modified: Wed, 08 Nov 2023 20:48:06 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1` - unknown; unknown

```console
$ docker pull cassandra@sha256:fd55b5fe315ab770069bd723ad63e038d68555c561a085a711b3ec4960c1dff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e95d1a907519ab9b3b4ef8de3b8403142b4cdf784cf40f98357826917a9fd1`

```dockerfile
```

-	Layers:
	-	`sha256:f5339eaaebcb07de07edaefb75b525956aba9c84655e49318b7e5465823f63de`  
		Last Modified: Wed, 08 Nov 2023 20:48:03 GMT  
		Size: 3.6 MB (3588824 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3ed069f5af5414019f7adb776abc070089c5c3a636c7e4e79a11e5f10a2228d`  
		Last Modified: Wed, 08 Nov 2023 20:48:02 GMT  
		Size: 35.8 KB (35843 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1` - linux; ppc64le

```console
$ docker pull cassandra@sha256:2e00f17e016a0ab7f15a51a8f05db126e4512cfe47e4e338414da5bb16b5c070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157156297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe2187cc8815dfec5c975bf5dfe77d1771eca06815db09d1c423af140e1e96d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f5989c4f51757083ecf4641b1b1c8b47378c8043684aedb5b3f3bcf53ec8738`  
		Last Modified: Sat, 02 Dec 2023 11:49:55 GMT  
		Size: 50.1 MB (50140526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:301a3e7b38e70f4f91567e3fa68d2e9a752231249b614a148cf8d21d61571925`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1` - unknown; unknown

```console
$ docker pull cassandra@sha256:69c3892fe7b764e2154499f4c016c7fce8ef2a3ffd30a54626c28dc939bee07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3631363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c45757d0ee664484346541a0967e3e426806d3c433cc12363d4f5bf1d3e0fae`

```dockerfile
```

-	Layers:
	-	`sha256:b730485c156a4a5ad12daae6484e74c2908b3989cefcacd5e36f704a9d1aaacf`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 3.6 MB (3595485 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:71a4973360d71e82a1baeae222df96977c574aa680252dccdab7ae20def3345e`  
		Last Modified: Sat, 02 Dec 2023 11:49:50 GMT  
		Size: 35.9 KB (35878 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1` - linux; s390x

```console
$ docker pull cassandra@sha256:9cae9e71a3c6db9658f6dd2b3c2163b78b0aa2dfa377b056b90f6be9fb50cc82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146408991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22d4507e9ea63b5e629d3e9a6120804528992a62485ef99c2154a3f3f1d58a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb2427e317a97aa7ccb7d36ba59346312147854f43bcd2b5478d38adc1b291ab`  
		Last Modified: Sat, 02 Dec 2023 10:09:43 GMT  
		Size: 50.1 MB (50140276 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6e2ea4958ce34dd014bacd369996f0bd3b08d1396f66ca38895fbb8306fa4a0`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1` - unknown; unknown

```console
$ docker pull cassandra@sha256:1577eaee8a20ab5cb3a2f92627bedad241c302ec72cd17a86b71ae57ef1f585a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52e0bae3fcd76dfd29cd9bbe33535478a42af46a7de318e5821a337d40060c0`

```dockerfile
```

-	Layers:
	-	`sha256:f502d9205a82eac738351ebd7f9768c88303d3a0e1c4f6acdefe4b24afc3300c`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 3.6 MB (3591665 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:08e9697cd0098392496fcb0ea480b3cad6e8de850a8abcb6a6050ab76ea0fd72`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:4.1.3`

```console
$ docker pull cassandra@sha256:e7f2a92533f24b3656aa1179df92cf95b7d16e45fa87f93fb7809cac757fd98a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:4.1.3` - linux; amd64

```console
$ docker pull cassandra@sha256:599be9b5e23f91edbc43598f7df994b53993d82ae65c2cc1aba9f0e5fa2af8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154749016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597c6621fd1dfe8ca2dafb7c39c3b6c113626cdfe8f7740708b6939b7936e2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6c48cef298b986e7cfd235b365ca20053fde3138d661e80c29fb4e0daa1fa88`  
		Last Modified: Sat, 02 Dec 2023 02:05:26 GMT  
		Size: 47.1 MB (47068582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b90bdd07aa688f6123bcef53bbaaf699cd0104995994b90787214abe494d2df`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa13e718ec7250f1c09858061de443dfd506a5c40a422d0586e57366a5dfada4`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed2030023c7b0aedadaa1f81c9305e6e17e83438572ec0884fb8b468f53b97db`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a9483292d0e0e03f0e6a4e628bc0b9dffb74b04fbf62e823ca3802e9cde789`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 10.9 MB (10934074 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:273a18c34b61cfe3e13656ced1129dcd8b59aa4013bd5c92a0cd0b44bd3b7a81`  
		Last Modified: Sat, 02 Dec 2023 03:12:37 GMT  
		Size: 1.1 MB (1098343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdd8f9e8894a325ee0a006affc7c485435db3076d4688cf1db04cf7b44e0fa9`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 50.1 MB (50139981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39c8fc1b3f62bcbcf45b2747bd2c71ace02f0e12b38bdb7d0707d957ebadfe3e`  
		Last Modified: Sat, 02 Dec 2023 03:12:38 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1.3` - unknown; unknown

```console
$ docker pull cassandra@sha256:996e0b0ef4446c0b10211489243681082f32635d8284f35f95c08e8cfe6ae040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc707d98d06138a1b15c81acec547ab76f41d9675f0e725062c1a67e0429ba3`

```dockerfile
```

-	Layers:
	-	`sha256:75341ea69fa2e930371db5f52ba7d03b30eab1a350ede59146677b62f622e2b7`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 3.6 MB (3590619 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6a00958cf9b8b16a6b18db001d4f649b0d940bce4cc639966bde0df1a492b3dc`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1.3` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:bd55cb2c5542fba3670f0bb97a1d891d1c5580e9c572b63571f6768f5bebeec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146789764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d571f6a6cc6de91e550b452c934b01334beffffe5e54416391402e3d981121d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba8e2d5a27a6f19d95e0d48c8b46050091977649696cd2bffea1dd999165fa5`  
		Last Modified: Sat, 02 Dec 2023 08:54:23 GMT  
		Size: 50.1 MB (50139985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77ce296b72ba77e2e0a97284a8296cbb1a93ccbb47873c29add5967cf17372c8`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1.3` - unknown; unknown

```console
$ docker pull cassandra@sha256:60353c59bf2d27bac4c7e40068eb2be4fdcea6cf592f761202d7037b14a28d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ccf3e8bd1a704391344aae44680381ef16c2f9847e103fce64bed7cf472e04`

```dockerfile
```

-	Layers:
	-	`sha256:6b4e8c116b1c79c683c4d4329c5604e86a3cb22e3f0e14025cf3a1971d9176ff`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 3.6 MB (3593168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2d1eacf167d8b9538eb88ffa5b093294596e6c1ccfb93fc68cced66c574bdf7f`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 35.9 KB (35943 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1.3` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:671ca9e4502d9c4610d70a75dd89aad2fb978d857dd9d8cbf15898c24e4e41f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151549151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fbb6df3072279264dfacef20ef26bc4157dd42e0134e0e7aacf99e893b7d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618ed61375ad4ec28a60723592784630c1740b36bc1e51769d4cab526a6d470a`  
		Last Modified: Wed, 08 Nov 2023 20:48:07 GMT  
		Size: 50.1 MB (50140404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba328d234a6c49ef77b6d558287d991b0c334b56092ce2165b9cb35a90bf2f88`  
		Last Modified: Wed, 08 Nov 2023 20:48:06 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1.3` - unknown; unknown

```console
$ docker pull cassandra@sha256:fd55b5fe315ab770069bd723ad63e038d68555c561a085a711b3ec4960c1dff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e95d1a907519ab9b3b4ef8de3b8403142b4cdf784cf40f98357826917a9fd1`

```dockerfile
```

-	Layers:
	-	`sha256:f5339eaaebcb07de07edaefb75b525956aba9c84655e49318b7e5465823f63de`  
		Last Modified: Wed, 08 Nov 2023 20:48:03 GMT  
		Size: 3.6 MB (3588824 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3ed069f5af5414019f7adb776abc070089c5c3a636c7e4e79a11e5f10a2228d`  
		Last Modified: Wed, 08 Nov 2023 20:48:02 GMT  
		Size: 35.8 KB (35843 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1.3` - linux; ppc64le

```console
$ docker pull cassandra@sha256:2e00f17e016a0ab7f15a51a8f05db126e4512cfe47e4e338414da5bb16b5c070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157156297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe2187cc8815dfec5c975bf5dfe77d1771eca06815db09d1c423af140e1e96d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f5989c4f51757083ecf4641b1b1c8b47378c8043684aedb5b3f3bcf53ec8738`  
		Last Modified: Sat, 02 Dec 2023 11:49:55 GMT  
		Size: 50.1 MB (50140526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:301a3e7b38e70f4f91567e3fa68d2e9a752231249b614a148cf8d21d61571925`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1.3` - unknown; unknown

```console
$ docker pull cassandra@sha256:69c3892fe7b764e2154499f4c016c7fce8ef2a3ffd30a54626c28dc939bee07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3631363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c45757d0ee664484346541a0967e3e426806d3c433cc12363d4f5bf1d3e0fae`

```dockerfile
```

-	Layers:
	-	`sha256:b730485c156a4a5ad12daae6484e74c2908b3989cefcacd5e36f704a9d1aaacf`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 3.6 MB (3595485 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:71a4973360d71e82a1baeae222df96977c574aa680252dccdab7ae20def3345e`  
		Last Modified: Sat, 02 Dec 2023 11:49:50 GMT  
		Size: 35.9 KB (35878 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:4.1.3` - linux; s390x

```console
$ docker pull cassandra@sha256:9cae9e71a3c6db9658f6dd2b3c2163b78b0aa2dfa377b056b90f6be9fb50cc82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146408991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22d4507e9ea63b5e629d3e9a6120804528992a62485ef99c2154a3f3f1d58a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb2427e317a97aa7ccb7d36ba59346312147854f43bcd2b5478d38adc1b291ab`  
		Last Modified: Sat, 02 Dec 2023 10:09:43 GMT  
		Size: 50.1 MB (50140276 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6e2ea4958ce34dd014bacd369996f0bd3b08d1396f66ca38895fbb8306fa4a0`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:4.1.3` - unknown; unknown

```console
$ docker pull cassandra@sha256:1577eaee8a20ab5cb3a2f92627bedad241c302ec72cd17a86b71ae57ef1f585a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52e0bae3fcd76dfd29cd9bbe33535478a42af46a7de318e5821a337d40060c0`

```dockerfile
```

-	Layers:
	-	`sha256:f502d9205a82eac738351ebd7f9768c88303d3a0e1c4f6acdefe4b24afc3300c`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 3.6 MB (3591665 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:08e9697cd0098392496fcb0ea480b3cad6e8de850a8abcb6a6050ab76ea0fd72`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:5`

```console
$ docker pull cassandra@sha256:3b9071e44754b6f7276e99a252799440586913fca1625ec706cc936571fd15b4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:5` - linux; amd64

```console
$ docker pull cassandra@sha256:ac5ecf526b3475c590f8e33dc192656a049e30888731b09f750cf7cd0195a609
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187726150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d24656f40b8922064c997a170b4bf4174f1620151e3bfdfff600e59b4d9e5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7931cb9f5edfcbe51fbcea9444db96cc98834a9d67447fda8bc5f8d35a41f6a`  
		Last Modified: Sat, 02 Dec 2023 02:05:56 GMT  
		Size: 20.7 MB (20662837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62db5efe399e58542dcf09ff993396b7fd714ce816b7cdcd552a84dfbb38b021`  
		Last Modified: Sat, 02 Dec 2023 02:06:44 GMT  
		Size: 47.1 MB (47148574 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ce6776554d94f55f454dde27303436ad0a68854efe5ea6811d6953b5b5ce5b`  
		Last Modified: Sat, 02 Dec 2023 02:06:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f3ee07bc40f0ec22ed21d3d526ebcb39a96e255ea2dafef11f89c909c98cb93`  
		Last Modified: Sat, 02 Dec 2023 02:06:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38d873200a410c9469baef1c6797f9b82146c6f8a39f4f2a527da7a83a7a003b`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ea6b59754fa2ee2cc3c8ea6c2c448831c37190814a0c90a5cec7d57cf6d9ba2`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 10.9 MB (10937020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1ab81fdb4a87ffa23f2ce23b3706e6270dcfd951e4d67d0e5284ba63ae57723`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.1 MB (1101149 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7944b733a4e2ce256967712eb92d148a62ac27af1d1b740e4150cb2216404a5`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 79.3 MB (79288692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9720c85e2628844a4db71e6e64b6c1d518b3528ece156617f6cf0a2bb35ad74`  
		Last Modified: Sat, 02 Dec 2023 03:12:25 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5` - unknown; unknown

```console
$ docker pull cassandra@sha256:51ac7f6eb37ff22f0c8a6f2132dc31aa6e51122f513a859c4b690231f4e8093e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3797674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd2b8b9ef7ca2b96a7faff2673ac608420ee12f7da01c76e1d366f4686eaee5`

```dockerfile
```

-	Layers:
	-	`sha256:756581929d87f6d040ee47ec1ea03f809e2cdc40e6bd886fd04f654f370fd375`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 3.8 MB (3762129 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8cf1a20f9d5a617fc9bb569c91e4169b97ce36aafbeb11053e7aefef4dd36bef`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:1040b047ea85327df3dedeb75a95ad9653852386ef0e8885450203333830b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.8 MB (179824890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b358c649a015fd1d11c651d510b62d8d922b6700032a0fa10fc7ef2e978b5e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9dec2f9566e72953501111c558a0e1f3141c3ab814b5ccbb5e2f2d304807386`  
		Last Modified: Sat, 02 Dec 2023 06:58:46 GMT  
		Size: 20.0 MB (19960106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:957d89aa618323d03334cba6d268a920e1c1c77674845851f2570ed6f775ab77`  
		Last Modified: Sat, 02 Dec 2023 06:59:37 GMT  
		Size: 44.8 MB (44788140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b9435146eb5d90a51b826db3a3199f4ea10c5fd7d21a9ac5da59fb400c272ed`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e57f8b5bfab2221f93a7e500e995618cfb33d78f71c25ebb9a94ba2d406c7f0`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5a4b251b03f62b3fb414ab1857a3ef0a6a5ffa5b826b5233e4606aae693a652`  
		Last Modified: Sat, 02 Dec 2023 08:49:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4267d8f5dcb6059dcdbb018c0885f28143d2f68c75e4f08707b29fd17f670474`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 10.1 MB (10115479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad9f8fb3a6db05fd488f3fc7fe7b279e7b0293dc55630ca9b0dfb95acf070662`  
		Last Modified: Sat, 02 Dec 2023 08:49:44 GMT  
		Size: 1.1 MB (1068395 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1246d19b9a2314e904fb5122c435b70a7f791d976bfc8dd324cbb41c03ee6da`  
		Last Modified: Sat, 02 Dec 2023 08:49:47 GMT  
		Size: 79.3 MB (79288754 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1cc82ab3371e1d68bbf2c71945d9db762ae39a1fc4907f088d16b2a99e52da1`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5` - unknown; unknown

```console
$ docker pull cassandra@sha256:ac440a6c529d4a2d02353cf9ba3288483a4d6ab39d6f87cc6216d500a86888f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3729866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221dfc40ae30fa3f80c198e94868240dc491a664fc79afa11596ee7c9f975d35`

```dockerfile
```

-	Layers:
	-	`sha256:64acb2ab6713fda00d9d454e0598e7d30459a03ee8892ce39181b1f07b13df0b`  
		Last Modified: Sat, 02 Dec 2023 08:49:42 GMT  
		Size: 3.7 MB (3694220 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:12f62a29fc8ce83c769dbe23bbd53f0545fe325b5a37d770e2314df0d6f426e3`  
		Last Modified: Sat, 02 Dec 2023 08:49:41 GMT  
		Size: 35.6 KB (35646 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffb3c1a0c40f2b30d964b0af03f13d4ed90b377309ade6a6792bd31467e0ce99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.5 MB (186537014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d75282370c30ee9dc11bb070befb243911af807cabc09a41bd7ee87096963a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:43:32 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:43:33 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:45:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:45:29 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:45:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:45:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3982c3bf03cb594352f69f3f546c659470c3051ff39a2f19d27f0ef95db66ca`  
		Last Modified: Mon, 30 Oct 2023 23:50:22 GMT  
		Size: 21.4 MB (21378540 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63e5d1582b3c2417d8b0b8335d34f748a17ee5fa019774754c1753245b62142b`  
		Last Modified: Mon, 30 Oct 2023 23:51:49 GMT  
		Size: 46.6 MB (46624289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07764e92b7187cc5adcea1819b77c42e6382b656201e4a17ab1b60f60b766297`  
		Last Modified: Mon, 30 Oct 2023 23:51:43 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1811b512327bd2ba0d318bc88d8eee511781da72b2e98b9cac89b3a16d0a1d17`  
		Last Modified: Mon, 30 Oct 2023 23:51:44 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:738c16eb915bdfb18fb3a789aa65a101ed1ac1692023f758c5c3f5be95b64423`  
		Last Modified: Wed, 08 Nov 2023 20:45:47 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db3a22e8b797e890b07eb4dfba71185b864fd48bd3ef26538ab5721a1e880d95`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 11.0 MB (11009383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:197923e30b0d1a23abd6e4138f2d9e2cc67af3e3e7d9ffad625ee4e17d6266c0`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.0 MB (1032491 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91c591a1b188a4858d6997dba5429041c65f6c069a6a3b31f8538af5c1528e70`  
		Last Modified: Wed, 08 Nov 2023 20:45:53 GMT  
		Size: 79.3 MB (79288952 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c64aade99aaf70b3dcca67100956dcdb7320217caa443546ec73f51c745daea9`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5` - unknown; unknown

```console
$ docker pull cassandra@sha256:14f4976476c11c5add8c9775db40bb0ba9120e49b7ef2d55ce5bd55bef6c72e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dd13b4c164c57bac470e7599af99bc1e8f1ae975d7973638246ccff68a8a83`

```dockerfile
```

-	Layers:
	-	`sha256:fb49813987d1a9c1bc952df5c2754c87bd17f48562763db68b877b83c3194ed8`  
		Last Modified: Wed, 08 Nov 2023 20:45:46 GMT  
		Size: 3.8 MB (3842410 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:43884c2bed213940c5c4399f26895cac3b5d3f17672e53b286e2c4eda13749f0`  
		Last Modified: Wed, 08 Nov 2023 20:45:45 GMT  
		Size: 35.6 KB (35553 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5` - linux; ppc64le

```console
$ docker pull cassandra@sha256:4289c7149bd77abdb67ed9664ceaaa7c1f662a6e8650298a4b51113ce807605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195305228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ab8dd91b980c80b52711dec6392027c0866b8c638080e006af74aef836bfd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c67a1d056689cea4c275027f768cfaa99dccfe862731aaf5c2927d88c90e541`  
		Last Modified: Sat, 02 Dec 2023 06:17:30 GMT  
		Size: 22.7 MB (22708785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32751e3544c7d70b4d159a9c51b858744b687cf327c015342d67f0c690fbfaa4`  
		Last Modified: Sat, 02 Dec 2023 06:18:23 GMT  
		Size: 47.0 MB (47000599 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10a83bbc3d77a6238250c9e07b0c88ec4f4dd381a34d0a3ad773fc700334b24b`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea5a80b2014144e0c5a34f5fc3f8aae9f0ced49124321bb9032103ca41cd4282`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 732.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:384c81e909ec0dd9615bcff7914486ce06c28fc69e92810cee0d9a6eb42b9e53`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:849eba6d020636a8ac19e26adcc8074d07824fe1b58cf2f842df0d3118b46517`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 12.0 MB (11966912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76040a3ed2c349a544306115a6f66f609e834859680aa2e69674ee10dcff3996`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.0 MB (1022109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e5e74a786a3edb229674125f9e2feb68791026cd2ea313b1f94164039876526`  
		Last Modified: Sat, 02 Dec 2023 11:47:59 GMT  
		Size: 79.3 MB (79289217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:528d0bfc49fe8a864d16fdac51fc3fa8e41f0484839ff6798d05033cf3dcdad4`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5` - unknown; unknown

```console
$ docker pull cassandra@sha256:6e98efa2cbd1fc79e0d153b3bcf5d847b5f708b209a3041033a4ad901ef27823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3824794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f91fd0631b49d3fea3966273aa23036ec7370a5fbe02d540a386c5795c84b38d`

```dockerfile
```

-	Layers:
	-	`sha256:71bd2af78f0dda88d22ae353ee7d77884b0e8b900384c3416a156d48081354ed`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 3.8 MB (3789211 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d39d3ed61254aa9c944d5ad2551ee49053a5684d29ad19830b370a409ab23523`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 35.6 KB (35583 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5` - linux; s390x

```console
$ docker pull cassandra@sha256:a67262e8a50f13b12f1de233b1d3248680afaddac808d1fc12c7ef9e5b86bde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182053696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a111e94adf15a057e16e014a2c8db0a1f4a874f9120bff2bba12a4b95615f8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d88ff680076c1c6114f126164c4743ce5e08f4929719b8c4a5c652670cc4771a`  
		Last Modified: Sat, 02 Dec 2023 05:53:23 GMT  
		Size: 20.1 MB (20142166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:336f063bfed8f8018886c8598fb2f448c787bd63ca0ab3485f80172364869126`  
		Last Modified: Sat, 02 Dec 2023 05:54:05 GMT  
		Size: 43.8 MB (43755116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:495b143a0de20904246dfc293831e266aadae3af965caffb137824c9527d1062`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c111579f8b53efd10f7ff570e7ffedb269264007645a1710579e68d344b696f`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5554e35aef014513102b03cfdfbc14875779adb8ea991fbc39db87419ef052e`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b494e33cb861841d772aa4183361138f60696a7a4692ad419f77ea037466fa36`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 10.8 MB (10781249 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e39012fbadf34356060adf030cff85a7d440051eb6b82c25d29378347a7f4fa2`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.1 MB (1066971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fa9211cc103959f0eae3ba586fc5f65e4610066415e68b10c602f4b6313e1ce`  
		Last Modified: Sat, 02 Dec 2023 10:03:09 GMT  
		Size: 79.3 MB (79288744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0dbb062c5eb78ec5f460e88ce88858d1d7d02dcda3c8f270c3310ce8028eae40`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5` - unknown; unknown

```console
$ docker pull cassandra@sha256:33fef038d8437b545b6b3954b7c7f113313c5d09eab151e3d9a19040094f9502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3735976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6a7cc79d401046cf8d39ac0738979f2565c7ee1e0d63e8042cbee9e3504301`

```dockerfile
```

-	Layers:
	-	`sha256:c70f89c8b4a948e84dd319230a35d5cf8fcbf69db139bcbec48434c3024ce143`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 3.7 MB (3700431 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1b5197445995e826e104f5c92f31574f9fcb91787750deb589ee0516acdfb279`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:5.0`

```console
$ docker pull cassandra@sha256:3b9071e44754b6f7276e99a252799440586913fca1625ec706cc936571fd15b4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:5.0` - linux; amd64

```console
$ docker pull cassandra@sha256:ac5ecf526b3475c590f8e33dc192656a049e30888731b09f750cf7cd0195a609
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187726150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d24656f40b8922064c997a170b4bf4174f1620151e3bfdfff600e59b4d9e5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7931cb9f5edfcbe51fbcea9444db96cc98834a9d67447fda8bc5f8d35a41f6a`  
		Last Modified: Sat, 02 Dec 2023 02:05:56 GMT  
		Size: 20.7 MB (20662837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62db5efe399e58542dcf09ff993396b7fd714ce816b7cdcd552a84dfbb38b021`  
		Last Modified: Sat, 02 Dec 2023 02:06:44 GMT  
		Size: 47.1 MB (47148574 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ce6776554d94f55f454dde27303436ad0a68854efe5ea6811d6953b5b5ce5b`  
		Last Modified: Sat, 02 Dec 2023 02:06:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f3ee07bc40f0ec22ed21d3d526ebcb39a96e255ea2dafef11f89c909c98cb93`  
		Last Modified: Sat, 02 Dec 2023 02:06:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38d873200a410c9469baef1c6797f9b82146c6f8a39f4f2a527da7a83a7a003b`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ea6b59754fa2ee2cc3c8ea6c2c448831c37190814a0c90a5cec7d57cf6d9ba2`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 10.9 MB (10937020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1ab81fdb4a87ffa23f2ce23b3706e6270dcfd951e4d67d0e5284ba63ae57723`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.1 MB (1101149 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7944b733a4e2ce256967712eb92d148a62ac27af1d1b740e4150cb2216404a5`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 79.3 MB (79288692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9720c85e2628844a4db71e6e64b6c1d518b3528ece156617f6cf0a2bb35ad74`  
		Last Modified: Sat, 02 Dec 2023 03:12:25 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:51ac7f6eb37ff22f0c8a6f2132dc31aa6e51122f513a859c4b690231f4e8093e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3797674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd2b8b9ef7ca2b96a7faff2673ac608420ee12f7da01c76e1d366f4686eaee5`

```dockerfile
```

-	Layers:
	-	`sha256:756581929d87f6d040ee47ec1ea03f809e2cdc40e6bd886fd04f654f370fd375`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 3.8 MB (3762129 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8cf1a20f9d5a617fc9bb569c91e4169b97ce36aafbeb11053e7aefef4dd36bef`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:1040b047ea85327df3dedeb75a95ad9653852386ef0e8885450203333830b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.8 MB (179824890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b358c649a015fd1d11c651d510b62d8d922b6700032a0fa10fc7ef2e978b5e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9dec2f9566e72953501111c558a0e1f3141c3ab814b5ccbb5e2f2d304807386`  
		Last Modified: Sat, 02 Dec 2023 06:58:46 GMT  
		Size: 20.0 MB (19960106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:957d89aa618323d03334cba6d268a920e1c1c77674845851f2570ed6f775ab77`  
		Last Modified: Sat, 02 Dec 2023 06:59:37 GMT  
		Size: 44.8 MB (44788140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b9435146eb5d90a51b826db3a3199f4ea10c5fd7d21a9ac5da59fb400c272ed`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e57f8b5bfab2221f93a7e500e995618cfb33d78f71c25ebb9a94ba2d406c7f0`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5a4b251b03f62b3fb414ab1857a3ef0a6a5ffa5b826b5233e4606aae693a652`  
		Last Modified: Sat, 02 Dec 2023 08:49:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4267d8f5dcb6059dcdbb018c0885f28143d2f68c75e4f08707b29fd17f670474`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 10.1 MB (10115479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad9f8fb3a6db05fd488f3fc7fe7b279e7b0293dc55630ca9b0dfb95acf070662`  
		Last Modified: Sat, 02 Dec 2023 08:49:44 GMT  
		Size: 1.1 MB (1068395 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1246d19b9a2314e904fb5122c435b70a7f791d976bfc8dd324cbb41c03ee6da`  
		Last Modified: Sat, 02 Dec 2023 08:49:47 GMT  
		Size: 79.3 MB (79288754 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1cc82ab3371e1d68bbf2c71945d9db762ae39a1fc4907f088d16b2a99e52da1`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:ac440a6c529d4a2d02353cf9ba3288483a4d6ab39d6f87cc6216d500a86888f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3729866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221dfc40ae30fa3f80c198e94868240dc491a664fc79afa11596ee7c9f975d35`

```dockerfile
```

-	Layers:
	-	`sha256:64acb2ab6713fda00d9d454e0598e7d30459a03ee8892ce39181b1f07b13df0b`  
		Last Modified: Sat, 02 Dec 2023 08:49:42 GMT  
		Size: 3.7 MB (3694220 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:12f62a29fc8ce83c769dbe23bbd53f0545fe325b5a37d770e2314df0d6f426e3`  
		Last Modified: Sat, 02 Dec 2023 08:49:41 GMT  
		Size: 35.6 KB (35646 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffb3c1a0c40f2b30d964b0af03f13d4ed90b377309ade6a6792bd31467e0ce99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.5 MB (186537014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d75282370c30ee9dc11bb070befb243911af807cabc09a41bd7ee87096963a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:43:32 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:43:33 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:45:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:45:29 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:45:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:45:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3982c3bf03cb594352f69f3f546c659470c3051ff39a2f19d27f0ef95db66ca`  
		Last Modified: Mon, 30 Oct 2023 23:50:22 GMT  
		Size: 21.4 MB (21378540 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63e5d1582b3c2417d8b0b8335d34f748a17ee5fa019774754c1753245b62142b`  
		Last Modified: Mon, 30 Oct 2023 23:51:49 GMT  
		Size: 46.6 MB (46624289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07764e92b7187cc5adcea1819b77c42e6382b656201e4a17ab1b60f60b766297`  
		Last Modified: Mon, 30 Oct 2023 23:51:43 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1811b512327bd2ba0d318bc88d8eee511781da72b2e98b9cac89b3a16d0a1d17`  
		Last Modified: Mon, 30 Oct 2023 23:51:44 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:738c16eb915bdfb18fb3a789aa65a101ed1ac1692023f758c5c3f5be95b64423`  
		Last Modified: Wed, 08 Nov 2023 20:45:47 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db3a22e8b797e890b07eb4dfba71185b864fd48bd3ef26538ab5721a1e880d95`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 11.0 MB (11009383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:197923e30b0d1a23abd6e4138f2d9e2cc67af3e3e7d9ffad625ee4e17d6266c0`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.0 MB (1032491 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91c591a1b188a4858d6997dba5429041c65f6c069a6a3b31f8538af5c1528e70`  
		Last Modified: Wed, 08 Nov 2023 20:45:53 GMT  
		Size: 79.3 MB (79288952 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c64aade99aaf70b3dcca67100956dcdb7320217caa443546ec73f51c745daea9`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:14f4976476c11c5add8c9775db40bb0ba9120e49b7ef2d55ce5bd55bef6c72e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dd13b4c164c57bac470e7599af99bc1e8f1ae975d7973638246ccff68a8a83`

```dockerfile
```

-	Layers:
	-	`sha256:fb49813987d1a9c1bc952df5c2754c87bd17f48562763db68b877b83c3194ed8`  
		Last Modified: Wed, 08 Nov 2023 20:45:46 GMT  
		Size: 3.8 MB (3842410 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:43884c2bed213940c5c4399f26895cac3b5d3f17672e53b286e2c4eda13749f0`  
		Last Modified: Wed, 08 Nov 2023 20:45:45 GMT  
		Size: 35.6 KB (35553 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0` - linux; ppc64le

```console
$ docker pull cassandra@sha256:4289c7149bd77abdb67ed9664ceaaa7c1f662a6e8650298a4b51113ce807605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195305228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ab8dd91b980c80b52711dec6392027c0866b8c638080e006af74aef836bfd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c67a1d056689cea4c275027f768cfaa99dccfe862731aaf5c2927d88c90e541`  
		Last Modified: Sat, 02 Dec 2023 06:17:30 GMT  
		Size: 22.7 MB (22708785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32751e3544c7d70b4d159a9c51b858744b687cf327c015342d67f0c690fbfaa4`  
		Last Modified: Sat, 02 Dec 2023 06:18:23 GMT  
		Size: 47.0 MB (47000599 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10a83bbc3d77a6238250c9e07b0c88ec4f4dd381a34d0a3ad773fc700334b24b`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea5a80b2014144e0c5a34f5fc3f8aae9f0ced49124321bb9032103ca41cd4282`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 732.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:384c81e909ec0dd9615bcff7914486ce06c28fc69e92810cee0d9a6eb42b9e53`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:849eba6d020636a8ac19e26adcc8074d07824fe1b58cf2f842df0d3118b46517`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 12.0 MB (11966912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76040a3ed2c349a544306115a6f66f609e834859680aa2e69674ee10dcff3996`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.0 MB (1022109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e5e74a786a3edb229674125f9e2feb68791026cd2ea313b1f94164039876526`  
		Last Modified: Sat, 02 Dec 2023 11:47:59 GMT  
		Size: 79.3 MB (79289217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:528d0bfc49fe8a864d16fdac51fc3fa8e41f0484839ff6798d05033cf3dcdad4`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:6e98efa2cbd1fc79e0d153b3bcf5d847b5f708b209a3041033a4ad901ef27823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3824794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f91fd0631b49d3fea3966273aa23036ec7370a5fbe02d540a386c5795c84b38d`

```dockerfile
```

-	Layers:
	-	`sha256:71bd2af78f0dda88d22ae353ee7d77884b0e8b900384c3416a156d48081354ed`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 3.8 MB (3789211 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d39d3ed61254aa9c944d5ad2551ee49053a5684d29ad19830b370a409ab23523`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 35.6 KB (35583 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0` - linux; s390x

```console
$ docker pull cassandra@sha256:a67262e8a50f13b12f1de233b1d3248680afaddac808d1fc12c7ef9e5b86bde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182053696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a111e94adf15a057e16e014a2c8db0a1f4a874f9120bff2bba12a4b95615f8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d88ff680076c1c6114f126164c4743ce5e08f4929719b8c4a5c652670cc4771a`  
		Last Modified: Sat, 02 Dec 2023 05:53:23 GMT  
		Size: 20.1 MB (20142166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:336f063bfed8f8018886c8598fb2f448c787bd63ca0ab3485f80172364869126`  
		Last Modified: Sat, 02 Dec 2023 05:54:05 GMT  
		Size: 43.8 MB (43755116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:495b143a0de20904246dfc293831e266aadae3af965caffb137824c9527d1062`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c111579f8b53efd10f7ff570e7ffedb269264007645a1710579e68d344b696f`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5554e35aef014513102b03cfdfbc14875779adb8ea991fbc39db87419ef052e`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b494e33cb861841d772aa4183361138f60696a7a4692ad419f77ea037466fa36`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 10.8 MB (10781249 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e39012fbadf34356060adf030cff85a7d440051eb6b82c25d29378347a7f4fa2`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.1 MB (1066971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fa9211cc103959f0eae3ba586fc5f65e4610066415e68b10c602f4b6313e1ce`  
		Last Modified: Sat, 02 Dec 2023 10:03:09 GMT  
		Size: 79.3 MB (79288744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0dbb062c5eb78ec5f460e88ce88858d1d7d02dcda3c8f270c3310ce8028eae40`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0` - unknown; unknown

```console
$ docker pull cassandra@sha256:33fef038d8437b545b6b3954b7c7f113313c5d09eab151e3d9a19040094f9502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3735976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6a7cc79d401046cf8d39ac0738979f2565c7ee1e0d63e8042cbee9e3504301`

```dockerfile
```

-	Layers:
	-	`sha256:c70f89c8b4a948e84dd319230a35d5cf8fcbf69db139bcbec48434c3024ce143`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 3.7 MB (3700431 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1b5197445995e826e104f5c92f31574f9fcb91787750deb589ee0516acdfb279`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:5.0-alpha2`

```console
$ docker pull cassandra@sha256:3b9071e44754b6f7276e99a252799440586913fca1625ec706cc936571fd15b4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:5.0-alpha2` - linux; amd64

```console
$ docker pull cassandra@sha256:ac5ecf526b3475c590f8e33dc192656a049e30888731b09f750cf7cd0195a609
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187726150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d24656f40b8922064c997a170b4bf4174f1620151e3bfdfff600e59b4d9e5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7931cb9f5edfcbe51fbcea9444db96cc98834a9d67447fda8bc5f8d35a41f6a`  
		Last Modified: Sat, 02 Dec 2023 02:05:56 GMT  
		Size: 20.7 MB (20662837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62db5efe399e58542dcf09ff993396b7fd714ce816b7cdcd552a84dfbb38b021`  
		Last Modified: Sat, 02 Dec 2023 02:06:44 GMT  
		Size: 47.1 MB (47148574 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ce6776554d94f55f454dde27303436ad0a68854efe5ea6811d6953b5b5ce5b`  
		Last Modified: Sat, 02 Dec 2023 02:06:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f3ee07bc40f0ec22ed21d3d526ebcb39a96e255ea2dafef11f89c909c98cb93`  
		Last Modified: Sat, 02 Dec 2023 02:06:38 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38d873200a410c9469baef1c6797f9b82146c6f8a39f4f2a527da7a83a7a003b`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ea6b59754fa2ee2cc3c8ea6c2c448831c37190814a0c90a5cec7d57cf6d9ba2`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 10.9 MB (10937020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1ab81fdb4a87ffa23f2ce23b3706e6270dcfd951e4d67d0e5284ba63ae57723`  
		Last Modified: Sat, 02 Dec 2023 03:12:24 GMT  
		Size: 1.1 MB (1101149 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7944b733a4e2ce256967712eb92d148a62ac27af1d1b740e4150cb2216404a5`  
		Last Modified: Sat, 02 Dec 2023 03:12:26 GMT  
		Size: 79.3 MB (79288692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9720c85e2628844a4db71e6e64b6c1d518b3528ece156617f6cf0a2bb35ad74`  
		Last Modified: Sat, 02 Dec 2023 03:12:25 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0-alpha2` - unknown; unknown

```console
$ docker pull cassandra@sha256:51ac7f6eb37ff22f0c8a6f2132dc31aa6e51122f513a859c4b690231f4e8093e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3797674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd2b8b9ef7ca2b96a7faff2673ac608420ee12f7da01c76e1d366f4686eaee5`

```dockerfile
```

-	Layers:
	-	`sha256:756581929d87f6d040ee47ec1ea03f809e2cdc40e6bd886fd04f654f370fd375`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 3.8 MB (3762129 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8cf1a20f9d5a617fc9bb569c91e4169b97ce36aafbeb11053e7aefef4dd36bef`  
		Last Modified: Sat, 02 Dec 2023 03:12:23 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0-alpha2` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:1040b047ea85327df3dedeb75a95ad9653852386ef0e8885450203333830b8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.8 MB (179824890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b358c649a015fd1d11c651d510b62d8d922b6700032a0fa10fc7ef2e978b5e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9dec2f9566e72953501111c558a0e1f3141c3ab814b5ccbb5e2f2d304807386`  
		Last Modified: Sat, 02 Dec 2023 06:58:46 GMT  
		Size: 20.0 MB (19960106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:957d89aa618323d03334cba6d268a920e1c1c77674845851f2570ed6f775ab77`  
		Last Modified: Sat, 02 Dec 2023 06:59:37 GMT  
		Size: 44.8 MB (44788140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b9435146eb5d90a51b826db3a3199f4ea10c5fd7d21a9ac5da59fb400c272ed`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e57f8b5bfab2221f93a7e500e995618cfb33d78f71c25ebb9a94ba2d406c7f0`  
		Last Modified: Sat, 02 Dec 2023 06:59:30 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5a4b251b03f62b3fb414ab1857a3ef0a6a5ffa5b826b5233e4606aae693a652`  
		Last Modified: Sat, 02 Dec 2023 08:49:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4267d8f5dcb6059dcdbb018c0885f28143d2f68c75e4f08707b29fd17f670474`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 10.1 MB (10115479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad9f8fb3a6db05fd488f3fc7fe7b279e7b0293dc55630ca9b0dfb95acf070662`  
		Last Modified: Sat, 02 Dec 2023 08:49:44 GMT  
		Size: 1.1 MB (1068395 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1246d19b9a2314e904fb5122c435b70a7f791d976bfc8dd324cbb41c03ee6da`  
		Last Modified: Sat, 02 Dec 2023 08:49:47 GMT  
		Size: 79.3 MB (79288754 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1cc82ab3371e1d68bbf2c71945d9db762ae39a1fc4907f088d16b2a99e52da1`  
		Last Modified: Sat, 02 Dec 2023 08:49:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0-alpha2` - unknown; unknown

```console
$ docker pull cassandra@sha256:ac440a6c529d4a2d02353cf9ba3288483a4d6ab39d6f87cc6216d500a86888f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3729866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221dfc40ae30fa3f80c198e94868240dc491a664fc79afa11596ee7c9f975d35`

```dockerfile
```

-	Layers:
	-	`sha256:64acb2ab6713fda00d9d454e0598e7d30459a03ee8892ce39181b1f07b13df0b`  
		Last Modified: Sat, 02 Dec 2023 08:49:42 GMT  
		Size: 3.7 MB (3694220 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:12f62a29fc8ce83c769dbe23bbd53f0545fe325b5a37d770e2314df0d6f426e3`  
		Last Modified: Sat, 02 Dec 2023 08:49:41 GMT  
		Size: 35.6 KB (35646 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0-alpha2` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ffb3c1a0c40f2b30d964b0af03f13d4ed90b377309ade6a6792bd31467e0ce99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.5 MB (186537014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d75282370c30ee9dc11bb070befb243911af807cabc09a41bd7ee87096963a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:43:32 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:43:33 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:45:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:45:29 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:45:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:45:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3982c3bf03cb594352f69f3f546c659470c3051ff39a2f19d27f0ef95db66ca`  
		Last Modified: Mon, 30 Oct 2023 23:50:22 GMT  
		Size: 21.4 MB (21378540 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63e5d1582b3c2417d8b0b8335d34f748a17ee5fa019774754c1753245b62142b`  
		Last Modified: Mon, 30 Oct 2023 23:51:49 GMT  
		Size: 46.6 MB (46624289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07764e92b7187cc5adcea1819b77c42e6382b656201e4a17ab1b60f60b766297`  
		Last Modified: Mon, 30 Oct 2023 23:51:43 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1811b512327bd2ba0d318bc88d8eee511781da72b2e98b9cac89b3a16d0a1d17`  
		Last Modified: Mon, 30 Oct 2023 23:51:44 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:738c16eb915bdfb18fb3a789aa65a101ed1ac1692023f758c5c3f5be95b64423`  
		Last Modified: Wed, 08 Nov 2023 20:45:47 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db3a22e8b797e890b07eb4dfba71185b864fd48bd3ef26538ab5721a1e880d95`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 11.0 MB (11009383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:197923e30b0d1a23abd6e4138f2d9e2cc67af3e3e7d9ffad625ee4e17d6266c0`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.0 MB (1032491 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91c591a1b188a4858d6997dba5429041c65f6c069a6a3b31f8538af5c1528e70`  
		Last Modified: Wed, 08 Nov 2023 20:45:53 GMT  
		Size: 79.3 MB (79288952 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c64aade99aaf70b3dcca67100956dcdb7320217caa443546ec73f51c745daea9`  
		Last Modified: Wed, 08 Nov 2023 20:45:48 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0-alpha2` - unknown; unknown

```console
$ docker pull cassandra@sha256:14f4976476c11c5add8c9775db40bb0ba9120e49b7ef2d55ce5bd55bef6c72e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69dd13b4c164c57bac470e7599af99bc1e8f1ae975d7973638246ccff68a8a83`

```dockerfile
```

-	Layers:
	-	`sha256:fb49813987d1a9c1bc952df5c2754c87bd17f48562763db68b877b83c3194ed8`  
		Last Modified: Wed, 08 Nov 2023 20:45:46 GMT  
		Size: 3.8 MB (3842410 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:43884c2bed213940c5c4399f26895cac3b5d3f17672e53b286e2c4eda13749f0`  
		Last Modified: Wed, 08 Nov 2023 20:45:45 GMT  
		Size: 35.6 KB (35553 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0-alpha2` - linux; ppc64le

```console
$ docker pull cassandra@sha256:4289c7149bd77abdb67ed9664ceaaa7c1f662a6e8650298a4b51113ce807605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195305228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ab8dd91b980c80b52711dec6392027c0866b8c638080e006af74aef836bfd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c67a1d056689cea4c275027f768cfaa99dccfe862731aaf5c2927d88c90e541`  
		Last Modified: Sat, 02 Dec 2023 06:17:30 GMT  
		Size: 22.7 MB (22708785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32751e3544c7d70b4d159a9c51b858744b687cf327c015342d67f0c690fbfaa4`  
		Last Modified: Sat, 02 Dec 2023 06:18:23 GMT  
		Size: 47.0 MB (47000599 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10a83bbc3d77a6238250c9e07b0c88ec4f4dd381a34d0a3ad773fc700334b24b`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea5a80b2014144e0c5a34f5fc3f8aae9f0ced49124321bb9032103ca41cd4282`  
		Last Modified: Sat, 02 Dec 2023 06:18:15 GMT  
		Size: 732.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:384c81e909ec0dd9615bcff7914486ce06c28fc69e92810cee0d9a6eb42b9e53`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:849eba6d020636a8ac19e26adcc8074d07824fe1b58cf2f842df0d3118b46517`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 12.0 MB (11966912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76040a3ed2c349a544306115a6f66f609e834859680aa2e69674ee10dcff3996`  
		Last Modified: Sat, 02 Dec 2023 11:47:55 GMT  
		Size: 1.0 MB (1022109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e5e74a786a3edb229674125f9e2feb68791026cd2ea313b1f94164039876526`  
		Last Modified: Sat, 02 Dec 2023 11:47:59 GMT  
		Size: 79.3 MB (79289217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:528d0bfc49fe8a864d16fdac51fc3fa8e41f0484839ff6798d05033cf3dcdad4`  
		Last Modified: Sat, 02 Dec 2023 11:47:56 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0-alpha2` - unknown; unknown

```console
$ docker pull cassandra@sha256:6e98efa2cbd1fc79e0d153b3bcf5d847b5f708b209a3041033a4ad901ef27823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3824794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f91fd0631b49d3fea3966273aa23036ec7370a5fbe02d540a386c5795c84b38d`

```dockerfile
```

-	Layers:
	-	`sha256:71bd2af78f0dda88d22ae353ee7d77884b0e8b900384c3416a156d48081354ed`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 3.8 MB (3789211 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d39d3ed61254aa9c944d5ad2551ee49053a5684d29ad19830b370a409ab23523`  
		Last Modified: Sat, 02 Dec 2023 11:47:53 GMT  
		Size: 35.6 KB (35583 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:5.0-alpha2` - linux; s390x

```console
$ docker pull cassandra@sha256:a67262e8a50f13b12f1de233b1d3248680afaddac808d1fc12c7ef9e5b86bde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.1 MB (182053696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a111e94adf15a057e16e014a2c8db0a1f4a874f9120bff2bba12a4b95615f8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 04 Nov 2023 14:24:28 GMT
ARG RELEASE
# Sat, 04 Nov 2023 14:24:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 04 Nov 2023 14:24:28 GMT
LABEL org.opencontainers.image.version=20.04
# Sat, 04 Nov 2023 14:24:28 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["/bin/bash"]
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2023 14:24:28 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 04 Nov 2023 14:24:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Sat, 04 Nov 2023 14:24:28 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 14:24:28 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_VERSION=5.0-alpha2
# Sat, 04 Nov 2023 14:24:28 GMT
ENV CASSANDRA_SHA512=f4476871b3d55a49c0e492dbf5d8f2f46cd0e82f1614cc0697daddd64c74c66883df3c45ce00bd028ea86ed88c3a30e1f36bcdcd929d225e38bd1c848c9d5841
# Sat, 04 Nov 2023 14:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
VOLUME [/var/lib/cassandra]
# Sat, 04 Nov 2023 14:24:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 04 Nov 2023 14:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2023 14:24:28 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Sat, 04 Nov 2023 14:24:28 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d88ff680076c1c6114f126164c4743ce5e08f4929719b8c4a5c652670cc4771a`  
		Last Modified: Sat, 02 Dec 2023 05:53:23 GMT  
		Size: 20.1 MB (20142166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:336f063bfed8f8018886c8598fb2f448c787bd63ca0ab3485f80172364869126`  
		Last Modified: Sat, 02 Dec 2023 05:54:05 GMT  
		Size: 43.8 MB (43755116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:495b143a0de20904246dfc293831e266aadae3af965caffb137824c9527d1062`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c111579f8b53efd10f7ff570e7ffedb269264007645a1710579e68d344b696f`  
		Last Modified: Sat, 02 Dec 2023 05:53:59 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5554e35aef014513102b03cfdfbc14875779adb8ea991fbc39db87419ef052e`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b494e33cb861841d772aa4183361138f60696a7a4692ad419f77ea037466fa36`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 10.8 MB (10781249 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e39012fbadf34356060adf030cff85a7d440051eb6b82c25d29378347a7f4fa2`  
		Last Modified: Sat, 02 Dec 2023 10:03:06 GMT  
		Size: 1.1 MB (1066971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fa9211cc103959f0eae3ba586fc5f65e4610066415e68b10c602f4b6313e1ce`  
		Last Modified: Sat, 02 Dec 2023 10:03:09 GMT  
		Size: 79.3 MB (79288744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0dbb062c5eb78ec5f460e88ce88858d1d7d02dcda3c8f270c3310ce8028eae40`  
		Last Modified: Sat, 02 Dec 2023 10:03:07 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:5.0-alpha2` - unknown; unknown

```console
$ docker pull cassandra@sha256:33fef038d8437b545b6b3954b7c7f113313c5d09eab151e3d9a19040094f9502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3735976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6a7cc79d401046cf8d39ac0738979f2565c7ee1e0d63e8042cbee9e3504301`

```dockerfile
```

-	Layers:
	-	`sha256:c70f89c8b4a948e84dd319230a35d5cf8fcbf69db139bcbec48434c3024ce143`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 3.7 MB (3700431 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1b5197445995e826e104f5c92f31574f9fcb91787750deb589ee0516acdfb279`  
		Last Modified: Sat, 02 Dec 2023 10:03:04 GMT  
		Size: 35.5 KB (35545 bytes)  
		MIME: application/vnd.in-toto+json

## `cassandra:latest`

```console
$ docker pull cassandra@sha256:e7f2a92533f24b3656aa1179df92cf95b7d16e45fa87f93fb7809cac757fd98a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `cassandra:latest` - linux; amd64

```console
$ docker pull cassandra@sha256:599be9b5e23f91edbc43598f7df994b53993d82ae65c2cc1aba9f0e5fa2af8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154749016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597c6621fd1dfe8ca2dafb7c39c3b6c113626cdfe8f7740708b6939b7936e2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6c48cef298b986e7cfd235b365ca20053fde3138d661e80c29fb4e0daa1fa88`  
		Last Modified: Sat, 02 Dec 2023 02:05:26 GMT  
		Size: 47.1 MB (47068582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b90bdd07aa688f6123bcef53bbaaf699cd0104995994b90787214abe494d2df`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa13e718ec7250f1c09858061de443dfd506a5c40a422d0586e57366a5dfada4`  
		Last Modified: Sat, 02 Dec 2023 02:05:19 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed2030023c7b0aedadaa1f81c9305e6e17e83438572ec0884fb8b468f53b97db`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a9483292d0e0e03f0e6a4e628bc0b9dffb74b04fbf62e823ca3802e9cde789`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 10.9 MB (10934074 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:273a18c34b61cfe3e13656ced1129dcd8b59aa4013bd5c92a0cd0b44bd3b7a81`  
		Last Modified: Sat, 02 Dec 2023 03:12:37 GMT  
		Size: 1.1 MB (1098343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdd8f9e8894a325ee0a006affc7c485435db3076d4688cf1db04cf7b44e0fa9`  
		Last Modified: Sat, 02 Dec 2023 03:12:39 GMT  
		Size: 50.1 MB (50139981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39c8fc1b3f62bcbcf45b2747bd2c71ace02f0e12b38bdb7d0707d957ebadfe3e`  
		Last Modified: Sat, 02 Dec 2023 03:12:38 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:latest` - unknown; unknown

```console
$ docker pull cassandra@sha256:996e0b0ef4446c0b10211489243681082f32635d8284f35f95c08e8cfe6ae040
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3626453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc707d98d06138a1b15c81acec547ab76f41d9675f0e725062c1a67e0429ba3`

```dockerfile
```

-	Layers:
	-	`sha256:75341ea69fa2e930371db5f52ba7d03b30eab1a350ede59146677b62f622e2b7`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 3.6 MB (3590619 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6a00958cf9b8b16a6b18db001d4f649b0d940bce4cc639966bde0df1a492b3dc`  
		Last Modified: Sat, 02 Dec 2023 03:12:36 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:latest` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:bd55cb2c5542fba3670f0bb97a1d891d1c5580e9c572b63571f6768f5bebeec2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146789764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d571f6a6cc6de91e550b452c934b01334beffffe5e54416391402e3d981121d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:043af50602b163e71a05aa02ec03cbbb2659582ffeea29004c4477939cf448e0 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:e2f879bfa159449422063ff666ac028f07b2d0d0240c9d1beecd2171ce0eac6b`  
		Last Modified: Wed, 29 Nov 2023 17:47:28 GMT  
		Size: 24.6 MB (24600167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aae850917417df586c6eb2de1d4b788845c7fb565cfcaa212040f1d4c0e5d3b8`  
		Last Modified: Sat, 02 Dec 2023 06:56:24 GMT  
		Size: 15.7 MB (15659161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48dd75cc5333e4ae1ddd6ad1e69f29adcc6f3344f338983d2da4ef7f680b0b76`  
		Last Modified: Sat, 02 Dec 2023 06:58:18 GMT  
		Size: 45.2 MB (45207724 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cece42f56f5813ee741a17dfeb27e1c1970d08deb8f5bf7e679b97c6315bd56a`  
		Last Modified: Sat, 02 Dec 2023 06:58:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8e8e3ed22b3076fd945a4192d60a8f479cc58a2a5dac0fc0664eacb21989b6`  
		Last Modified: Sat, 02 Dec 2023 06:58:11 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7a1765b3f1b90917a6fe4ec54e59f66a299341047977851f12b6ec53e14b4fd`  
		Last Modified: Sat, 02 Dec 2023 08:54:20 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:069b9a194f575fb33eda8040ccb23822ca2be16193496112f8ebf0a6e840b850`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 10.1 MB (10113304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c188268b618ec8ff0f36a2ec72e7ace6be4584edd0844e6421c04e913e9623eb`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.1 MB (1065573 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba8e2d5a27a6f19d95e0d48c8b46050091977649696cd2bffea1dd999165fa5`  
		Last Modified: Sat, 02 Dec 2023 08:54:23 GMT  
		Size: 50.1 MB (50139985 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77ce296b72ba77e2e0a97284a8296cbb1a93ccbb47873c29add5967cf17372c8`  
		Last Modified: Sat, 02 Dec 2023 08:54:21 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:latest` - unknown; unknown

```console
$ docker pull cassandra@sha256:60353c59bf2d27bac4c7e40068eb2be4fdcea6cf592f761202d7037b14a28d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ccf3e8bd1a704391344aae44680381ef16c2f9847e103fce64bed7cf472e04`

```dockerfile
```

-	Layers:
	-	`sha256:6b4e8c116b1c79c683c4d4329c5604e86a3cb22e3f0e14025cf3a1971d9176ff`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 3.6 MB (3593168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2d1eacf167d8b9538eb88ffa5b093294596e6c1ccfb93fc68cced66c574bdf7f`  
		Last Modified: Sat, 02 Dec 2023 08:54:19 GMT  
		Size: 35.9 KB (35943 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:latest` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:671ca9e4502d9c4610d70a75dd89aad2fb978d857dd9d8cbf15898c24e4e41f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.5 MB (151549151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fbb6df3072279264dfacef20ef26bc4157dd42e0134e0e7aacf99e893b7d1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2717b88e02799c1309e24243b581cd227d05944a061c0c57d1cac69369a47533`  
		Last Modified: Mon, 30 Oct 2023 23:48:05 GMT  
		Size: 16.8 MB (16768205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69babd9c42e52e7f0b9436e4498ae4a1944f9a01b2640bf62ef9c1426e06292e`  
		Last Modified: Mon, 30 Oct 2023 23:49:28 GMT  
		Size: 45.4 MB (45399668 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8bc3a7959b7c939bebd95303b996e61b56d36ff6b75f034596a1cfa87b60f1a`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f96bb6916357fe00bd6e6ed154ab0c1af5a17e96a042a287dcb1b00e5d9cc6`  
		Last Modified: Mon, 30 Oct 2023 23:49:23 GMT  
		Size: 733.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12c026a35dfca99234045c9c663d75b36cecb18027d714da6c219c86cd344513`  
		Last Modified: Wed, 08 Nov 2023 20:48:04 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd924de2254237def1588b9896af2c17e79369428ca889cd4ca15977b0e2d57`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 11.0 MB (11007033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa0083f331d2788855276f63018836dfdebe1b84f2cea8827b834ab491cf0b`  
		Last Modified: Wed, 08 Nov 2023 20:48:05 GMT  
		Size: 1.0 MB (1030480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618ed61375ad4ec28a60723592784630c1740b36bc1e51769d4cab526a6d470a`  
		Last Modified: Wed, 08 Nov 2023 20:48:07 GMT  
		Size: 50.1 MB (50140404 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba328d234a6c49ef77b6d558287d991b0c334b56092ce2165b9cb35a90bf2f88`  
		Last Modified: Wed, 08 Nov 2023 20:48:06 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:latest` - unknown; unknown

```console
$ docker pull cassandra@sha256:fd55b5fe315ab770069bd723ad63e038d68555c561a085a711b3ec4960c1dff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3624667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e95d1a907519ab9b3b4ef8de3b8403142b4cdf784cf40f98357826917a9fd1`

```dockerfile
```

-	Layers:
	-	`sha256:f5339eaaebcb07de07edaefb75b525956aba9c84655e49318b7e5465823f63de`  
		Last Modified: Wed, 08 Nov 2023 20:48:03 GMT  
		Size: 3.6 MB (3588824 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3ed069f5af5414019f7adb776abc070089c5c3a636c7e4e79a11e5f10a2228d`  
		Last Modified: Wed, 08 Nov 2023 20:48:02 GMT  
		Size: 35.8 KB (35843 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:latest` - linux; ppc64le

```console
$ docker pull cassandra@sha256:2e00f17e016a0ab7f15a51a8f05db126e4512cfe47e4e338414da5bb16b5c070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157156297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe2187cc8815dfec5c975bf5dfe77d1771eca06815db09d1c423af140e1e96d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0feca61d6e49f8b3080150f749da49efb095ec8816598c9bb326674e092dce0`  
		Last Modified: Sat, 02 Dec 2023 06:14:58 GMT  
		Size: 18.2 MB (18215146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc91c532ebd217ca8cae029e3d8a69856130a937bb7022d403195f519e88c28c`  
		Last Modified: Sat, 02 Dec 2023 06:17:00 GMT  
		Size: 42.5 MB (42499126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eead568ca3143ef43404733804d072a904855bfbab9b6e4a444e2d1f372596b3`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f593faf96839a34b4d4ad828b70a1fbf4ac2978dcabeb09e047675057e7b31b0`  
		Last Modified: Sat, 02 Dec 2023 06:16:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9333508291e6c825f7e0af76474581c3a414ef959b5fbeccaad42041e5581f8d`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c63cb81c1988fcfb30c08780e03bbfd4aa6dbaf88ab51934e30556385c0839b7`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 12.0 MB (11964380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b9ba1a08cf4afadf247efeb9d72beeac60cad47b3161a699ef2ebf0641d60e0`  
		Last Modified: Sat, 02 Dec 2023 11:49:52 GMT  
		Size: 1.0 MB (1019508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f5989c4f51757083ecf4641b1b1c8b47378c8043684aedb5b3f3bcf53ec8738`  
		Last Modified: Sat, 02 Dec 2023 11:49:55 GMT  
		Size: 50.1 MB (50140526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:301a3e7b38e70f4f91567e3fa68d2e9a752231249b614a148cf8d21d61571925`  
		Last Modified: Sat, 02 Dec 2023 11:49:53 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:latest` - unknown; unknown

```console
$ docker pull cassandra@sha256:69c3892fe7b764e2154499f4c016c7fce8ef2a3ffd30a54626c28dc939bee07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3631363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c45757d0ee664484346541a0967e3e426806d3c433cc12363d4f5bf1d3e0fae`

```dockerfile
```

-	Layers:
	-	`sha256:b730485c156a4a5ad12daae6484e74c2908b3989cefcacd5e36f704a9d1aaacf`  
		Last Modified: Sat, 02 Dec 2023 11:49:51 GMT  
		Size: 3.6 MB (3595485 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:71a4973360d71e82a1baeae222df96977c574aa680252dccdab7ae20def3345e`  
		Last Modified: Sat, 02 Dec 2023 11:49:50 GMT  
		Size: 35.9 KB (35878 bytes)  
		MIME: application/vnd.in-toto+json

### `cassandra:latest` - linux; s390x

```console
$ docker pull cassandra@sha256:9cae9e71a3c6db9658f6dd2b3c2163b78b0aa2dfa377b056b90f6be9fb50cc82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146408991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22d4507e9ea63b5e629d3e9a6120804528992a62485ef99c2154a3f3f1d58a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Mon, 24 Jul 2023 20:24:23 GMT
ARG RELEASE
# Mon, 24 Jul 2023 20:24:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 24 Jul 2023 20:24:23 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 24 Jul 2023 20:24:23 GMT
ADD file:d9d0513ebd111f79b38e6a84389a13bff0ea39811a455d2bf83565e10a32040e in / 
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["/bin/bash"]
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 24 Jul 2023 20:24:23 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 24 Jul 2023 20:24:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GOSU_VERSION=1.16
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 24 Jul 2023 20:24:23 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jul 2023 20:24:23 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55 	7464AAD9068241C50BA6A26232F35CB2F546D93E 	CEC5C50B9C629EF0F5AB2706650B72EB14CCD622
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_VERSION=4.1.3
# Mon, 24 Jul 2023 20:24:23 GMT
ENV CASSANDRA_SHA512=393443a5b9849645362df2f7536e734e1fc6d513aadf440fab8dda3063553394a138805098796d35f9d4d31e2899ecab630a2ec2a44d00d5e63bed549a2e844c
# Mon, 24 Jul 2023 20:24:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm-server.options"; 			sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm-server.options"; 			grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm-server.options"; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 1777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
VOLUME [/var/lib/cassandra]
# Mon, 24 Jul 2023 20:24:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 20:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 20:24:23 GMT
EXPOSE map[7000/tcp:{} 7001/tcp:{} 7199/tcp:{} 9042/tcp:{} 9160/tcp:{}]
# Mon, 24 Jul 2023 20:24:23 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:5c76130ae9eb84bd09498a783136b5699a48ba6368f627d730a08ba67d8af7f4`  
		Last Modified: Sat, 02 Dec 2023 05:42:27 GMT  
		Size: 27.0 MB (27015595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7758a0038c4d904175abd45d2bfe270c47167ad44c918d7c58c9d7abdf71070`  
		Last Modified: Sat, 02 Dec 2023 05:52:18 GMT  
		Size: 16.6 MB (16643111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f54d998f34297048b54611183475f25ca1e3735973611a71b83a33f2b671200`  
		Last Modified: Sat, 02 Dec 2023 05:52:57 GMT  
		Size: 40.8 MB (40762220 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23523bafb58d3b505a1a504d5620803e1016354abb942c03a57698019a82c57`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88b05caae6d9f1cda4f774b8ac3e3de63044775bcedf0b4237e77140a220a74b`  
		Last Modified: Sat, 02 Dec 2023 05:52:52 GMT  
		Size: 734.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a4d92a2e215f2acecb134884fa8c658633506893792d22045a7000bad5dfcfa`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a91c69f7e470c9f06cecd8540c0463501416e3dfbaadf3f5527b5de8fdd852f`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 10.8 MB (10779058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0383e6348449f41133a794559318b6ef4aac938badd783fc5aa253748e47a818`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.1 MB (1064878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb2427e317a97aa7ccb7d36ba59346312147854f43bcd2b5478d38adc1b291ab`  
		Last Modified: Sat, 02 Dec 2023 10:09:43 GMT  
		Size: 50.1 MB (50140276 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6e2ea4958ce34dd014bacd369996f0bd3b08d1396f66ca38895fbb8306fa4a0`  
		Last Modified: Sat, 02 Dec 2023 10:09:41 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `cassandra:latest` - unknown; unknown

```console
$ docker pull cassandra@sha256:1577eaee8a20ab5cb3a2f92627bedad241c302ec72cd17a86b71ae57ef1f585a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52e0bae3fcd76dfd29cd9bbe33535478a42af46a7de318e5821a337d40060c0`

```dockerfile
```

-	Layers:
	-	`sha256:f502d9205a82eac738351ebd7f9768c88303d3a0e1c4f6acdefe4b24afc3300c`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 3.6 MB (3591665 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:08e9697cd0098392496fcb0ea480b3cad6e8de850a8abcb6a6050ab76ea0fd72`  
		Last Modified: Sat, 02 Dec 2023 10:09:40 GMT  
		Size: 35.8 KB (35834 bytes)  
		MIME: application/vnd.in-toto+json
