## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:eb9b4b49d8504df790e8593bce89a40c03752d3b9413f2332f3d892a5ec54cd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:5cca7b7eb43dba0e0141ba057d9c0ebf5bc6aeff2cd6bf281e48cb8db677ae41
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62864824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cbe0e673886c535e572b9490e313b4ecfb8cc05c41d686495febf4cd3d1c85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:25:19 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 20:25:20 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 20:25:20 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 20:25:20 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 20:25:20 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 20:25:21 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 20:25:21 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 20:40:26 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 20:40:26 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:40:27 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 20:40:28 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 20:40:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 20:40:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 20:40:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 20:40:43 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 20:40:44 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 20:40:45 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:40:45 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 20:40:45 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 20:40:45 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 20:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 20:40:46 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 20:40:46 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 20:41:02 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 20:41:09 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 20:41:09 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c804563f19d596d7637dea8548081b2312d725ecaa8074b1c435d7a2c9f61e27`  
		Last Modified: Tue, 24 Dec 2019 20:42:40 GMT  
		Size: 1.4 MB (1431588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e7d481c55e5da940b402efb845918bb65080c5e8e21bdc733758a7c3ea60bd`  
		Last Modified: Tue, 24 Dec 2019 20:42:47 GMT  
		Size: 35.6 MB (35602291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d20bd6cd4eee79ae8b820804e07c7095df5e79bda8908930caa715f5ff8637`  
		Last Modified: Tue, 24 Dec 2019 20:42:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a78cfffc19423467f87fa463fc9f016368d0b63427bac15bb6179cbc9a3792`  
		Last Modified: Tue, 24 Dec 2019 20:42:40 GMT  
		Size: 12.0 MB (12036924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d55998d7f44d383a6760f90b5c240189cadea5bf1d1351d589937f5c771f9bb`  
		Last Modified: Tue, 24 Dec 2019 20:42:38 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a3108b2f9b5d39890ed1e58f50c4f4984bef3f9bb335e69dd860a278135db`  
		Last Modified: Tue, 24 Dec 2019 20:42:38 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644bb250bfe3a59dcbeff1122cc7d8c87c34e36c4d658a33965d0654d2d3e36`  
		Last Modified: Tue, 24 Dec 2019 20:42:54 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d8f47a837200c27eec196551bb507afd7ae6583cbcd34371095b506912b8be`  
		Last Modified: Tue, 24 Dec 2019 20:42:56 GMT  
		Size: 11.0 MB (10986147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:423a7db83fc5294bd157944585dd57f732d8af6c877e4cf0883cec798e15b3d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61630930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b817663d9dc7adacaf00a3b3493f0df43f19ed4b95776de3104b72c50ecf7c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 19:22:38 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 19:22:39 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 19:22:39 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 19:22:40 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 19:22:41 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 19:22:41 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 19:22:42 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 20:02:52 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 20:02:54 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:02:56 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 20:02:57 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 20:02:58 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 20:03:00 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 20:03:02 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 20:03:24 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 20:03:27 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 20:03:27 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:03:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 20:03:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 20:03:29 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 20:03:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 20:03:31 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 20:03:31 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 20:03:53 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 20:04:02 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 20:04:03 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645e6532e1df84d7aea290d9bafa99f9536a03106b0ff296fad9cb5c6f4dfc`  
		Last Modified: Tue, 24 Dec 2019 20:05:26 GMT  
		Size: 1.4 MB (1382699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c954e6d3506f343540507851b1e1ef7164d0ccfec2185efedd6cd00360471b5`  
		Last Modified: Tue, 24 Dec 2019 20:05:35 GMT  
		Size: 34.7 MB (34689118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cc78d1051441473705ad02402d68937151bb81969d2b8e046e4ed833c827f2`  
		Last Modified: Tue, 24 Dec 2019 20:05:23 GMT  
		Size: 1.5 KB (1455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de2ab69ad945c0b60faa9a5ccf25e527a1a953468f062cd76399e0b35b679e8`  
		Last Modified: Tue, 24 Dec 2019 20:05:25 GMT  
		Size: 12.0 MB (12036081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b3a71b61073138082b320d24f5a5ed064828b1ad41d88bc51b555f55a32fe`  
		Last Modified: Tue, 24 Dec 2019 20:05:23 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a672ae4de1f481fe1a110afa1b1c919b6bf4a3487604cd8443dac847298f4683`  
		Last Modified: Tue, 24 Dec 2019 20:05:23 GMT  
		Size: 4.4 KB (4414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4b2186b252c690b690232761236ac754a959193e10f90664a59ce3045650cc`  
		Last Modified: Tue, 24 Dec 2019 20:05:46 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c7b29a9e030b88262420a667872068625011589e7446ba355425acd7b2964a`  
		Last Modified: Tue, 24 Dec 2019 20:05:50 GMT  
		Size: 10.9 MB (10904843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:2c31818dca7e6a14e06a756280724de48e218fc2484804caed27de2da1859741
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.7 MB (60738514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55514c4616c62c72a47a00e354af148f01a959cc36cf34283576615b1832b3c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:25:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 20:25:37 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 20:25:38 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 20:25:39 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 20:25:40 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 20:25:41 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 20:25:42 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 20:30:27 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 20:30:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:30:37 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 20:30:40 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 20:30:43 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 20:30:45 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 20:30:45 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 20:30:57 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 20:30:59 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 20:31:00 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:31:01 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 20:31:02 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 20:31:02 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 20:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 20:31:04 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 20:31:05 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 20:31:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 20:31:43 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 20:31:48 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ba45d57f8e9c9d8f3de6ac0e2987448879106c39cdac602ea7826dd5b41c7`  
		Last Modified: Tue, 24 Dec 2019 20:33:34 GMT  
		Size: 1.3 MB (1300778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb806ccb11bc8c0c2536440990ef827a993fdd481ffcc1765ba908c1dad0e8b`  
		Last Modified: Tue, 24 Dec 2019 20:33:38 GMT  
		Size: 34.3 MB (34304190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dbbbc6642fb902407f22cba75ab2b86cd6d14aae79f34fa9a2f85be2c69b9f`  
		Last Modified: Tue, 24 Dec 2019 20:33:31 GMT  
		Size: 1.5 KB (1453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59286753365158890a767a8f4d8fa5f6ac873c861e9990fef3348cba40b0e0d7`  
		Last Modified: Tue, 24 Dec 2019 20:33:31 GMT  
		Size: 12.0 MB (12036048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641bb4fd357a40a54e09f2c018d5e28510d07986437bf78a9aedab3a7fdd0ecc`  
		Last Modified: Tue, 24 Dec 2019 20:33:32 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5ab074b10bd9e98d1bc225a92aec1bdc772c25f02bb446c33ba20da8eeeaf5`  
		Last Modified: Tue, 24 Dec 2019 20:33:31 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f0e0a2b9d7c25b21ea32c2fddf255d3978b00b309ba7ef8c8cc98f84c3f4bc`  
		Last Modified: Tue, 24 Dec 2019 20:33:48 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8a189a1832310c0e3661cd9744e107acee73c8a9faa27c2ef8be65538ba370`  
		Last Modified: Tue, 24 Dec 2019 20:33:53 GMT  
		Size: 10.7 MB (10674640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:45cd142d467e7f76afb0633465b5a81fd770d654020326c5d7a618b07f1f3850
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62551424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2f394e89a141acad5c90aa790cc5ec83562100e50d408cc768396b3b195cf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 21:15:33 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 21:15:34 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 21:15:35 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 21:15:35 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 21:15:36 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 21:15:36 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 21:15:37 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 21:19:32 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 21:19:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 21:19:39 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 21:19:39 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 21:19:40 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 21:19:41 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 21:19:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 21:19:56 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 21:19:59 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 21:19:59 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 21:20:00 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 21:20:01 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 21:20:02 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 21:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 21:20:03 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 21:20:03 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 21:20:23 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 21:20:31 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 21:20:32 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354409b8ee992e04c7ab1fdb3811b5b266b845ea477b748e3be0d31b5be94f3b`  
		Last Modified: Tue, 24 Dec 2019 21:21:53 GMT  
		Size: 1.5 MB (1462882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fb8054ab1b8171501355141f9929e2a9ff577c305a778c91540b3d94ad6d3`  
		Last Modified: Tue, 24 Dec 2019 21:21:59 GMT  
		Size: 35.3 MB (35261461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11643f211c8843ee1353b73eb067fe2b8db7e900ac30c625a6ad1fc5709f638`  
		Last Modified: Tue, 24 Dec 2019 21:21:51 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986345de8960f9bc822f0c56fa7b0bf55b38c10c60b82872ce93a692d5480759`  
		Last Modified: Tue, 24 Dec 2019 21:21:53 GMT  
		Size: 12.0 MB (12035942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6340c44a660eb8c869e231e4392cb3b565cd077f936e8f06c930a91779734116`  
		Last Modified: Tue, 24 Dec 2019 21:21:51 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aeefbbc7ccb2c98d3fcaa6e6a985c67d5a07f1fe900818589545cd5c8b5a2f`  
		Last Modified: Tue, 24 Dec 2019 21:21:51 GMT  
		Size: 4.4 KB (4414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c932c1595b22de3ec559d868763cfbd1b7ee2b4aebc104f266a65727a408ca75`  
		Last Modified: Tue, 24 Dec 2019 21:22:08 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65c8a5a539c0b804e646b96f0fb657ca82742dc236b4e7715569f7902ad367c`  
		Last Modified: Tue, 24 Dec 2019 21:22:12 GMT  
		Size: 11.1 MB (11065789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:0855d8944b1627021725e5c97f575b893daf324b1561e2203dd0c399ec89aa3c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63132030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948c3a18be2869a1144f06cd2c5592b71d15a2077e65cbfd74afe333b66cb10e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 22:43:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 22:43:39 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 22:43:40 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 22:43:40 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 22:43:40 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 22:43:40 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 22:43:40 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 22:53:01 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 22:53:01 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 22:53:02 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 22:53:02 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 22:53:02 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 22:53:02 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 22:53:02 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 22:53:11 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 22:53:12 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 22:53:12 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 22:53:13 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 22:53:13 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 22:53:13 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 22:53:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 22:53:13 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 22:53:14 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 22:53:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 22:53:35 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 22:53:35 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea01899649bb84896e33c74fc1266d2292ee2715655ba19a7024cfe6d2b035`  
		Last Modified: Tue, 24 Dec 2019 22:54:28 GMT  
		Size: 1.5 MB (1484033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c48ee59cba49e02616d65a27dad1b7a2e6ed57442d54e64481477ae5082641c`  
		Last Modified: Tue, 24 Dec 2019 22:54:33 GMT  
		Size: 35.7 MB (35696409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54831b9fe5bd448105696932f51d90fd6fa1631526a55dbb6fecf8e531ac7ea`  
		Last Modified: Tue, 24 Dec 2019 22:54:26 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8178a09a2526d8b732244946e5c185de646d10cbcfb9b22a2ff1301d92c7a9`  
		Last Modified: Tue, 24 Dec 2019 22:54:28 GMT  
		Size: 12.0 MB (12035550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baec51118feb551bb4a1ec150cb1b30dca8ef9799728b25113532b6e7d1cd2d`  
		Last Modified: Tue, 24 Dec 2019 22:54:26 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0796e598b77269b76f3fd36226e468f64da09a21809661a2b76f43fea0bbb1d6`  
		Last Modified: Tue, 24 Dec 2019 22:54:26 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9626b24fe50549f289db13b262423ddf073f7549fed37884ed1e65d19bcb618c`  
		Last Modified: Tue, 24 Dec 2019 22:54:38 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92103799b36d40bf391e96a12b658970c384c0e1b1e98184147b423dfabaadf1`  
		Last Modified: Tue, 24 Dec 2019 22:54:41 GMT  
		Size: 11.1 MB (11104797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:90c1dd36cdc9303379d012abbdab9acdcf5d45d6bedc2718a7e5ddfcc19bea7a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63591030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d237cd1d484297dce4357a7ec24bf13fbdbb3af1f17e0288f7b8ed2f48c36c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:42:00 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 20:42:04 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 20:42:09 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 20:42:14 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 20:42:17 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 20:42:22 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 20:42:26 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 20:56:54 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 20:57:03 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:57:16 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 20:57:24 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 20:57:33 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 20:57:44 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 20:57:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 20:58:43 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 20:59:04 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 20:59:14 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:59:23 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 20:59:29 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 20:59:32 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 20:59:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 20:59:40 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 20:59:45 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 21:00:29 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 21:00:53 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 21:01:01 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78be75180598caf1fc8cc604644e2b593c14ed569d5f5a0d0d80a2ddc70f4a68`  
		Last Modified: Tue, 24 Dec 2019 21:06:50 GMT  
		Size: 1.5 MB (1546994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc19e8dde1a21ae0b7ca13b93da6642bd9760f11cf2345f65ab221feef4b3c`  
		Last Modified: Tue, 24 Dec 2019 21:06:54 GMT  
		Size: 36.0 MB (35950879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa5a773506d460e672bd3c9eef33ab3ed0c470869ac4a01322755715872f328`  
		Last Modified: Tue, 24 Dec 2019 21:06:45 GMT  
		Size: 1.5 KB (1462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb2625f0a2953e5001a3c0859e3166d69b336108bc55ffe34cdd83cdcafd`  
		Last Modified: Tue, 24 Dec 2019 21:06:46 GMT  
		Size: 12.0 MB (12036723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f082b9998e5342ea4d68ef4cf9797a17e79350770aae515d987087884b2d49b9`  
		Last Modified: Tue, 24 Dec 2019 21:06:45 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97354455b4c185ae235fc88a618595cfc16450a25bebe67e1b2aadad66c363f2`  
		Last Modified: Tue, 24 Dec 2019 21:06:45 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83daa2616bfa361e9353513600cdfb5a5e7dbd2b2fd31e8d30fbfde6342ed685`  
		Last Modified: Tue, 24 Dec 2019 21:07:15 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54ff53b2785a6a6d317aed81a732c7a23859d9acebd259b948056b832421ccb`  
		Last Modified: Tue, 24 Dec 2019 21:07:20 GMT  
		Size: 11.2 MB (11233776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:aa99e525b46e0310c4b090c86b9204d74c6fa0307916502a5861e19f6e4c57f6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61874550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68cc7ee018b185469712eab7822fcfb502c6ba3638aecc0424f63539a5d285dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 24 Dec 2019 20:16:56 GMT
ADD file:d26fbcd308b78da175af74382b16ee1f7a3370ab9d618b306d604d292e72c560 in / 
# Tue, 24 Dec 2019 20:16:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:44:49 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps
# Tue, 24 Dec 2019 20:44:50 GMT
ARG PGP_KEYSERVER=ha.pool.sks-keyservers.net
# Tue, 24 Dec 2019 20:44:50 GMT
ENV OPENSSL_VERSION=1.1.1d
# Tue, 24 Dec 2019 20:44:50 GMT
ENV OPENSSL_SOURCE_SHA256=1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
# Tue, 24 Dec 2019 20:44:50 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Tue, 24 Dec 2019 20:44:50 GMT
ENV OTP_VERSION=22.2.1
# Tue, 24 Dec 2019 20:44:51 GMT
ENV OTP_SOURCE_SHA256=65ab58ce79181895afc66716cc735a0ada4a3b705a525407d7e1d4c5deb95e72
# Tue, 24 Dec 2019 20:47:59 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		ca-certificates 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/archive/OTP-$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-erl_interface 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Tue, 24 Dec 2019 20:48:00 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:48:00 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Tue, 24 Dec 2019 20:48:01 GMT
ENV RABBITMQ_VERSION=3.8.2
# Tue, 24 Dec 2019 20:48:01 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 24 Dec 2019 20:48:01 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 24 Dec 2019 20:48:01 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 24 Dec 2019 20:48:06 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Tue, 24 Dec 2019 20:48:06 GMT
# ARGS: PGP_KEYSERVER=ha.pool.sks-keyservers.net
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Tue, 24 Dec 2019 20:48:07 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 24 Dec 2019 20:48:07 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 24 Dec 2019 20:48:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 24 Dec 2019 20:48:07 GMT
COPY file:2cb4eee6ce39121e7f1de01e8683347296de40d81470fb3070423f105fe0c348 in /usr/local/bin/ 
# Tue, 24 Dec 2019 20:48:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Dec 2019 20:48:08 GMT
EXPOSE 25672 4369 5671 5672
# Tue, 24 Dec 2019 20:48:08 GMT
CMD ["rabbitmq-server"]
# Tue, 24 Dec 2019 20:48:23 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Tue, 24 Dec 2019 20:48:26 GMT
RUN set -eux; 	erl -noinput -eval ' 		{ ok, AdminBin } = zip:foldl(fun(FileInArchive, GetInfo, GetBin, Acc) -> 			case Acc of 				"" -> 					case lists:suffix("/rabbitmqadmin", FileInArchive) of 						true -> GetBin(); 						false -> Acc 					end; 				_ -> Acc 			end 		end, "", init:get_plain_arguments()), 		io:format("~s", [ AdminBin ]), 		init:stop(). 	' -- /plugins/rabbitmq_management-*.ez > /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python; 	rabbitmqadmin --version
# Tue, 24 Dec 2019 20:48:26 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:bca389ebb9be8103bf737251d68f962104771b2f9c1fff1f7ae0207458fa4c86`  
		Last Modified: Tue, 24 Dec 2019 20:17:18 GMT  
		Size: 2.6 MB (2579591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ba90fcdfe79f10a89975f46e887163933ac8eb2a40f8d5633457a5a9b0a37`  
		Last Modified: Tue, 24 Dec 2019 20:49:14 GMT  
		Size: 1.5 MB (1474203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d977f45e7948b5c7143d087d2ee946519c0fb37a55ae967096a7fb0300b5ef79`  
		Last Modified: Tue, 24 Dec 2019 20:49:17 GMT  
		Size: 34.7 MB (34692262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bd4d693d08f991007051d1596374f473a75e245c5360cac1e55efe54e97f0`  
		Last Modified: Tue, 24 Dec 2019 20:49:12 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408383329c96727ba0006b9f9ea85b1421fcbf81510bcbec4907cb3bb6f26ed6`  
		Last Modified: Tue, 24 Dec 2019 20:49:13 GMT  
		Size: 12.0 MB (12035424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2d044a8770866d6b55bab1411cd7d7bd5da842a94a79df04cbe811f69621fd`  
		Last Modified: Tue, 24 Dec 2019 20:49:12 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6898ea2163d1abef966f29691191a050514ad16a0f8ed2ff0c16559434bfba`  
		Last Modified: Tue, 24 Dec 2019 20:49:12 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6525324ca6e23123192e9b944f22cef078c0b8f4c0642af86846d9263c3775b6`  
		Last Modified: Tue, 24 Dec 2019 20:49:23 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e91db225582d2d15f626c26704ab29c6d5bb66a7efb3ff0565658a13da7a`  
		Last Modified: Tue, 24 Dec 2019 20:49:25 GMT  
		Size: 11.1 MB (11086974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
