## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:7904e2706bf7be76ea97822345d4c86c162ca24c1c0273e25281c0f4c013ae12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:c2288abd87e769289ff9be69d441e3295b4779a696d6d82d88bc41c3f1aa8836
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69122086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78588ad09ca600979371a29f66d39f2b8508f3eb7a2547f303d40db20d32ad63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:13:12 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 07 Oct 2022 03:13:12 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 07 Oct 2022 03:13:12 GMT
ENV OPENSSL_VERSION=1.1.1q
# Fri, 07 Oct 2022 03:13:12 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Fri, 07 Oct 2022 03:13:12 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 07 Oct 2022 03:13:12 GMT
ENV OTP_VERSION=25.1.1
# Fri, 07 Oct 2022 03:13:12 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Fri, 07 Oct 2022 03:15:57 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 07 Oct 2022 03:15:57 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 07 Oct 2022 03:15:58 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:44:20 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:44:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:44:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:44:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:44:29 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:44:31 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:44:31 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:44:31 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:44:31 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:44:32 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:44:32 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:44:32 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:44:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:44:32 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:44:32 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318d296d987c600b27b56ffd11690e1b378d300d81629ee8ff94ed7358d50511`  
		Last Modified: Fri, 07 Oct 2022 03:17:58 GMT  
		Size: 1.4 MB (1442754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94935948487e4b46ec394bbf7fae7eb8d0e24537c2d15b751074d24c402293f`  
		Last Modified: Fri, 07 Oct 2022 03:18:03 GMT  
		Size: 47.5 MB (47499539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b965c5965a73ecbee8bd61fa4fb3f61d558da0ee1808d634dbf328a0cc6ed2`  
		Last Modified: Fri, 07 Oct 2022 03:17:57 GMT  
		Size: 1.5 KB (1489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f2d8e6ff45414fdbeda7e24659f7b6302dce37c172f42ac5d9885b8c277f2`  
		Last Modified: Wed, 19 Oct 2022 19:46:06 GMT  
		Size: 17.4 MB (17370527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061cc2135d4c05c33d7c61bcf35eb3c1a64c3c015e0365620447603f82e0b5e0`  
		Last Modified: Wed, 19 Oct 2022 19:46:05 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84ee15c8b718ae0316a8370a666de27ecf818ec1e061c6a6ef4e1f625361756`  
		Last Modified: Wed, 19 Oct 2022 19:46:05 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e60a40d72f1b2f1d21adeec97a5b1bc3d94157b70d447f1bd4bab9b667b5d32`  
		Last Modified: Wed, 19 Oct 2022 19:46:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb5fb58ab025b190900262b549f9548a8af294a880f4428547972d2379cb788`  
		Last Modified: Wed, 19 Oct 2022 19:46:05 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:0e6021c5b35ecca7be63e10d23b6ec5271309f0a548a308903da1cd335200484
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59915296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c9767e89f60b2ee474d6bd75b96e79d28a7237c52c6937e3e9250b5daa635b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 02:31:32 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Sat, 08 Oct 2022 02:31:32 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Sat, 08 Oct 2022 02:31:32 GMT
ENV OPENSSL_VERSION=1.1.1q
# Sat, 08 Oct 2022 02:31:33 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Sat, 08 Oct 2022 02:31:33 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Sat, 08 Oct 2022 02:31:33 GMT
ENV OTP_VERSION=25.1.1
# Sat, 08 Oct 2022 02:31:33 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Sat, 08 Oct 2022 02:39:45 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Sat, 08 Oct 2022 02:39:45 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 08 Oct 2022 02:39:46 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:56:15 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:56:15 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:56:15 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:56:15 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:56:31 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:56:35 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:56:35 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:56:35 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:56:36 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:56:36 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:56:36 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:56:36 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:56:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:56:36 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:56:36 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7809ae365a96aea9451be5ebcc3e9ffdd5a7f522a65e467e04f217ec3ae732e8`  
		Last Modified: Sat, 08 Oct 2022 02:42:59 GMT  
		Size: 1.4 MB (1400781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced579b22b2076a85db505d4214a1bc376e62a02d7d1a9136ee53fd1aaf5008`  
		Last Modified: Sat, 08 Oct 2022 02:43:05 GMT  
		Size: 38.5 MB (38526869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21862477bdfcc26af445945f819d3ce40f39cb09627fe4b04f22d35f511c01a6`  
		Last Modified: Sat, 08 Oct 2022 02:42:59 GMT  
		Size: 1.5 KB (1491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879a2d0650ec9543f1d41497e3a61fd78f61cd145c3ae6c892f2a476d7f0a83`  
		Last Modified: Wed, 19 Oct 2022 19:58:02 GMT  
		Size: 17.4 MB (17370470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d93f58de39ca7a1e1994af1a845409457fb46a6fab5390fc6faf768d1fb4b9`  
		Last Modified: Wed, 19 Oct 2022 19:57:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e01c9d8bd20333590fb36f594ba84ef81b2610f582fd88c7b348e088c659e`  
		Last Modified: Wed, 19 Oct 2022 19:57:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecab7b3c907925106487c215a641b0145393475fa288d70ffd5a2f298d2eba`  
		Last Modified: Wed, 19 Oct 2022 19:57:59 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd55a6ed7af41c9cd736d194f35ec45158c2294017550e8ca4c374e654cae37`  
		Last Modified: Wed, 19 Oct 2022 19:57:58 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:dd3ed04ed097346db49340d6e10357174b75f43298ec520785910f5a468dbc18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59227972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c02d1ff2073fa9c34c0142c62c872fb5cf581b615b6a321dfced7d149ae71690`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 03:32:27 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Sat, 08 Oct 2022 03:32:28 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Sat, 08 Oct 2022 03:32:28 GMT
ENV OPENSSL_VERSION=1.1.1q
# Sat, 08 Oct 2022 03:32:28 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Sat, 08 Oct 2022 03:32:28 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Sat, 08 Oct 2022 03:32:28 GMT
ENV OTP_VERSION=25.1.1
# Sat, 08 Oct 2022 03:32:28 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Sat, 08 Oct 2022 03:41:12 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Sat, 08 Oct 2022 03:41:13 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 08 Oct 2022 03:41:13 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:21:27 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:21:27 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:21:27 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:21:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:21:35 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:21:36 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:21:37 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:21:37 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:21:37 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:21:37 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:21:37 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:21:37 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:21:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:21:37 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:21:38 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a33b0282f220bfec79aa77429da113a29bfc90116838b37d967b4b99851288`  
		Last Modified: Sat, 08 Oct 2022 03:44:44 GMT  
		Size: 1.3 MB (1309561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b498c0b76514600c8ef71e77f45446666b1a9b30cb606578d98bb4b5072b5e2`  
		Last Modified: Sat, 08 Oct 2022 03:44:50 GMT  
		Size: 38.1 MB (38127649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1a672219ec4bfafe3065a710411347a47e097214da63214132648baa3773e`  
		Last Modified: Sat, 08 Oct 2022 03:44:43 GMT  
		Size: 1.5 KB (1493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7efd28e31781b1d530cdd1b3b1fd06f7914af2025e675af8cb3cccc63df1deb`  
		Last Modified: Wed, 19 Oct 2022 20:24:23 GMT  
		Size: 17.4 MB (17370485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f034efd62530520114792474e50e1b1973a0e82ade37d1959610d3e548928d5`  
		Last Modified: Wed, 19 Oct 2022 20:24:21 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eb51e82accdb90c3715ce7ac7773de719e4c58b8ffbaba824e11fbab0fb049`  
		Last Modified: Wed, 19 Oct 2022 20:24:22 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3275f2ed4e58686f834e603d0de167768d02488e1198c835b24a3f73470b7c0`  
		Last Modified: Wed, 19 Oct 2022 20:24:21 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a34863e582b0ab3cd6840f9392bd34c4f0c226e78c78f6050a699eefe825517`  
		Last Modified: Wed, 19 Oct 2022 20:24:21 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:03fd607b99d851cc0f210c5ca63c2ce095d511ec301fb249ce6f4adac6451acd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66756336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842af53426ac34cf5250058c5ac408035339e4ced3ca55f0d5e0ea3b36c2f4c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 06:36:21 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 07 Oct 2022 06:36:22 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 07 Oct 2022 06:36:23 GMT
ENV OPENSSL_VERSION=1.1.1q
# Fri, 07 Oct 2022 06:36:24 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Fri, 07 Oct 2022 06:36:25 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 07 Oct 2022 06:36:26 GMT
ENV OTP_VERSION=25.1.1
# Fri, 07 Oct 2022 06:36:27 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Fri, 07 Oct 2022 06:39:28 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 07 Oct 2022 06:39:29 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 07 Oct 2022 06:39:30 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:09:18 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:09:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:09:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:09:21 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:09:30 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:09:32 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:09:33 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:09:34 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:09:35 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:09:36 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:09:38 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:09:39 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:09:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:09:40 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:09:41 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bd7cfcf5941ffbcc27aa82446023e3356d35bf61028d5fcc0d1291fd3c105e`  
		Last Modified: Fri, 07 Oct 2022 06:42:54 GMT  
		Size: 1.5 MB (1467121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bae94bce5c6ec2fcd7371e78514a90c08190f569dd5e7dfafc250f4fb02e7a`  
		Last Modified: Fri, 07 Oct 2022 06:42:59 GMT  
		Size: 45.2 MB (45208128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e97f253fe20fb9cf8393b16d0c90acccffd11d18dd66efeadc556d95e280424`  
		Last Modified: Fri, 07 Oct 2022 06:42:53 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cd92256a261692df7c21b3479480c2836a0a95dd8a183c5900a5c83b22bb2`  
		Last Modified: Wed, 19 Oct 2022 20:12:10 GMT  
		Size: 17.4 MB (17370278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf99adb54c7f306b15115c874559a293d89f543fc11cd10835ad7af0aec52a7`  
		Last Modified: Wed, 19 Oct 2022 20:12:08 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d395135a38a5410ec6f6b2acb31af183b4f72dee4615117a4e5d3238124bc728`  
		Last Modified: Wed, 19 Oct 2022 20:12:08 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2f3300433853a485c16e322efc52a2dace54d713708067337def8653b4697b`  
		Last Modified: Wed, 19 Oct 2022 20:12:08 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f7f3896ac115f66682b343bbefd466d4f8b4c3181e05e0200afa40299852ec`  
		Last Modified: Wed, 19 Oct 2022 20:12:08 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:dd20ed95f29889484f5a29910d64f48d92eb7ff93ae6d08ee4ee832f6e8da83e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61369347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c658ef64ea5ec79c13fd7bc16f02a4d487d15dbf9d4283e7db6a2a52423507eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:21:41 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 07 Oct 2022 01:21:42 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 07 Oct 2022 01:21:43 GMT
ENV OPENSSL_VERSION=1.1.1q
# Fri, 07 Oct 2022 01:21:44 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Fri, 07 Oct 2022 01:21:45 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 07 Oct 2022 01:21:46 GMT
ENV OTP_VERSION=25.1.1
# Fri, 07 Oct 2022 01:21:47 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Fri, 07 Oct 2022 01:24:28 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 07 Oct 2022 01:24:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 07 Oct 2022 01:24:29 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:55:42 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:55:43 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:55:44 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:55:45 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:55:54 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:55:55 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:55:56 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:55:57 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:55:58 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:55:59 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:56:01 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:56:02 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:56:03 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:56:04 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68152d48c2675b07ae45205ee8c19c2c3f5922cf8a450fd2c582906c496f0468`  
		Last Modified: Fri, 07 Oct 2022 01:27:11 GMT  
		Size: 1.5 MB (1503564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfd851e1a18db07601370f9238d8167a6f0c8c3c65bcecfb65a46d3dc81ca3d`  
		Last Modified: Fri, 07 Oct 2022 01:27:15 GMT  
		Size: 39.7 MB (39685345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229357e69dcdd66b799f308a2e1ad29ccc7818f39e03f6330c47e34fa3d94d4a`  
		Last Modified: Fri, 07 Oct 2022 01:27:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07578005786deeff9105a7e578e62b9612752d5082fd91b182f43f22ece3fdbe`  
		Last Modified: Wed, 19 Oct 2022 19:57:11 GMT  
		Size: 17.4 MB (17370172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c0720557bd29bdf905ddcf480af10ba3d78ad0e38a8a61b2a69decd3a1d17`  
		Last Modified: Wed, 19 Oct 2022 19:57:09 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e1c6be9f97c5abb2f28f2f17b15698c9cdf55675f0a8417087edacc08a38b7`  
		Last Modified: Wed, 19 Oct 2022 19:57:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17e00598fdf8696ae6a91f619677aa5cc274733dfad1a3d8a6c6cd50afd5bd9`  
		Last Modified: Wed, 19 Oct 2022 19:57:09 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd260d9ac344c30f86b5930e6250130ad83e74a79aa8e35c90651bc94b036971`  
		Last Modified: Wed, 19 Oct 2022 19:57:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:261ea4faa01705432d125cf12c4644df5c9cbde0483157c981dfd203b8698af9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61742094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cada104be3a410775ac6274451e47b4279add81153b236970f289906d09b8972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 06:44:25 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 07 Oct 2022 06:44:26 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 07 Oct 2022 06:44:26 GMT
ENV OPENSSL_VERSION=1.1.1q
# Fri, 07 Oct 2022 06:44:26 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Fri, 07 Oct 2022 06:44:27 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 07 Oct 2022 06:44:27 GMT
ENV OTP_VERSION=25.1.1
# Fri, 07 Oct 2022 06:44:27 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Fri, 07 Oct 2022 06:47:39 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 07 Oct 2022 06:47:41 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 07 Oct 2022 06:47:42 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 19:41:09 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 19:41:09 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 19:41:09 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 19:41:09 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 19:41:23 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 19:41:26 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 19:41:28 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 19:41:28 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 19:41:29 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 19:41:29 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 19:41:30 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 19:41:30 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:41:31 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 19:41:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f729487fa5e92b7b31a26d77fca5059f591d5477c25e5182b85b5f8ce018c7d`  
		Last Modified: Fri, 07 Oct 2022 06:51:18 GMT  
		Size: 1.6 MB (1573167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683c104c174aaebd7809dcb873444dca84c4657010fa05a6e2ac3889f8dd7119`  
		Last Modified: Fri, 07 Oct 2022 06:51:25 GMT  
		Size: 40.0 MB (39991912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5f65ca9909bcfa45d470dd293de81f70171caf0727ab1a07c69f93fb780001`  
		Last Modified: Fri, 07 Oct 2022 06:51:17 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d718ba5fc2c8b28320ed40cb01fc653a57c3ee167a07b302d324f695f754c8`  
		Last Modified: Wed, 19 Oct 2022 19:44:18 GMT  
		Size: 17.4 MB (17370482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b29e95f2a2238a96836f5dbf8d0e1faf8ca868ed324e47183b9c61a00b86391`  
		Last Modified: Wed, 19 Oct 2022 19:44:16 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75bf29009f459ae2bc2894f67dca443339e16aa1c8ffdf70cb719d81a9d0168`  
		Last Modified: Wed, 19 Oct 2022 19:44:16 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1683b9286b720a4e1a917dc2bdb086e008d6b7aa8e96380f3cf153005753016a`  
		Last Modified: Wed, 19 Oct 2022 19:44:16 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9420e1571ca990af3186f565d4ab1d11489b5c879a719e0660829c2266d882`  
		Last Modified: Wed, 19 Oct 2022 19:44:16 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:02f987e4983c936a777c30c05e8df3f68dabef4088df2d37d01a4d09dbf99663
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59933118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8dcbcf447b8c8b9d5d0b7331280adcba0194beea2ae93980cb200756f516522`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:02:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 07 Oct 2022 09:02:36 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 07 Oct 2022 09:02:36 GMT
ENV OPENSSL_VERSION=1.1.1q
# Fri, 07 Oct 2022 09:02:37 GMT
ENV OPENSSL_SOURCE_SHA256=d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca
# Fri, 07 Oct 2022 09:02:37 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 07 Oct 2022 09:02:37 GMT
ENV OTP_VERSION=25.1.1
# Fri, 07 Oct 2022 09:02:38 GMT
ENV OTP_SOURCE_SHA256=42840c32e13a27bdb2c376d69aa22466513d441bfe5eb882de23baf8218308d3
# Fri, 07 Oct 2022 09:06:29 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 07 Oct 2022 09:06:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 07 Oct 2022 09:06:32 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Wed, 19 Oct 2022 20:17:35 GMT
ENV RABBITMQ_VERSION=3.11.2
# Wed, 19 Oct 2022 20:17:36 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Wed, 19 Oct 2022 20:17:36 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Wed, 19 Oct 2022 20:17:37 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Oct 2022 20:17:53 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Wed, 19 Oct 2022 20:17:56 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Wed, 19 Oct 2022 20:17:56 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Wed, 19 Oct 2022 20:17:57 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 19 Oct 2022 20:17:57 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 19 Oct 2022 20:17:57 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 19 Oct 2022 20:17:58 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Wed, 19 Oct 2022 20:17:58 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Wed, 19 Oct 2022 20:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 20:17:59 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Wed, 19 Oct 2022 20:17:59 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ef4c666c3b38a15155683ed9e9cabc5abe28e68b8f8c84a6aabfa13a7b13c`  
		Last Modified: Fri, 07 Oct 2022 09:11:10 GMT  
		Size: 1.5 MB (1494107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ba060c807c788f10bffcbe53e9b9547b21c420c2c3cec45fe9d00b9a66172c`  
		Last Modified: Fri, 07 Oct 2022 09:11:13 GMT  
		Size: 38.5 MB (38474724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbc6d822f848b5920487811087015d254e22ab6cd1f25d43e2d32915a4250c`  
		Last Modified: Fri, 07 Oct 2022 09:11:09 GMT  
		Size: 1.5 KB (1491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4893a7503ec0a97bff87b8a256962dc9e6dbf37889d4f092666da5c123a13444`  
		Last Modified: Wed, 19 Oct 2022 20:22:18 GMT  
		Size: 17.4 MB (17370477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1741f83e4c66172ea94e6ee530ce9c78664e6f326cac9ec9aa24e53f19d32f`  
		Last Modified: Wed, 19 Oct 2022 20:22:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447e5679a4278b6df3e1cda1b489cf4c4183a3925e139ed7c4fe66f22a5a29f9`  
		Last Modified: Wed, 19 Oct 2022 20:22:17 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e3755cc94f0e1827b35593219e835ef57bc14c6fe015305e6ded745310257b`  
		Last Modified: Wed, 19 Oct 2022 20:22:17 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b66a4789b502717c11910f95dbf47718fab278dec01d91e00667f5b418f257`  
		Last Modified: Wed, 19 Oct 2022 20:22:17 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
