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
