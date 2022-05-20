## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:b4bbc6e1f1c9ced180afa97f73af3a6d2cf81eeed8995647fce7bb203e91926e
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

### `rabbitmq:3-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:1b3aedd7ede70b9721f2f3ea8d90ba4fd8592c6d47ecde6ae6c5532fd1152dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82116956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbbf172901dc4986539242b4665fab04c2b6d13a173b0e59ad5956c1120a972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:19:51 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 11:19:51 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:29:49 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:29:49 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:29:49 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:29:49 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:29:49 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:32:24 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:32:24 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:32:25 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 21:55:44 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 21:55:44 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 21:55:44 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 21:55:44 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 21:55:52 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 21:55:54 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 21:55:54 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 21:55:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 21:55:55 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 21:55:55 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 21:55:55 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 21:55:55 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 21:55:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 21:55:55 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 21:55:55 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 21:56:02 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 21:56:02 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367ecfcc737e874ea4275a24293e6d70a8c5ac59782d5eca8914b95b60682912`  
		Last Modified: Tue, 05 Apr 2022 11:25:47 GMT  
		Size: 1.1 MB (1053981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2390758a14ac4d0a6f30575cf1387132f4eb1f21e2a12afb85b3a5203c809`  
		Last Modified: Tue, 03 May 2022 19:35:59 GMT  
		Size: 47.0 MB (46985326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f4b11a85e9cef11e70488447bed590c5bebb9cf1089dbd050962d1c54d2586`  
		Last Modified: Tue, 03 May 2022 19:35:53 GMT  
		Size: 1.5 KB (1489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ca71e749d2c1d2bdac0130fc4ab233596a29a7c82a59fc889a4ed882af187d`  
		Last Modified: Fri, 20 May 2022 21:59:10 GMT  
		Size: 16.9 MB (16851822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d5174db67f5688a6c4d392007e45fe313e01298d153fa114db3a0556f6c62`  
		Last Modified: Fri, 20 May 2022 21:59:09 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c337472a84b7d9e74e42b9b904126ad137c26e077b484b87e4e0d87103bbd57`  
		Last Modified: Fri, 20 May 2022 21:59:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4244133915f007b952be9581517486467a9ef6fab6d3a17a07d801448b0e62fc`  
		Last Modified: Fri, 20 May 2022 21:59:09 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4ae04f5222ead59e42033222d4ec74ff9b844fa61503f0d2a2ba776858998d`  
		Last Modified: Fri, 20 May 2022 21:59:09 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4401220100bb3446a53da10c1a75abcc1877cae23db3f37693181ef57949a9f9`  
		Last Modified: Fri, 20 May 2022 21:59:27 GMT  
		Size: 14.4 MB (14408059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:f5a34d8ab975bf7eebbe916c037772cfa8f37fecfdb6f3b3abf9a9655167acd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73698911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff6c187f076ae1ece6644f6ba82870df16185cb36df7fb6ace38b07fc63b1c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:27:44 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 11:27:44 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:59:42 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:59:43 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:59:43 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:59:43 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:59:44 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 20:03:44 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 20:03:44 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 20:03:46 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 21:15:46 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 21:15:47 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 21:15:47 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 21:15:48 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 21:16:13 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 21:16:19 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 21:16:21 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 21:16:21 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 21:16:22 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 21:16:22 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 21:16:22 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 21:16:23 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 21:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 21:16:24 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 21:16:24 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 21:16:48 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 21:16:49 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5264b23495a17e4420ca5b0e5ab4505c64f53a3211fd7cf1a229bc32f032100`  
		Last Modified: Tue, 05 Apr 2022 11:37:01 GMT  
		Size: 1.0 MB (1010018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb184200e48b6e85a9e4c02b4c4ce45bf0f2d0f721f517ad6c07e6caf8d61f9`  
		Last Modified: Tue, 03 May 2022 20:09:02 GMT  
		Size: 38.5 MB (38477492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fa947c546f66e72fa231af6f3467a031df7c7a2e0efa7103c2d41327f8b719`  
		Last Modified: Tue, 03 May 2022 20:08:42 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b48e13a6bfe2457d10b6c1a9dcb57a81809ebfc7cba3a5202042cf41024cd4e`  
		Last Modified: Fri, 20 May 2022 21:20:47 GMT  
		Size: 16.9 MB (16851634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ea6641b2440f004d8d1a4a140d9e82f8673c6030116083da4b045b93be0996`  
		Last Modified: Fri, 20 May 2022 21:20:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dec61a5efa0323a168523e48df01248897fd66cde23e6aefeb636fcd044607`  
		Last Modified: Fri, 20 May 2022 21:20:40 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9664fa65a933a46aab92ae40a7657d5934319c1d6b7a9a40a4a819bb6f114f0`  
		Last Modified: Fri, 20 May 2022 21:20:40 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cc624d09655ce592a8ba493e0a0096ac4850ef516008bfef6b7d68b348518c`  
		Last Modified: Fri, 20 May 2022 21:20:40 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f132b0acc7e173bcbd9dcd9f6eb9cfbafa387954dabe5a646635e18bef4df02b`  
		Last Modified: Fri, 20 May 2022 21:21:18 GMT  
		Size: 14.7 MB (14734588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:84b88aea38415aa483fea474ee149e902653b6b099750fc039a1d8d7e0d0dd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72626464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b7c6e1ec02f59a0c5e778a6a9755fdf3a393e8aea202729e12cdd26e1cfc0c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:24:54 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 15:24:54 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:34:07 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:34:08 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:34:08 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:34:09 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:34:09 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:38:00 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:38:00 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:38:02 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 22:01:57 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 22:01:57 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 22:01:58 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 22:01:58 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 22:02:15 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 22:02:19 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 22:02:21 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 22:02:21 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 22:02:22 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 22:02:22 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 22:02:22 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 22:02:23 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 22:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 22:02:24 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 22:02:24 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 22:02:47 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 22:02:48 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f12bec611c705995fc5e1af1dad48d843a7b287a450059fa091c961029f77d`  
		Last Modified: Tue, 05 Apr 2022 15:35:04 GMT  
		Size: 921.8 KB (921830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7f4d123b5dead7e6c28e18c34dcb789e2b57b1aa053a18a03321ce79e3e9a4`  
		Last Modified: Tue, 03 May 2022 19:48:23 GMT  
		Size: 38.1 MB (38068980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4c57500473d960cf56c439a3ac25b8796d25c14cf6a99515cabc367fc0936`  
		Last Modified: Tue, 03 May 2022 19:48:05 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebbe4d5ac3603bddf2c8d45782fa7d3b383fc0aa6da003446671c8e26c0e5f7`  
		Last Modified: Fri, 20 May 2022 22:11:46 GMT  
		Size: 16.9 MB (16851577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc6f0356f9e9e94861a7674b899e252ed1cf4fc5f5191ac5906a6a1d3787c19`  
		Last Modified: Fri, 20 May 2022 22:11:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e449b12cce5eb7de34afde3f991c28ca2bbaab73bc7cc44c444eac6f28e2bc8`  
		Last Modified: Fri, 20 May 2022 22:11:39 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59bb252e872826890a4ec918fa3d30d94da06e1961cf90490c5005138a41e6f`  
		Last Modified: Fri, 20 May 2022 22:11:40 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d466f64bcbd25032629f783f3af30f68862e82484793239c8f3965406ebb32`  
		Last Modified: Fri, 20 May 2022 22:11:39 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471920e119cd1944ed659c5903ef6f0202cbc5fb8767812bd48a3030d04bb06`  
		Last Modified: Fri, 20 May 2022 22:12:17 GMT  
		Size: 14.4 MB (14356540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:16d513cdeefe27eaa641b036e2cfa7221a596c0efc53afffdeb53e8c2ef8cf72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75064613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb055d894367063106e5a901312837d88d8ee517b6c2c5dd581a0a839c3e947`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:45:47 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 06:45:48 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:47:23 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:47:24 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:47:25 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:47:26 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:47:27 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:49:51 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:49:51 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:49:52 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 21:24:37 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 21:24:38 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 21:24:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 21:24:40 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 21:24:49 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 21:24:51 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 21:24:52 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 21:24:53 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 21:24:54 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 21:24:55 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 21:24:57 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 21:24:58 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 21:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 21:24:59 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 21:25:00 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 21:25:12 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 21:25:12 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba95a793ebb86c33635e227617b480257f702f4fd72df8c6eae2f8fb2981f1e7`  
		Last Modified: Tue, 05 Apr 2022 06:51:42 GMT  
		Size: 1.1 MB (1079997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ea4d21ffea0c074e6bfbfc3690ec6e6fc9729cd15baa6572d5e717c0a8e694`  
		Last Modified: Tue, 03 May 2022 19:55:27 GMT  
		Size: 39.3 MB (39348212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acefa04ee6f39a7a2e9bf9b3bdf52b2b2d1f1cec279c8f6d3964e7584c49243a`  
		Last Modified: Tue, 03 May 2022 19:55:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6d3a29936ef6222652e68f1f5a91a85559502c9640c3f65a8fffe887eb0fe8`  
		Last Modified: Fri, 20 May 2022 21:30:29 GMT  
		Size: 16.9 MB (16851290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016ce73c9a602a0c11f4c8f7c7bb941fb410be2cfd77c185fe0b1392cf742e5`  
		Last Modified: Fri, 20 May 2022 21:30:27 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fce3c28e01e0b6f54711cff35966a6d164066b87087ad1721df05bdcf1ab2eb`  
		Last Modified: Fri, 20 May 2022 21:30:27 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc6a8b00b7c54f9ba881886fbad2d239209807a2c1b3f144abac021fbbb89f`  
		Last Modified: Fri, 20 May 2022 21:30:27 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983f5f7233435c39df011d09cbf59ad6ff5880c8c30fbf4b392723c68d49b64c`  
		Last Modified: Fri, 20 May 2022 21:30:27 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923faf8f83a310c24945ce4e0c3d55f17612391fb58c9f0f013ff86f27a96242`  
		Last Modified: Fri, 20 May 2022 21:30:49 GMT  
		Size: 15.1 MB (15065494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:2085d779b0de970321565ebb403c2cb8e58cc16ad4f2e623abd767b2b03ad089
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75530049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1e5dd0c764ae2aaf22537f5e309916075c3cc7b75210d8582e300b80b0c979`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:27:53 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 06:27:54 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:43:07 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:43:08 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:43:09 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:43:10 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:43:11 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:45:37 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:45:37 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:45:38 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 20:56:34 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 20:56:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 20:56:36 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 20:56:37 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 20:56:46 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 20:56:47 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 20:56:48 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 20:56:49 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 20:56:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 20:56:51 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 20:56:53 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 20:56:54 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 20:56:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 20:56:55 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 20:56:56 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 20:57:08 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 20:57:08 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0dc27fe624a22d1cb8dace34b1b0be387746e3ffbee03e2cc7753f8909d735`  
		Last Modified: Tue, 05 Apr 2022 06:33:04 GMT  
		Size: 1.1 MB (1109053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a005784549e7c151b02f7144cc20deaf6caf4d541b62ed180a89452c3013a34`  
		Last Modified: Tue, 03 May 2022 19:48:21 GMT  
		Size: 39.7 MB (39653779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924289a2acbbcf190a3ae4872ebfea556dd286ff69a61396cd000fa018b1120`  
		Last Modified: Tue, 03 May 2022 19:48:16 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbe679cf371b660e2d8429f4de00bbd5d51a9a48812f3986b263b186a78fd1a`  
		Last Modified: Fri, 20 May 2022 20:59:06 GMT  
		Size: 16.9 MB (16851276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefac3ddff1bf63205ab19f1c6e10f9bc7adeecf7a80c978923cbf46a9cd1e9e`  
		Last Modified: Fri, 20 May 2022 20:59:04 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5755613031cccf80f52a2020e206b1f02ba04e2eeedf47a31dbc53cd603180ca`  
		Last Modified: Fri, 20 May 2022 20:59:04 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f77cce83b1f47d2a9b367fe02d1cb92271e1f5452c7190da9c000164b9249d`  
		Last Modified: Fri, 20 May 2022 20:59:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c6ba289e12e60e22ff235783f815522f6bd21a3b80565475cbd3067411f73a`  
		Last Modified: Fri, 20 May 2022 20:59:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07895d1ef5b8dfa44edc31300a4ce2db108e64f099c21cba544c477af7a530`  
		Last Modified: Fri, 20 May 2022 20:59:27 GMT  
		Size: 15.1 MB (15093829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:e2dc3e941711c1f510bff8f411b79ef613a2fec67b2315619d85b329b28fdc4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76143505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c9fa9ab0cc10e123e8a375a590061265ed440d0c4575ce722ffa2963ce3887`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:13:47 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 19:13:51 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:47:02 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:47:08 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:47:13 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:47:17 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:47:21 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:51:16 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:51:23 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:51:39 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 22:46:20 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 22:46:22 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 22:46:24 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 22:46:27 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 22:46:56 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 22:47:11 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 22:47:23 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 22:47:26 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 22:47:29 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 22:47:34 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 22:47:36 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 22:47:37 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 22:47:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 22:47:44 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 22:47:48 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 22:48:15 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 22:48:23 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c66855ccac46a2305763411fdbb3608cd838d728da7e78221ef028bbc5992c`  
		Last Modified: Tue, 05 Apr 2022 19:27:15 GMT  
		Size: 1.2 MB (1174884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f1399a80c3aa6783e037023027b4174dfeca7209b059a1ef5d9d73ef4162e`  
		Last Modified: Tue, 03 May 2022 20:14:18 GMT  
		Size: 40.1 MB (40145468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4224b479185ebf731f055f1e1593487f63ffc24a7546e206de5e8081576172`  
		Last Modified: Tue, 03 May 2022 20:14:11 GMT  
		Size: 1.5 KB (1495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53671cc69fce217d1844d810d9e6745950d4a51c38501831764d70e0668f8fa`  
		Last Modified: Fri, 20 May 2022 23:04:22 GMT  
		Size: 16.9 MB (16851628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c899921982e4b12a9df4ab36a2503a5612b1eecb0ffd290ac916d05bddd6c4`  
		Last Modified: Fri, 20 May 2022 23:04:20 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea26f8453427d7e5723f6fa229d9e0b230ea6bb460fd7145d5a784cc2a7bfc62`  
		Last Modified: Fri, 20 May 2022 23:04:20 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec37a6a88bb922e13cc8af5921890affb02a8730eb6e78954db5e1d4ca62cce5`  
		Last Modified: Fri, 20 May 2022 23:04:20 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57417b65d1c1a08201c79b2d434fbbcd4d43e3451fb96e683a6069a9fc3a56c`  
		Last Modified: Fri, 20 May 2022 23:04:20 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f502ffa50f198401619f6ce334d80448da2ffa2cf42182468dfe21a702841b0`  
		Last Modified: Fri, 20 May 2022 23:04:46 GMT  
		Size: 15.2 MB (15157120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:e1d466149f7f30c6ce45c01914fc48d6838ed53b1294cc6b9c25fa779b3713ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74484858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad01b0944082c1e6283064c3b21b639f3dff23bc2eb81ef0f77dcf118107b13a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:23:53 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 05 Apr 2022 11:23:53 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Tue, 03 May 2022 19:49:50 GMT
ENV OPENSSL_VERSION=1.1.1o
# Tue, 03 May 2022 19:49:50 GMT
ENV OPENSSL_SOURCE_SHA256=9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f
# Tue, 03 May 2022 19:49:50 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 03 May 2022 19:49:50 GMT
ENV OTP_VERSION=24.3.4
# Tue, 03 May 2022 19:49:51 GMT
ENV OTP_SOURCE_SHA256=76fcca5ba6f11eb9caac32bf053badc46b5d66f867150eef077f4f0d7944ecd7
# Tue, 03 May 2022 19:53:17 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 03 May 2022 19:53:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 May 2022 19:53:20 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 20 May 2022 21:22:30 GMT
ENV RABBITMQ_VERSION=3.10.2
# Fri, 20 May 2022 21:22:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 20 May 2022 21:22:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 20 May 2022 21:22:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 May 2022 21:22:48 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 20 May 2022 21:22:51 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 20 May 2022 21:22:52 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 20 May 2022 21:22:53 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 20 May 2022 21:22:53 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 20 May 2022 21:22:53 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 20 May 2022 21:22:54 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 20 May 2022 21:22:54 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 20 May 2022 21:22:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 21:22:55 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 20 May 2022 21:22:55 GMT
CMD ["rabbitmq-server"]
# Fri, 20 May 2022 21:23:08 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 20 May 2022 21:23:10 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23964259f35ee3486444d0e1c7f98eefa83bb319fe6597c0596b65c3041d0d90`  
		Last Modified: Tue, 05 Apr 2022 11:29:21 GMT  
		Size: 1.1 MB (1100601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f725d6a2ff441382a2651c71b4f646c78ce81fd1d73797b1b741cffc34ab42c8`  
		Last Modified: Tue, 03 May 2022 19:57:53 GMT  
		Size: 38.9 MB (38860100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98dedb94baca8f95e426ecc0e2763b8d82eb896119b53965a587557dfcf2e8f`  
		Last Modified: Tue, 03 May 2022 19:57:48 GMT  
		Size: 1.5 KB (1488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffef4d894ab8285999a6078f4243d538815339f7aa1cd985b880685335d37e8f`  
		Last Modified: Fri, 20 May 2022 21:28:40 GMT  
		Size: 16.9 MB (16851684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0600a6cb22ea6047fade757f81678fdc54ac1769d83091f62996561668648988`  
		Last Modified: Fri, 20 May 2022 21:28:39 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150660cf7c252e1fd1adf603877a8e1bc2644a33487072b9174a82d6c35a2097`  
		Last Modified: Fri, 20 May 2022 21:28:39 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f441aaffb3725583fc7872ba78c475fbe261ab13d66ff867de144e4c481a99`  
		Last Modified: Fri, 20 May 2022 21:28:39 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b7ff4af71bea30702124f3293193244dc68fc04ecf0a04b3281949fdbd03c6`  
		Last Modified: Fri, 20 May 2022 21:28:39 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ae301bbcc90b96a4bcbf45d40861222b36dff027d2a77f96d2e2d589864840`  
		Last Modified: Fri, 20 May 2022 21:28:53 GMT  
		Size: 15.1 MB (15068888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
