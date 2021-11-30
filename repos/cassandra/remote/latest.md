## `cassandra:latest`

```console
$ docker pull cassandra@sha256:c186d79dca1cebe1ce382aaba201cce08b0f415e850d4b9eb6c1317f02bea293
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `cassandra:latest` - linux; amd64

```console
$ docker pull cassandra@sha256:ff5c38ec345b34b0305ca2138d710662247656a18ad9ee57284dd3925c547e51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.9 MB (149916919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e185c0e3501c39fd23a856afaeaf516a421e6f647f8df6f35b7c59d19429e37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:21:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:22:21 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 20:22:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='76f7da05d905b5f9de8de1a34c1a206744f7589bf0eed876cd9069cb1d913806';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='aee2f20d005b58e79c3c6c02271f797cb387d33a135b762886990b9bf7cb262e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f267876675dac3da3f4ceccd44d812b57098505eeec5fb1688d54bdeffcd1da';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b4a5af4ffcc98f6b7cdd2232f79aa12f20efa769b5255277fa4974e2e19d4409';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb0a27e6e1f26a1ee79daa92e4cfe3ec0d676acfe114d99dd84b3414f056e8a0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:22:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:22:48 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 30 Nov 2021 01:12:32 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Tue, 30 Nov 2021 01:12:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Tue, 30 Nov 2021 01:12:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 30 Nov 2021 01:13:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 01:13:02 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Tue, 30 Nov 2021 01:13:03 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Tue, 30 Nov 2021 01:13:03 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 01:13:03 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Tue, 30 Nov 2021 01:13:03 GMT
ENV CASSANDRA_VERSION=4.0.1
# Tue, 30 Nov 2021 01:13:03 GMT
ENV CASSANDRA_SHA512=2890c054666afa93fe2978c46da5db15ed7d11d60f4890574dc642bd81f7b3af40b41d3e5b8245e6c1453a165eddebeb28bcf3fef1a2b2fc6fb3b82058d7ceb0
# Tue, 30 Nov 2021 01:13:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Tue, 30 Nov 2021 01:13:36 GMT
VOLUME [/var/lib/cassandra]
# Tue, 30 Nov 2021 01:13:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Tue, 30 Nov 2021 01:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 01:13:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Tue, 30 Nov 2021 01:13:37 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c122ee837fa892e5fdd4f7c857600f80a7b8fa855d2475bb325372d55eaff04`  
		Last Modified: Mon, 29 Nov 2021 20:25:31 GMT  
		Size: 24.8 MB (24814948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060f1998a9aba4fee813599796e2502aac2844a51a791fdccdf274824664cb50`  
		Last Modified: Mon, 29 Nov 2021 20:26:41 GMT  
		Size: 43.2 MB (43201085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d68b8b292ea2456da9c58fc765ee49e44c5b1e640c6ec5ec01f7db864df5606`  
		Last Modified: Mon, 29 Nov 2021 20:26:35 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa81e9d8a3ab7ffcd5e3d8cc7a42f882f48916307d862d598ee83cd41ef565`  
		Last Modified: Tue, 30 Nov 2021 01:15:52 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8a264b599dc8d5563ff8175d85057582fb7955bebf2bcac5cc36bd3a1cb995`  
		Last Modified: Tue, 30 Nov 2021 01:15:52 GMT  
		Size: 2.2 MB (2160812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8983c926a1c989fd889800d814a67d9d1e5222f0a6fa2d61d114297f774944`  
		Last Modified: Tue, 30 Nov 2021 01:15:52 GMT  
		Size: 1.3 MB (1315971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1802c7f27836310bb292187df1986df35ff8c546dab154ea91ef3d5cfd9e921c`  
		Last Modified: Tue, 30 Nov 2021 01:15:56 GMT  
		Size: 49.9 MB (49853868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcd8d5209834ffb5d3f822ad25d5e5f7382f7b420ad27547727c7c55e3d7964`  
		Last Modified: Tue, 30 Nov 2021 01:15:51 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; arm variant v7

```console
$ docker pull cassandra@sha256:facc06df16bab2aba52bbde87f3bb0ecba532f69b16d75b658826183731f2567
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142011661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7393602330578b6b1e0dd4ad656bd66d8e6012bf12cf8d12c07c0787bc47579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:58:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:59:57 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 20:00:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='76f7da05d905b5f9de8de1a34c1a206744f7589bf0eed876cd9069cb1d913806';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='aee2f20d005b58e79c3c6c02271f797cb387d33a135b762886990b9bf7cb262e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f267876675dac3da3f4ceccd44d812b57098505eeec5fb1688d54bdeffcd1da';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b4a5af4ffcc98f6b7cdd2232f79aa12f20efa769b5255277fa4974e2e19d4409';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb0a27e6e1f26a1ee79daa92e4cfe3ec0d676acfe114d99dd84b3414f056e8a0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:00:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:00:53 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 21:57:10 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Mon, 29 Nov 2021 21:57:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Mon, 29 Nov 2021 21:57:23 GMT
ENV GOSU_VERSION=1.12
# Mon, 29 Nov 2021 21:57:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 29 Nov 2021 21:57:43 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 29 Nov 2021 21:57:44 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 29 Nov 2021 21:57:44 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 21:57:45 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Mon, 29 Nov 2021 21:57:45 GMT
ENV CASSANDRA_VERSION=4.0.1
# Mon, 29 Nov 2021 21:57:46 GMT
ENV CASSANDRA_SHA512=2890c054666afa93fe2978c46da5db15ed7d11d60f4890574dc642bd81f7b3af40b41d3e5b8245e6c1453a165eddebeb28bcf3fef1a2b2fc6fb3b82058d7ceb0
# Mon, 29 Nov 2021 21:58:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Mon, 29 Nov 2021 21:58:35 GMT
VOLUME [/var/lib/cassandra]
# Mon, 29 Nov 2021 21:58:36 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:58:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Nov 2021 21:58:36 GMT
EXPOSE 7000 7001 7199 9042 9160
# Mon, 29 Nov 2021 21:58:37 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f49a73fe087725ab5b9956d86afb7a1ca7735fe7eb993e92d61d1d780acba64`  
		Last Modified: Mon, 29 Nov 2021 20:05:51 GMT  
		Size: 23.1 MB (23068723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc737d2b5103dbc4a72b621b5299b2d7ebcd1f47bb90c5b2ee006cf4da3a93`  
		Last Modified: Mon, 29 Nov 2021 20:08:58 GMT  
		Size: 41.8 MB (41815184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80530a9d33f73ee9ddebbebb5e081e02740350c2831411c5cd79c46761461b0c`  
		Last Modified: Mon, 29 Nov 2021 20:08:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eab7cc3eb5dbbc8f6c16cd6ad0c860b9fad39e517f497df1fad14359b73003`  
		Last Modified: Mon, 29 Nov 2021 21:59:16 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f144f95a3ff463b965746ae93c8347cf2a6006a4b7cd3c0caca2a4caa136c1`  
		Last Modified: Mon, 29 Nov 2021 21:59:17 GMT  
		Size: 1.9 MB (1936167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511be5c00a9953850df650201865ea53e7580cb81bd71704bddca92761dbb2fc`  
		Last Modified: Mon, 29 Nov 2021 21:59:17 GMT  
		Size: 1.3 MB (1269259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c8499694630a6d3c2165053a8732055da8944d16dab35cc5de6cabb4172665`  
		Last Modified: Mon, 29 Nov 2021 21:59:31 GMT  
		Size: 49.9 MB (49854743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c981eac238fb993a549af170e3a5fd0101ed53b05f4b14df82b8a4cb4553216a`  
		Last Modified: Mon, 29 Nov 2021 21:59:16 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; arm64 variant v8

```console
$ docker pull cassandra@sha256:ce2bc0b6ae1eada48deefcd03ec43f1de9b8c9c748232915a7fd8e5e18bba6b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.2 MB (146208063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abe8e2dbfcd3afd24830eaa1e72584f50eff196c9dd92118fa3d5445866040d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:25:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:40:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:40:43 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 19:41:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='76f7da05d905b5f9de8de1a34c1a206744f7589bf0eed876cd9069cb1d913806';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='aee2f20d005b58e79c3c6c02271f797cb387d33a135b762886990b9bf7cb262e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f267876675dac3da3f4ceccd44d812b57098505eeec5fb1688d54bdeffcd1da';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b4a5af4ffcc98f6b7cdd2232f79aa12f20efa769b5255277fa4974e2e19d4409';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb0a27e6e1f26a1ee79daa92e4cfe3ec0d676acfe114d99dd84b3414f056e8a0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 19:41:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 19:41:16 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:53:38 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Mon, 29 Nov 2021 20:53:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Mon, 29 Nov 2021 20:53:48 GMT
ENV GOSU_VERSION=1.12
# Mon, 29 Nov 2021 20:54:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 29 Nov 2021 20:54:02 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 29 Nov 2021 20:54:03 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 29 Nov 2021 20:54:04 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:54:05 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Mon, 29 Nov 2021 20:54:06 GMT
ENV CASSANDRA_VERSION=4.0.1
# Mon, 29 Nov 2021 20:54:07 GMT
ENV CASSANDRA_SHA512=2890c054666afa93fe2978c46da5db15ed7d11d60f4890574dc642bd81f7b3af40b41d3e5b8245e6c1453a165eddebeb28bcf3fef1a2b2fc6fb3b82058d7ceb0
# Mon, 29 Nov 2021 20:54:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Mon, 29 Nov 2021 20:54:55 GMT
VOLUME [/var/lib/cassandra]
# Mon, 29 Nov 2021 20:54:57 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Nov 2021 20:54:58 GMT
EXPOSE 7000 7001 7199 9042 9160
# Mon, 29 Nov 2021 20:54:59 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa42563dc02061b51ce62bff7340de9cea06ea720e8658d2a7693902aa8f700`  
		Last Modified: Mon, 29 Nov 2021 19:44:11 GMT  
		Size: 24.8 MB (24763049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101fa15230f89da61eea58b54b9d024d06737226966fe8f8c5171944f7fb4979`  
		Last Modified: Mon, 29 Nov 2021 19:45:35 GMT  
		Size: 41.5 MB (41518776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32a871c058540a54a618d3b3727d761f8693bb09d004cd9b726a47b559c9e7`  
		Last Modified: Mon, 29 Nov 2021 19:45:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b9a0fa872298d537ab5099b488679e0f83303f84ebe452bc929896479abcb5`  
		Last Modified: Mon, 29 Nov 2021 20:57:14 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20707b0292da66d15b464b40c18ee4ee0226e5c7d3385e2910b260506d064b74`  
		Last Modified: Mon, 29 Nov 2021 20:57:14 GMT  
		Size: 2.1 MB (2129221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0ada430cba0de731fc7f71222d4cd4464cd0df1e40d0d1bff751b87266c096`  
		Last Modified: Mon, 29 Nov 2021 20:57:14 GMT  
		Size: 1.0 MB (1010331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cba36b9aaf99a1001fc191dcb112c33d0d9c632fbdb150c74f8795951abd0`  
		Last Modified: Mon, 29 Nov 2021 20:57:18 GMT  
		Size: 49.6 MB (49612701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a4f063da9d8a0fd982fcba8e087b67ec09f86c2e685a4a731720b85dd002db`  
		Last Modified: Mon, 29 Nov 2021 20:57:14 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cassandra:latest` - linux; ppc64le

```console
$ docker pull cassandra@sha256:12385626754700a983fbe275018b96d2c7ec35f39f533586d4232634662105bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152161269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554f97b529d68087ef5963d686c44b1f28d3d6d5bab68ea25e02cd0ee6435dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["cassandra","-f"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:18:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:19:43 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 20:20:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='76f7da05d905b5f9de8de1a34c1a206744f7589bf0eed876cd9069cb1d913806';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='aee2f20d005b58e79c3c6c02271f797cb387d33a135b762886990b9bf7cb262e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f267876675dac3da3f4ceccd44d812b57098505eeec5fb1688d54bdeffcd1da';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='b4a5af4ffcc98f6b7cdd2232f79aa12f20efa769b5255277fa4974e2e19d4409';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fb0a27e6e1f26a1ee79daa92e4cfe3ec0d676acfe114d99dd84b3414f056e8a0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:20:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:20:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 23:15:01 GMT
RUN set -eux; 	groupadd -r cassandra --gid=999; 	useradd -r -g cassandra --uid=999 cassandra
# Mon, 29 Nov 2021 23:15:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libjemalloc2 		procps 		python3 		iproute2 		numactl 	; 	rm -rf /var/lib/apt/lists/*; 	libjemalloc="$(readlink -e /usr/lib/*/libjemalloc.so.2)"; 	ln -sT "$libjemalloc" /usr/local/lib/libjemalloc.so; 	ldconfig
# Mon, 29 Nov 2021 23:15:25 GMT
ENV GOSU_VERSION=1.12
# Mon, 29 Nov 2021 23:16:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 29 Nov 2021 23:16:03 GMT
ENV CASSANDRA_HOME=/opt/cassandra
# Mon, 29 Nov 2021 23:16:04 GMT
ENV CASSANDRA_CONF=/etc/cassandra
# Mon, 29 Nov 2021 23:16:05 GMT
ENV PATH=/opt/cassandra/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 23:16:07 GMT
ENV GPG_KEYS=CEC86BB4A0BA9D0F90397CAEF8358FA2F2833C93 	C4965EE9E3015D192CCCF2B6F758CE318D77295D 	5AED1BF378E9A19DADE1BCB34BD736A82B5C1B00 	514A2AD631A57A16DD0047EC749D6EEC0353B12C 	A26E528B271F19B9E5D8E19EA278B781FE4B2BDA 	A4C465FEA0C552561A392A61E91335D77E3E87CB 	9E66CEC6106D578D0B1EB9BFF1000962B7F6840C 	C4009872C59B49561310D966D0062876AF30F054 	B7842CDAF36E6A3214FAE35D5E85B9AE0B84C041 	3E9C876907A560ACA00964F363E9BAD215BBF5F0 	F8B7FD00E05C932991A2CD6150EE103D162C5A55
# Mon, 29 Nov 2021 23:16:09 GMT
ENV CASSANDRA_VERSION=4.0.1
# Mon, 29 Nov 2021 23:16:11 GMT
ENV CASSANDRA_SHA512=2890c054666afa93fe2978c46da5db15ed7d11d60f4890574dc642bd81f7b3af40b41d3e5b8245e6c1453a165eddebeb28bcf3fef1a2b2fc6fb3b82058d7ceb0
# Mon, 29 Nov 2021 23:17:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget --progress=dot:giga -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'cassandra-bin.tgz' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz"; 	echo "$CASSANDRA_SHA512 *cassandra-bin.tgz" | sha512sum --check --strict -; 		ddist 'cassandra-bin.tgz.asc' "cassandra/$CASSANDRA_VERSION/apache-cassandra-$CASSANDRA_VERSION-bin.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify cassandra-bin.tgz.asc cassandra-bin.tgz; 	rm -rf "$GNUPGHOME"; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		mkdir -p "$CASSANDRA_HOME"; 	tar --extract --file cassandra-bin.tgz --directory "$CASSANDRA_HOME" --strip-components 1; 	rm cassandra-bin.tgz*; 		[ ! -e "$CASSANDRA_CONF" ]; 	mv "$CASSANDRA_HOME/conf" "$CASSANDRA_CONF"; 	ln -sT "$CASSANDRA_CONF" "$CASSANDRA_HOME/conf"; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		ppc64el) 			if grep -q -- '^-Xss' "$CASSANDRA_CONF/jvm.options"; then 				grep -- '^-Xss256k$' "$CASSANDRA_CONF/jvm.options"; 				sed -ri 's/^-Xss256k$/-Xss512k/' "$CASSANDRA_CONF/jvm.options"; 				grep -- '^-Xss512k$' "$CASSANDRA_CONF/jvm.options"; 			elif grep -q -- '-Xss256k' "$CASSANDRA_CONF/cassandra-env.sh"; then 				sed -ri 's/-Xss256k/-Xss512k/g' "$CASSANDRA_CONF/cassandra-env.sh"; 				grep -- '-Xss512k' "$CASSANDRA_CONF/cassandra-env.sh"; 			fi; 			;; 	esac; 		mkdir -p "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chown -R cassandra:cassandra "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod 777 "$CASSANDRA_CONF" /var/lib/cassandra /var/log/cassandra; 	chmod -R a+rwX "$CASSANDRA_CONF"; 	ln -sT /var/lib/cassandra "$CASSANDRA_HOME/data"; 	ln -sT /var/log/cassandra "$CASSANDRA_HOME/logs"; 		cassandra -v
# Mon, 29 Nov 2021 23:17:04 GMT
VOLUME [/var/lib/cassandra]
# Mon, 29 Nov 2021 23:17:05 GMT
COPY file:a8d4fc10252d8783a105c235b3eef2315dbe3b0b1be0f1e4650f19fa5a56ab29 in /usr/local/bin/ 
# Mon, 29 Nov 2021 23:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Nov 2021 23:17:11 GMT
EXPOSE 7000 7001 7199 9042 9160
# Mon, 29 Nov 2021 23:17:13 GMT
CMD ["cassandra" "-f"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce46da97c533978caacb28d5a66ed1f0b6374622ee6806ebe49cc2fa004597f`  
		Last Modified: Mon, 29 Nov 2021 20:25:42 GMT  
		Size: 26.6 MB (26647174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8269e16c15316b550660b9994c851cab79f9fdebdf42c79b8529f0aee69143`  
		Last Modified: Mon, 29 Nov 2021 20:27:10 GMT  
		Size: 38.6 MB (38610182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c82f11e0647d3ee00a96acb9ec278aac47c4b5b8fde3cec519fad7146843088`  
		Last Modified: Mon, 29 Nov 2021 20:27:01 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c41271c9a2b8152a44dce03a10f54a06825e94072aae67a7ff8cefcbcc4966a`  
		Last Modified: Mon, 29 Nov 2021 23:22:02 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7bbfb23d955654bc15f44d2e665248f7ab3bb59445b65469139bc58e9b2e0f`  
		Last Modified: Mon, 29 Nov 2021 23:22:02 GMT  
		Size: 2.5 MB (2522984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d6dc3a79179d3b59892ca8a38a1a00bad8f964e03c29bc7c776d8ef73f85b4`  
		Last Modified: Mon, 29 Nov 2021 23:22:03 GMT  
		Size: 1.2 MB (1236158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aabd645966470febf98c760de29dfa5113e61f0d8e84cdf9877aaa3ba4140f`  
		Last Modified: Mon, 29 Nov 2021 23:22:07 GMT  
		Size: 49.9 MB (49854395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f021656b24ceb3b5833ae8408c70bb7fa5128fcb0214b724f67b21910a9e406b`  
		Last Modified: Mon, 29 Nov 2021 23:22:02 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
