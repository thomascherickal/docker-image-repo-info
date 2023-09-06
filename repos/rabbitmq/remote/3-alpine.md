## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:89bd42a2e4d2f76ea1026f7b8fb2f0020fb9fe484fe0326c12ae50444e451087
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `rabbitmq:3-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:2945e4d1c768487af77bdf1a46e87fb9e5ef242e637dea8eac3d63e69c8d41f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70997980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1094c81f35849c69b1bca2bffcdccc53d1e4384edead4e78a2ce7d7fd02504b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a5385fcc36c33c419077bb01c1e1b8f2302dfa0d5649c21df1cc7a8a457e860`  
		Last Modified: Wed, 06 Sep 2023 00:08:19 GMT  
		Size: 40.1 MB (40053046 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ce0b45764de69064430bf1c8e7363b9623d0a857e76be135788af9bd1a4a112`  
		Last Modified: Wed, 06 Sep 2023 00:08:18 GMT  
		Size: 7.5 MB (7543339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f80342b0598519d2622118d2055b07f05ae930e4a2c1add6beba7213849fb6bd`  
		Last Modified: Wed, 06 Sep 2023 00:08:18 GMT  
		Size: 2.3 MB (2297421 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:591a55830d55f0fa4e279e0ee4ad7320ec84e30c8b50956446b0f6c753413d0c`  
		Last Modified: Wed, 06 Sep 2023 00:08:18 GMT  
		Size: 17.7 MB (17700811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8a7e1778096388a64e31dce09b721125387e31cab491da2aa518e3d6d93e4de`  
		Last Modified: Wed, 06 Sep 2023 00:08:15 GMT  
		Size: 194.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:633a4b8b03ac8794fbc9855431f1eabda9887cf8eedb1399055f6ffc8c337067`  
		Last Modified: Wed, 06 Sep 2023 00:08:16 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c9dc74bd0572fef0deaf6e7efeda1554283636e0abbe6d59f6111729a1fbc9b`  
		Last Modified: Wed, 06 Sep 2023 00:08:20 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55d6487310c9c56f6d616e5dabf771320f000ab829a29d176108174be4b44007`  
		Last Modified: Wed, 06 Sep 2023 00:08:20 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:de3dc9463fc62904cbef9f1ac0bea0a2bbdcf54d4c355cc30abf2cb2ef5bef06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **763.1 KB (763069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b58f8be43556185ec4ea2e488f87c8c0083a0059d879d76371137ba1ed4cea`

```dockerfile
```

-	Layers:
	-	`sha256:531b71606133cbf39800c4107e463e4af920c22918271e31e80e2ca67d738bd6`  
		Last Modified: Wed, 06 Sep 2023 00:08:17 GMT  
		Size: 701.5 KB (701508 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a0e7066e86127eea92be402d6ae3bb4350cf02fc2f5081ca410c03e4b3e6e397`  
		Last Modified: Wed, 06 Sep 2023 00:08:17 GMT  
		Size: 61.6 KB (61561 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:cd89395b92699eb1691d20290d0125b602d2954f12e28baab33b493b591df238
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60996578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70ad931e59edad79a5f4b66c722f781cbeae773e442282cdf14a7602d47ffecd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee1536c6d5ae5014d6e8009b5893fd8b99f5d03e2b1586613ae8784eaf26354`  
		Last Modified: Tue, 05 Sep 2023 23:57:27 GMT  
		Size: 32.4 MB (32362191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b29922f46d4bca60eafdcaa6ea27a6721d32793512d1802757752383ae3afd`  
		Last Modified: Tue, 05 Sep 2023 23:57:25 GMT  
		Size: 6.4 MB (6374627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8d7348a1228bee886882208420db56a8394de980a77df42d69bf8c1927aac7`  
		Last Modified: Tue, 05 Sep 2023 23:57:24 GMT  
		Size: 1.4 MB (1412497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d59ed3d40176776728c5aec715d8d4ff860d83ab9bbbc7ca3674e23be3e1c9`  
		Last Modified: Tue, 05 Sep 2023 23:57:24 GMT  
		Size: 17.7 MB (17700697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9cb073fc918fe7ec1f51c7b9daa2785d35f750224cae9a48601aafb8e6879`  
		Last Modified: Tue, 05 Sep 2023 23:57:22 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11901e7317e6ee7cac4ef48b182e93763c1e736aa12479397ab236226e9e2fa`  
		Last Modified: Tue, 05 Sep 2023 23:57:22 GMT  
		Size: 109.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddafb430231a4a96c4d6896c8d7dfaae2905699f4dd549bd95ef97a84700a554`  
		Last Modified: Tue, 05 Sep 2023 23:57:22 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64fcba55ae8ec6111eb6938069b04cff8ade2f9705b32a29c79e27745d420f7`  
		Last Modified: Tue, 05 Sep 2023 23:57:22 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:08283f391ea38e5d7d005aa8b5bd1a2a15a513f505af33b71008890ccb5b1d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60230138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ff7b89826f64405ec44d70d221790e7dec4af336ddedbc9ff6afe0444dbd3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a1d118fe34bd11b09f71087ade8179adcf641f1b3330dfee02bb5a6810d418d`  
		Last Modified: Wed, 06 Sep 2023 02:36:26 GMT  
		Size: 32.2 MB (32249675 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79ec82a3c629e9d8d9f510102bf314c1803715eb9477dd8ebd2d68ef937e3154`  
		Last Modified: Wed, 06 Sep 2023 02:36:24 GMT  
		Size: 6.1 MB (6078152 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ee153bb1bc7220ee792ec588f51d153512fd99e78e5dac7e47fa478fd780019`  
		Last Modified: Wed, 06 Sep 2023 02:36:24 GMT  
		Size: 1.3 MB (1300436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d9ad6d8b2f4a91cde8039574bf63336b0e9ddb8346a94d26b919d61a2066336`  
		Last Modified: Wed, 06 Sep 2023 02:36:26 GMT  
		Size: 17.7 MB (17700647 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffab2ee38a3ba05aef04c89202ee57f9a43c2fffd36ac6b3c3e3518dbfa15bbf`  
		Last Modified: Wed, 06 Sep 2023 02:36:26 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:884c5b49b611f6fd42c1d7ebe80be398409740a07567bbcaa3a878cc3d541f6b`  
		Last Modified: Wed, 06 Sep 2023 02:36:26 GMT  
		Size: 106.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d37d00fcb8915668657519ed2f87a3001b71146475dd4ac4d63aa7be148ecb8`  
		Last Modified: Wed, 06 Sep 2023 02:36:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac99735a04bf871dc95b012d52e2265c0c2f92f7cbce7ce77f239cbf3d64306c`  
		Last Modified: Wed, 06 Sep 2023 02:36:28 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:3cea51bc07325d940a9de6d8a1eee8ccb598b8ff0742a90df448f58add048d81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.2 KB (759175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d1e78fec04adc177f864eea8a1d7520f65f10939ad51abe47dca57944c1891`

```dockerfile
```

-	Layers:
	-	`sha256:d29a72f9a6a96c807a82e5e28d5304b4af286c61247c77ce5a91ab9b5f724233`  
		Last Modified: Wed, 06 Sep 2023 02:36:24 GMT  
		Size: 697.4 KB (697426 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cb2b06c37478c72c3ed78c75e727ee2845bf3a22b0adf5b457671b31fe578ccf`  
		Last Modified: Wed, 06 Sep 2023 02:36:24 GMT  
		Size: 61.7 KB (61749 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:57c4b2b1b120a754d11feda9cc547e84c29982001c7d7d9b500b97d0f6f5240b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68396109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60a6f7812f65481c5f3b8d0ab3a9514ddef3ff33764923e14c877917a8a53f43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cea33bac8ee110735c004b6468f0acf7259ffcb2c21691286e2310d74bdebc50`  
		Last Modified: Wed, 06 Sep 2023 01:05:18 GMT  
		Size: 37.9 MB (37859969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc7b3cd3b7c294580e8f15ba0bf1552cbdbaf3c1cd0c8fa251289d7e4a223d89`  
		Last Modified: Wed, 06 Sep 2023 01:05:16 GMT  
		Size: 7.1 MB (7133991 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d1b35a70d737b702b5bdc4b3d15998c5e247bc1c82587acf45cf17457800d31`  
		Last Modified: Wed, 06 Sep 2023 01:05:16 GMT  
		Size: 2.4 MB (2368782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e62a501798f5e5acd7bc65399657998b99230ce68a66620e1968a5df1afdd3`  
		Last Modified: Wed, 06 Sep 2023 01:05:16 GMT  
		Size: 17.7 MB (17700853 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b7c4fa1dbd5e4f9279a817ade25978f636f85406394312259d2a49fde726be1`  
		Last Modified: Wed, 06 Sep 2023 01:05:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81e61c77e20e418caa890f5676cf97722e0cc7f4307708e46a347f3635f2c5c6`  
		Last Modified: Wed, 06 Sep 2023 01:05:17 GMT  
		Size: 108.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9cc5193ec06ba5dd83566404c83d67a6bb03014dde830ffa3ed757d42c63877e`  
		Last Modified: Wed, 06 Sep 2023 01:05:18 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8691bc3302004ec2807ad9fdd1be68924b6e9d9bb7e232f683ef53aebd958aca`  
		Last Modified: Wed, 06 Sep 2023 01:05:19 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:da8bb0849dcd7fc8eb48d86ea2c786097bda797e336e4bc864aec0fda72f42a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **763.1 KB (763102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84eca508d486e24745fa4936186f9c9618255c4c71436ba0edbf0f3bda7a6a2c`

```dockerfile
```

-	Layers:
	-	`sha256:93f9592d5fe0cf130a1441f82914fa731fa50cacedeea8a031bc31d0de07905c`  
		Last Modified: Wed, 06 Sep 2023 01:05:16 GMT  
		Size: 701.5 KB (701530 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c2c2834b37616a4f5e31406d18e0c33112d99e29572596578b009c4b41d7a090`  
		Last Modified: Wed, 06 Sep 2023 01:05:15 GMT  
		Size: 61.6 KB (61572 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:1caa8a56aff2572f63798a645189af0c2e7bca56f0c1cdd70abd00646b4b5f8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62376586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab330238f90b08c537cdc596572a945a7ec2017ab65c8c65feb2f651aa382f33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30e933032cd8c0f5792db9a3db41438d934274acb2a898d43ca4d5d767b84a96`  
		Last Modified: Wed, 06 Sep 2023 00:06:31 GMT  
		Size: 32.6 MB (32602202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9afd97e31d6f4088a4426bb354b7f1cf8fd80083882adbed94abae4cd7fa66b0`  
		Last Modified: Wed, 06 Sep 2023 00:06:30 GMT  
		Size: 7.4 MB (7435040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e50ceab4a96cca14edea2f0eacc1ca655ce517901c75b3fcac5e5eeaaa0bd3e1`  
		Last Modified: Wed, 06 Sep 2023 00:06:30 GMT  
		Size: 1.4 MB (1401810 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:317cae0f21e28c9d9da5b46c79ae1f6952ed00fce2af78fead6e94a0464b241b`  
		Last Modified: Wed, 06 Sep 2023 00:06:31 GMT  
		Size: 17.7 MB (17700645 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d32e0847cdb1afac3a460b67735e9b13ea1400c1d9ade44653ac1eca65521020`  
		Last Modified: Wed, 06 Sep 2023 00:06:31 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90ade2b24037642c92567c71f11962dc07f44f584996986b720398c8c41c4856`  
		Last Modified: Wed, 06 Sep 2023 00:06:32 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8331ac6e6ebdd345fa2e3ec3dd9df2597d61ace268202b425594453c867b1bd`  
		Last Modified: Wed, 06 Sep 2023 00:06:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5a5e7d725474b21c5c4643c00faab78dfa102f8de17f17f7905ff3d4f5d046b`  
		Last Modified: Wed, 06 Sep 2023 00:06:32 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:048e163848d30e90271c4db42203e96011327005de92ea8aa18c79bc080358b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 KB (61290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad07bdb2c3289ed80b7a624f9a06bc68c65a66a6ef6aa6bafdbcde9f9b97ac8`

```dockerfile
```

-	Layers:
	-	`sha256:3af18dfe07108ae37f6ed250099883a9df4763e08f3f7e2609a2f87913205350`  
		Last Modified: Wed, 06 Sep 2023 00:06:29 GMT  
		Size: 61.3 KB (61290 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:421c2e8b8b1c6c1d3947999b2d1c56b4b32f0f92a393d44a6fab8153f2259d63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63301480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35fb4e1a68033292397b8f962adcab425e8a073cf9fe837e7c016686e700b61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ae59b2d23c1225860de1ba5db630c5d985dad99e799af59bf6703718fb5db40`  
		Last Modified: Wed, 06 Sep 2023 01:30:14 GMT  
		Size: 32.8 MB (32782678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:790083b3783ab1447839d38d5f4127c97e0c50db5c072752efbc6a45909988cd`  
		Last Modified: Wed, 06 Sep 2023 01:30:13 GMT  
		Size: 7.9 MB (7947903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7262306011532bd69b71d9e72c12922be7cb0b5633c8c771004751790c1bd5b2`  
		Last Modified: Wed, 06 Sep 2023 01:30:12 GMT  
		Size: 1.5 MB (1522233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd64bb80c86b465099b0d00ed76da49187780d52f627de184ad8a4fa52509eaa`  
		Last Modified: Wed, 06 Sep 2023 01:30:14 GMT  
		Size: 17.7 MB (17700659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:baac0be2abf0cc643cf86896379de8390d7c1080cb89b236ecaa7c943017e2d6`  
		Last Modified: Wed, 06 Sep 2023 01:30:14 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:210179825bb2b29dc7396190efef4b6928e58ab6f3c0022a1e33c7f3bd9d8559`  
		Last Modified: Wed, 06 Sep 2023 01:30:14 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1301403b24a13df5931e096b91a5f0b0284214d7c24ee52f34faa464e7a84e2b`  
		Last Modified: Wed, 06 Sep 2023 01:30:15 GMT  
		Size: 624.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:695bd5091ad9fd76381d11819f3e2d28bd453029fa14485f7e3843df03a56c46`  
		Last Modified: Wed, 06 Sep 2023 01:30:15 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:9dedcfaec854ebc61c1ccf17976ae170a19cfaee389a9f444326def5eea44546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **757.6 KB (757595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05ba9865cfab33c28f23cee83e3d339f8f85963aacaab6aefbef13034e0e9db`

```dockerfile
```

-	Layers:
	-	`sha256:9c06d0c2e3fa046ab8f766a2cef70b2b0b3db2096da578ba621b81598499ec6b`  
		Last Modified: Wed, 06 Sep 2023 01:30:12 GMT  
		Size: 696.0 KB (695977 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c64c077441b50ae2d05abb852f1a024c18ff4e65ea63b514cfdb2e8933ad5c85`  
		Last Modified: Wed, 06 Sep 2023 01:30:12 GMT  
		Size: 61.6 KB (61618 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:7aee96002cbed9e7e1f32a70b2e73fcb2ec7e332b359275fc1e459cc27f1e878
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61270873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a78704a163e41314289d872399a9edb001619f4fc4e796c07f449f9c374db5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 01 Sep 2023 22:23:31 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_VERSION=3.12.4
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 01 Sep 2023 22:23:31 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 22:23:31 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 01 Sep 2023 22:23:31 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 01 Sep 2023 22:23:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 01 Sep 2023 22:23:31 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 01 Sep 2023 22:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 22:23:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 01 Sep 2023 22:23:31 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a64503492628bc3dcf32d329e1d15edf49bbcfe427c49faf8e5f6763049e6922`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 32.4 MB (32434658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc9637575282029d461cd71a90bde28042644769743dcd36ddf2c4e38a63c769`  
		Last Modified: Wed, 06 Sep 2023 00:52:50 GMT  
		Size: 6.4 MB (6424146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ed79074943acda31f9e021473eb008258c2795452dbff061c915e1101a10d1c`  
		Last Modified: Wed, 06 Sep 2023 00:52:50 GMT  
		Size: 1.5 MB (1495472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a5bf298c15c6f38b19b473e77497c39d403c1531958a0d9fad5dbe427ceb2ff`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 17.7 MB (17700650 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ace8a872fc5a69e22e7cfbba59d87fc7bb6723638d94e82b8406d7ed6c020b7`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e22414232df877c756b3627a93b3c956617ae1728d490579c5121bb719ea1ef8`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ae193595d0cad7c8333ad6109b019d1146fd97534b81e48f26bfa5bf91d7033`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bd4ad0c7052445a6a46449ed8eec4c93f931da51672e3ba25c396713517ab40c`  
		Last Modified: Wed, 06 Sep 2023 00:52:51 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:e6c78373c151dac54e10435d66359b6b2b04d6b3c5f9c154bf7ea5c9e8b5ba76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **757.5 KB (757472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:653a08b35940cf333f3b9ae097e4775aa659401a8d68d11f914b1ec17027cb9b`

```dockerfile
```

-	Layers:
	-	`sha256:f859103fd32af1ad15d1b98af1624bae63c27bb4f6411e2abe6b4c7986f31afa`  
		Last Modified: Wed, 06 Sep 2023 00:52:49 GMT  
		Size: 695.9 KB (695910 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a328a3a72519e04405f946b18755a733057b4087b4a82bc6996833bbd0ca6349`  
		Last Modified: Wed, 06 Sep 2023 00:52:49 GMT  
		Size: 61.6 KB (61562 bytes)  
		MIME: application/vnd.in-toto+json
