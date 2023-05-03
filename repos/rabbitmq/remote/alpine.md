## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:de56847256476947f85b417b8020a9bcff6d3b33dac89d9f2f47197931a789f9
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
$ docker pull rabbitmq@sha256:75329d91dc36b58729ee5ffa7c0bdd249494f9622870a0eedd14cd0b3c3d9fb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73047079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51dee2c24ba20c1089a4341627747201853813c1d4ae5a1a3fa5571a5a933337`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ce63b53ed6e70ac016efb871bb7a71ddeed533285a72b19a0d3fb66a8660c`  
		Last Modified: Wed, 29 Mar 2023 23:51:52 GMT  
		Size: 427.1 KB (427054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a191c506adac6587361ab0139ea8cca2602064adeaf9dc5b7a26b7ea6ab4be99`  
		Last Modified: Wed, 29 Mar 2023 23:51:52 GMT  
		Size: 10.1 KB (10136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756ef6d093ba051dfaa3539dacd047cd85e5b1e1d8fbc07e2af7416d99e16c7`  
		Last Modified: Thu, 27 Apr 2023 21:55:32 GMT  
		Size: 44.0 MB (43964932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befd9fd2573c5e8c5f6615ee4be1dc1217bdd6c52be5f28d6f2f8d961554fcb5`  
		Last Modified: Thu, 27 Apr 2023 21:55:28 GMT  
		Size: 2.3 MB (2325497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1222186221a46857dcdd19179544901e6875ccc8a2732f775f0249833bdc27`  
		Last Modified: Wed, 03 May 2023 11:17:45 GMT  
		Size: 22.9 MB (22943126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e89e9262bd13910639550af9f2fec80136690108bee82a2ef790172220df8b8`  
		Last Modified: Wed, 03 May 2023 11:17:44 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3135ecc2629c303ee8dc514b72a79900adacec1020996fcab08ecb8b3f6d35db`  
		Last Modified: Wed, 03 May 2023 11:17:44 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb5b9a9d279c12e85ba04ce79b76b285330cd96e08d3fa2cb04e3c03b301ebe`  
		Last Modified: Wed, 03 May 2023 11:17:44 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a0888571813b8dcde1085d379b996d50ae73e1fbcc82b4f1341bdbffc22f1`  
		Last Modified: Wed, 03 May 2023 11:17:44 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:5530b13873e582e799aad2012ff99902fe4bc1fcbadf08a0458bd6b2b5d25774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69260931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394c6f9a7c5855832dea1a6461a44330fe866194a36cdf8ee0444a7763cae066`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02294948b5b877efed88a32afdbb7b479057d79a674ecd4737b986a01abef26c`  
		Last Modified: Tue, 04 Apr 2023 00:39:37 GMT  
		Size: 404.5 KB (404536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52226f1ab0e5055ec2c9c3dda33d8820495a38b0b4a6a714f695d2b22039a59`  
		Last Modified: Tue, 04 Apr 2023 00:39:36 GMT  
		Size: 10.1 KB (10128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142d91117ebb095ce8fd649a558f673d1e5c8c81f180b8e0a78a4bf9a6358fc0`  
		Last Modified: Thu, 27 Apr 2023 21:56:29 GMT  
		Size: 41.3 MB (41335282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4177ad4c0700edd49cdf9b9545c12e01add04951d13afa635743d57915fcd9`  
		Last Modified: Thu, 27 Apr 2023 21:56:25 GMT  
		Size: 1.5 MB (1455643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac8e9aad77829bee8f6b462b00fe53ebecf3600b16c8e7e5ded325f3caf306b`  
		Last Modified: Wed, 03 May 2023 01:25:28 GMT  
		Size: 22.9 MB (22942758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f045404294b745dea50dcf7e89995abcfc0aeaadb472558f012d0c03b63992`  
		Last Modified: Wed, 03 May 2023 01:25:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cd54085d56258a3c8b760f3ab2c886e122732c3427e92ce2b9cd27c1fd7378`  
		Last Modified: Wed, 03 May 2023 01:25:25 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc908ae1d3caee131f52207992dffe11b15948de6e8f7b0bdb4b846428913e77`  
		Last Modified: Wed, 03 May 2023 01:25:25 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d16becd77e7836ce94a346d369eacee6e673e07fe838b6f07e50b93d89b22`  
		Last Modified: Wed, 03 May 2023 01:25:25 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:e49db990982db1a723b4618465fa124a7cfa6941a75187780b4f6d4b3618f284
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68338152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44fa3f0201a51814fcb8a35afa71ec30452d7b32a15b59faf6a0fdc0495106b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e24ee9844234d79c85a6cecd3937551a5bb1186343d4e0bc2a1a0fb47b3cf68`  
		Last Modified: Tue, 04 Apr 2023 02:11:13 GMT  
		Size: 386.0 KB (386003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d843c77ef63d65f612e263c75ff9cdf1fcb3d2d4b93320b3aa809774a7efda`  
		Last Modified: Tue, 04 Apr 2023 02:11:12 GMT  
		Size: 10.1 KB (10129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b991b428a5427d08183f9aa622dbfdc8966e5d8a4bdf9a6f70fbe977db18ca`  
		Last Modified: Thu, 27 Apr 2023 22:44:32 GMT  
		Size: 40.8 MB (40764754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e2c4e05514c16ea9ec864d1bad51029ffe60f50761519543e4aeb67013b75`  
		Last Modified: Thu, 27 Apr 2023 22:44:29 GMT  
		Size: 1.4 MB (1364472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff93770119572a5679fb5e7db45ed66491e03fb5d52aeade2bc4ecdb46d34a4`  
		Last Modified: Wed, 03 May 2023 14:40:37 GMT  
		Size: 22.9 MB (22942497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0afad9043e3608c4be732ac79065c484aec29ebeffd186d40002bf6b15b5b9`  
		Last Modified: Wed, 03 May 2023 14:40:36 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f7163bf63f73e77826db0bcf0a82c0d68c7a51f41bbd71ef471def2c8305f8`  
		Last Modified: Wed, 03 May 2023 14:40:35 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baff01bf7bbaed10f43ebf4ad56fb90087b90f3c8e1375f493539fb37211e7b`  
		Last Modified: Wed, 03 May 2023 14:40:35 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bf432d014c834603630143bdd41f906bb20df0d062ecc681cb4846d89894f`  
		Last Modified: Wed, 03 May 2023 14:40:35 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:3f23088726b7f2006e9f12090ce3af4ba44bc1b882124a3851a60cb5bc32132c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76824501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b579876824dd514954b0531665fd7ba1640752dd7ec13d34fb5b34a300475e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca68ddbeb56228c338c16f4936342fc3ef6f99e13de1eafb38bdb5cff47973d`  
		Last Modified: Thu, 30 Mar 2023 00:20:34 GMT  
		Size: 406.3 KB (406251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f70c1ad2290b54d06a12a4f370ef5ca1c7b07ea552329bac81f010916bf331`  
		Last Modified: Thu, 30 Mar 2023 00:20:34 GMT  
		Size: 10.1 KB (10134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d2f19aa100f31c917cc33630d95bbbfabb424f0a3c59644ec1c415c414ae62`  
		Last Modified: Thu, 27 Apr 2023 22:12:52 GMT  
		Size: 47.8 MB (47822875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44119cb0239c5aa54c008417760fa5d62ce2343a41462a1b3d9795201bb47345`  
		Last Modified: Thu, 27 Apr 2023 22:12:49 GMT  
		Size: 2.4 MB (2378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fe481c4c1d928f5583b31ff72f4768fb73bbcb7198ed67952c1509f4ef018`  
		Last Modified: Wed, 03 May 2023 10:22:04 GMT  
		Size: 22.9 MB (22943088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e31b22dce4ea370b5aa492aaed148a6fceaba3c57811ee630835f90ddd8949`  
		Last Modified: Wed, 03 May 2023 10:22:02 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abab3ab1a6cb400b7dc91de316ba44e961981d30161195d334f7f14178a6cd3d`  
		Last Modified: Wed, 03 May 2023 10:22:02 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629a0634a91364a5cefbe643eee5d282046513aa32a47e38f9fd413b1816e914`  
		Last Modified: Wed, 03 May 2023 10:22:02 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b914735f7c8a95c21d9b09e7c91437ffac3e582d298f16d8e3cc69925cb188a7`  
		Last Modified: Wed, 03 May 2023 10:22:02 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:a3dbba03f6a0ca2b841fd19263b98700f9ea5f3f99d05788df93bf2b0a392c19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71414558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4557b33596474d9d43dba86f95e6e99cccab4865ef3876f544b7806086d7b9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ef2c43ba530d62fc506b832d99f4cd1bc8d8ce5f6592bb7fa936c90bbcb34`  
		Last Modified: Thu, 30 Mar 2023 01:01:32 GMT  
		Size: 442.2 KB (442230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee587207ab12c6e9cc5f061dd015e65f5cada7b34de8c3c0257d747a34a4bf7`  
		Last Modified: Thu, 30 Mar 2023 01:01:32 GMT  
		Size: 10.1 KB (10134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb9b892241935211be3070bca941cdfb1860da57dc34956f8ca35b30d46dd69`  
		Last Modified: Thu, 27 Apr 2023 22:22:03 GMT  
		Size: 43.1 MB (43109440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa83ab36b0456f612caa9420f3a528ec823cf0e8a2b39a7d1d5e8d6c170508b9`  
		Last Modified: Thu, 27 Apr 2023 22:21:57 GMT  
		Size: 1.5 MB (1495933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a67750c3416331fead212347556cad58cd2ad8ba89c02852b0d3de785f24cf`  
		Last Modified: Wed, 03 May 2023 12:42:41 GMT  
		Size: 22.9 MB (22942783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544dad8e3b3ab29749c5391c6112bad95b02ee6d9b2d8543ef9a682dc3f83e42`  
		Last Modified: Wed, 03 May 2023 12:42:38 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4508dfb171e9f230691abd039b36b2c0db062244555d5708f352b7be53d57fc9`  
		Last Modified: Wed, 03 May 2023 12:42:39 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491323a4d14a4e1c90bf3f72183f95acba243a0b48185306ebca9d77d7677006`  
		Last Modified: Wed, 03 May 2023 12:42:39 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb683cd81ea147db0418138b0b856ef46972c2bc981a075f055427373d4e11`  
		Last Modified: Wed, 03 May 2023 12:42:38 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:17763e10c0a976eed25a9b12101e55f66d2a0d883ac93f56ddb98ae5bd78c75e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72354719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4950049921a205e3287cf08eb29f6e9f2ebe166b45965fcb3fb843c3ef50ce4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518a33b8b4be6660c86c1d4872eed5464417829ad1231f64e3bcf9d87124bb`  
		Last Modified: Thu, 30 Mar 2023 05:43:06 GMT  
		Size: 470.5 KB (470475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3300e76b5534f5bd6ea1010b26d1f4189cb90164e8874b7deebeb42d136a93e2`  
		Last Modified: Thu, 30 Mar 2023 05:43:05 GMT  
		Size: 10.1 KB (10134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d858a6d012830d2135496a4a008484f23e4e8313ebb933af047d509c23bf91`  
		Last Modified: Thu, 27 Apr 2023 22:12:37 GMT  
		Size: 44.0 MB (43983880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04260607313478bd05e12d5e68d06efc1425cf3644d20ac03e7441e8e730c93e`  
		Last Modified: Thu, 27 Apr 2023 22:12:30 GMT  
		Size: 1.6 MB (1554729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156168c025e75e6ebda7d4c731f6509f42fcfc4a185cd1f71c5afbfeeae6a137`  
		Last Modified: Wed, 03 May 2023 16:59:12 GMT  
		Size: 22.9 MB (22942788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc64bbe6ab77f06b29fd7d840a98c0967bff1164fccd400b7db3b1abe0292c5`  
		Last Modified: Wed, 03 May 2023 16:59:09 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca6f55f8c02e1e14b098fb4a2fe4c26b68e1848f8b6a7b3e846d3ea280c83c4`  
		Last Modified: Wed, 03 May 2023 16:59:09 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9d6847db771aa07b78689ae288cd966b2fb7d2e88f8fb094faff286e4fd788`  
		Last Modified: Wed, 03 May 2023 16:59:09 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cab05b2318e0ac0d1f5a0505f56eedce273afe63e1db93a7a4bad6e4b8ec2fe`  
		Last Modified: Wed, 03 May 2023 16:59:09 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:08ff2a71340cb41366aee6456534d2532cc023b55b3fdb8a0cc85d4867351335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63852113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225195edc41bcd1eac990a4c35a378d0f07238cb7c2b4892b262463d6261d64e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_VERSION=3.11.15
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 29 Apr 2023 17:16:35 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Apr 2023 17:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 29 Apr 2023 17:16:35 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 29 Apr 2023 17:16:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 29 Apr 2023 17:16:35 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 29 Apr 2023 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 29 Apr 2023 17:16:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 29 Apr 2023 17:16:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334fc5c11099c92efe8c4b82ba9ef33007ca200400ca14a32bb61d39961fa1a6`  
		Last Modified: Wed, 29 Mar 2023 22:03:57 GMT  
		Size: 425.2 KB (425170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bf2ac7d88975211cf172ac3df90f59ad5b2a20512c70f5a6763882605ac382`  
		Last Modified: Wed, 29 Mar 2023 22:03:57 GMT  
		Size: 10.1 KB (10140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5995137e0db12767d7479cea2eb3a390e6f293e38804f4916ad893f71e5e4930`  
		Last Modified: Thu, 27 Apr 2023 22:15:53 GMT  
		Size: 35.8 MB (35810820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc323ebde3c0f70a2e7fa00f7c5507d5676764c88d5bac2489b8ab93cc207152`  
		Last Modified: Thu, 27 Apr 2023 22:15:50 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7bdf7f4171ae492acecc9fe771f3d2137ea496ba2ee53609b99a1128118b73`  
		Last Modified: Wed, 03 May 2023 14:05:45 GMT  
		Size: 22.9 MB (22942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a47e56b60e5ce43ae07a2ed71af06a648fc717e0a9ed84a2ad52ebed14c420`  
		Last Modified: Wed, 03 May 2023 14:05:43 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d1ce6dcada356174bd881e72f763eb643beb740657a1c46db924885d8c7b64`  
		Last Modified: Wed, 03 May 2023 14:05:43 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4e06b9c0237c43aabef04754a80a0a8615b01b12cd7fb13af8c0b91f73c5b`  
		Last Modified: Wed, 03 May 2023 14:05:43 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015178ff20c32561353177d604a2bb061c0199a88dca038dec3bcc97424375fb`  
		Last Modified: Wed, 03 May 2023 14:05:43 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
