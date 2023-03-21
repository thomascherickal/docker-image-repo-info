## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:d485d73d4d53ba3f4363f4ce46115fcc7fff3e52275b9449a8c5e775a4a8fb24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:beacc452b261c292ed9109c647b5c7b13aef940c71b8bf91bb721cb73dcac095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67538664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f03e52b56d10aea0537d831b1983b3a87af6b9247e83976ac853a03d18e9981`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_VERSION=3.11.10
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Mar 2023 00:07:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Mar 2023 00:07:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Mar 2023 00:07:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7963c6f2876757a02fa01c367be7ef658e3d4e8ff23ac968a0166d2f2bc412a9`  
		Last Modified: Sat, 11 Feb 2023 13:17:52 GMT  
		Size: 427.1 KB (427054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264d2cfd94921f1758308ab55e2dc1d5d14c011fe6c573d6755b6f0ab01bfffa`  
		Last Modified: Sat, 11 Feb 2023 13:17:51 GMT  
		Size: 10.1 KB (10129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44e0cc39d145a0782824e9957bc1990307d47fa58a250c63307e2326409b656`  
		Last Modified: Thu, 09 Mar 2023 00:50:25 GMT  
		Size: 44.0 MB (43954934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d7c84178ebaa0ee7498f8b4f8e569016509b0a3822152f697bb051b17f65fc`  
		Last Modified: Tue, 21 Mar 2023 00:05:44 GMT  
		Size: 2.3 MB (2326196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc2d6a6f1552e2cf3a49554b5528ebbf9b959377e88de0e3e2baed0fc74ad14`  
		Last Modified: Tue, 21 Mar 2023 00:06:10 GMT  
		Size: 17.4 MB (17444170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5633cab35146d786778265cb9191af83de087f2981c6ea7f420dc818792b1d1f`  
		Last Modified: Tue, 21 Mar 2023 00:06:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2644df322e44802459e3961e22fe5a6e012f99ed3cc860dee31df1cc5a31c`  
		Last Modified: Tue, 21 Mar 2023 00:06:08 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506e18b6effe82f5ea2e986824ec44f76555078d1ab5dbb484bfc6ecbdc4b461`  
		Last Modified: Tue, 21 Mar 2023 00:06:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e259f6033c6619c3edc9e16ae36db96a3613257f5cedcdd6b3975885c489ea2`  
		Last Modified: Tue, 21 Mar 2023 00:06:08 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:e652fec05d837955e559924f2fcd003833ff4cb3adbb2e644a4eee7c5282309e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69232290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c0b16343a0bdc92c1b2e225c62119a0ab03b8d6cbdfed44d91596dc878c2f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_VERSION=3.11.11
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 20 Mar 2023 23:05:20 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 20 Mar 2023 23:05:20 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 20 Mar 2023 23:05:20 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5286bf4ae85fb346faec01de59b2ba1462ba5b54533d362a1e312e04c046a3`  
		Last Modified: Thu, 02 Mar 2023 23:23:00 GMT  
		Size: 404.5 KB (404537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75459f5043bd24b1e4dc3e411ac67d24f69ccdc2605a9cb09e63d6ea1c89b805`  
		Last Modified: Thu, 02 Mar 2023 23:22:59 GMT  
		Size: 10.1 KB (10137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330850596dc9120bbc5d4391f397e19bcfce20789108ae8cae2f40243f34fa66`  
		Last Modified: Thu, 09 Mar 2023 00:43:22 GMT  
		Size: 41.3 MB (41331194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037d27a0b47364e6549acc0e2414acc5a2c7622f42c19d723e4f53dc31340ed1`  
		Last Modified: Tue, 21 Mar 2023 00:17:43 GMT  
		Size: 1.5 MB (1456189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79372e1d2c1a5cd9441e25feb102c766a268399991982eaca9751c17f5e5e793`  
		Last Modified: Tue, 21 Mar 2023 00:17:55 GMT  
		Size: 22.9 MB (22917607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c716fa2600a92b4b36332c94dc313031e37b789f8d85eaf607804889e496d879`  
		Last Modified: Tue, 21 Mar 2023 00:17:53 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd73a68973cc52a5e92ea85cadad5c6dd7002b78aeaa7ba3e8a74f63b4df04`  
		Last Modified: Tue, 21 Mar 2023 00:17:53 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d6ff7c7fdc7ebe5ce9607fa5d64a4519fbc0a4f9162102b726fdc1eee8425c`  
		Last Modified: Tue, 21 Mar 2023 00:17:53 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346116e6ab524c5011284a1a5151bf7149f3f4254186cd715375cddfe6dfcb4a`  
		Last Modified: Tue, 21 Mar 2023 00:17:53 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:1374993570311b1e70d4f899ae1a9ed9e31a97af2230260863fd32e34c670253
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62828011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:131fab7be3407f9178146f584e6f03b800532ba16f9e5dc50aac16dccfa15736`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 11:20:42 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 02 Mar 2023 11:20:42 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 09 Mar 2023 01:15:24 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 09 Mar 2023 01:15:26 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 09 Mar 2023 01:15:26 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 09 Mar 2023 01:15:26 GMT
ENV RABBITMQ_VERSION=3.11.10
# Thu, 09 Mar 2023 01:15:26 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 09 Mar 2023 01:15:26 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 09 Mar 2023 01:15:26 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Mar 2023 01:17:06 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 09 Mar 2023 01:17:07 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Thu, 09 Mar 2023 01:17:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 09 Mar 2023 01:17:07 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 09 Mar 2023 01:17:07 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 09 Mar 2023 01:17:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 09 Mar 2023 01:17:07 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 09 Mar 2023 01:17:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Mar 2023 01:17:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 01:17:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 09 Mar 2023 01:17:07 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b76bab40461f2741f62d2becf33dc368a428d814518695ff9d4296e106d56af`  
		Last Modified: Thu, 02 Mar 2023 11:25:55 GMT  
		Size: 386.0 KB (386009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2ff030771b9415872d63b0d24bc73fb1e7c26afeed69a28ea1ce91237d4ce7`  
		Last Modified: Thu, 02 Mar 2023 11:25:54 GMT  
		Size: 10.1 KB (10143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c96d077feaa15c8346f2e1880a8fa6b0b4338a454405b1949ad193949fcba`  
		Last Modified: Thu, 09 Mar 2023 01:22:14 GMT  
		Size: 40.8 MB (40752457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f36b4696b11179b39da07ac5effbf21092c99a99dbf8f5654739627c5b4b88`  
		Last Modified: Thu, 09 Mar 2023 01:22:10 GMT  
		Size: 1.4 MB (1365089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2de31a96ddae3edd69f3705493ca923924fcd7e0543103ca2869e3682113472`  
		Last Modified: Thu, 09 Mar 2023 01:23:19 GMT  
		Size: 17.4 MB (17444084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60358cbcc0ba4779793a8c54da7299b2da9064fd99286dca75a0265dde3a298`  
		Last Modified: Thu, 09 Mar 2023 01:23:17 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636658959c130b8f616ca545267124ef2e4d750dfd14f2f2707955660556fb18`  
		Last Modified: Thu, 09 Mar 2023 01:23:17 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808e04f6dbba956f15323b1ccdaaa764880af3410296cfbc2a6f834828e58d7c`  
		Last Modified: Thu, 09 Mar 2023 01:23:17 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb72772156f4eec118d434c3c43b6953123a389a6ab2b739f91d0ac3d925607`  
		Last Modified: Thu, 09 Mar 2023 01:23:17 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:f771429677452a91f77b5ef4df76801bd215b013e0f99f16d2eddd8a0a9c44f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76790415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:963fde9f0345a5316bb22d35b1373524ddde5abc77d39eafbf9036031dfa06c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_VERSION=3.11.11
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 20 Mar 2023 23:05:20 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 20 Mar 2023 23:05:20 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 20 Mar 2023 23:05:20 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b9fdb6ecf093b8d8724777a4d5ba0b80e0ee223f67bd939818afc45aa9e3b89`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 406.3 KB (406257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5c4afd33e0a2ee96cdb7545374ed71dc910f85d1d9520ab0b32676f5e588864`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 10.1 KB (10118 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:936525585b16c8069253071f07c232f948918e0ba1fe9dce55107c96d0b8e082`  
		Last Modified: Tue, 21 Mar 2023 00:37:10 GMT  
		Size: 47.8 MB (47812881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94cb67db73f1e9901a5fe2012faf5ed2a98e6e7fe6288b961e57536593721ba7`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 2.4 MB (2380061 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87d395e7b3ba9ae8400c6c16783fedb091ece3bb91053b6a52e59fb138187b3d`  
		Last Modified: Tue, 21 Mar 2023 00:37:09 GMT  
		Size: 22.9 MB (22917402 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70d3f7e3e4c4cb9b45210854758e271a1487385ff488626df5f0813991bb8f38`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5458a2c556b8c97b2852b2db3480d22f66d6dd102cc8d37ca00a2126ee5e38d`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8687856c63db31da74368a2ef3c2134b94e4dd6dadf22a0717d51b7967904300`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 503.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:febe816b5c1689eaf40bde37277637a3d6e43cf6e7d1d18dfd07b30b6306c921`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 836.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:e77191d1c6051b09a7894af2f1d1ba6b5c140157b70e95415a3902b94f4ee96d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **744.9 KB (744946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d57beda73bae08d214b6e610b0636000defd08f2385d2d57482fb7f106cc1ce`

```dockerfile
```

-	Layers:
	-	`sha256:e08de4a9b715bbbe041539c39185c89e54e9f0cbdbcf053e0a9929bd500490b8`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 688.6 KB (688637 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e033ac8d36f6aa12094fd9feb40d6a32687128b2fa4b8852231cfcdf84d26fd5`  
		Last Modified: Tue, 21 Mar 2023 00:37:08 GMT  
		Size: 56.3 KB (56309 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:b817c39b80fc949ebca37a0fd73e106657b99178625d105d72b9e9cfe8c65f1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71383389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1232ca9aeae0a692f113ca07ca14dd46dfdac6acd0e90afcade8eeff741fd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_VERSION=3.11.11
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 20 Mar 2023 23:05:20 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 20 Mar 2023 23:05:20 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 20 Mar 2023 23:05:20 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6aa49cf2486eed9049f1a809e6eff09d7c6188bab2993cca70af28eb4f74ccc`  
		Last Modified: Fri, 17 Mar 2023 06:31:05 GMT  
		Size: 442.2 KB (442234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464fe747a7eb0d730e84e74bf16896e3cd18f6d75f4aa3d37268c7d3827411a`  
		Last Modified: Fri, 17 Mar 2023 06:31:05 GMT  
		Size: 10.1 KB (10144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513ae53c4c2877c561c744e2d7e3a5879f50048636df0cb84795e24c858d10c8`  
		Last Modified: Fri, 17 Mar 2023 06:31:11 GMT  
		Size: 43.1 MB (43102635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21d69299b9306cbb4f9d020f996df0bbb1afef1fddccfed52b8a5886514c329`  
		Last Modified: Tue, 21 Mar 2023 00:06:06 GMT  
		Size: 1.5 MB (1496578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ca5fc9722d320c354a443a046ca7829e172218542121081fc4cba16c89c92`  
		Last Modified: Tue, 21 Mar 2023 00:43:00 GMT  
		Size: 22.9 MB (22917712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dde1bdbfffab9e806976890460cc083651238df795d5b65cf3d2db7e4ee89f`  
		Last Modified: Tue, 21 Mar 2023 00:42:57 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dec94350c63c9df1db81fa46f6e0a134f8e9e3bdd71d437a4520a05a95a906f`  
		Last Modified: Tue, 21 Mar 2023 00:42:58 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a875530dbe1cb9d2957a60c09a86dc6a409ec4d0ea6fd0dd59440d1e0334f4`  
		Last Modified: Tue, 21 Mar 2023 00:42:57 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001dd96fab178d9d04e5707cf1195c504da6641a25aac02abd3d2dbedb71e504`  
		Last Modified: Tue, 21 Mar 2023 00:42:57 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:f1f0b529ff0af68d662ae0a9a30c94618dd8113ec741e4e84bb0c1e6f97643c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66855582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9adee7e91c3230e56fbf517573e2e067e0158bdf34cc69883c22e3aa9062f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_VERSION=3.11.10
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Mar 2023 00:07:30 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Mar 2023 00:07:30 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Mar 2023 00:07:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Mar 2023 00:07:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Mar 2023 00:07:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Mar 2023 00:07:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Mar 2023 00:07:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc19507b0e3484e06793e889c4736e9a41e569b42305b639e85f6b48bce329ca`  
		Last Modified: Sat, 11 Feb 2023 05:00:41 GMT  
		Size: 470.5 KB (470478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927bc627d272f364d6cc58636184a3ed06669ab32fb286991d2b6f2c5be94f1b`  
		Last Modified: Sat, 11 Feb 2023 05:00:41 GMT  
		Size: 10.1 KB (10135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b171fe324f44add4f563228b711000497e2d28f2c9db9629d8d65d45ab9c5d15`  
		Last Modified: Thu, 09 Mar 2023 01:48:34 GMT  
		Size: 44.0 MB (43982910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404ac8cd65dfff2f3f641ccf799fdfc746921f61b8b21a0f9076bd50911f68e0`  
		Last Modified: Tue, 21 Mar 2023 00:01:06 GMT  
		Size: 1.6 MB (1555433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3e7042f92fc62a5bd294de383627c09ed9fc7b8aabbb22a62ad10be20c0d14`  
		Last Modified: Tue, 21 Mar 2023 00:01:41 GMT  
		Size: 17.4 MB (17444135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d60deede913be85c73daefbfbad1e7cb8a5a2ef7d298ba0614c345ff7424964`  
		Last Modified: Tue, 21 Mar 2023 00:01:39 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a7f1862e29548e9df04b89a29537c0a750359adb822fd5c1d8bd054aa51cee`  
		Last Modified: Tue, 21 Mar 2023 00:01:39 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544fff65126f5325af8a2abe72fa3375d9105cf8e87fc0dc3b800c347085b60c`  
		Last Modified: Tue, 21 Mar 2023 00:01:39 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383142c61dc4457b033e141c6881cddbc4bfabd6c82f7ab0bf523ad5cb0e0a5e`  
		Last Modified: Tue, 21 Mar 2023 00:01:39 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:43607bc37540dee9be3362253a89454b49fb300dc1218286c4db7975da8a722c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63826555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08df0c8778cb0ceea87fec08e4cd5891ac5f924b87c7f7e764433551ffcd12e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_VERSION=3.11.11
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 20 Mar 2023 23:05:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 20 Mar 2023 23:05:20 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 20 Mar 2023 23:05:20 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 20 Mar 2023 23:05:20 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 20 Mar 2023 23:05:20 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3903e2d450130a33dcea620e06c94a1cde137452fd31b84f67e982bd286d2c94`  
		Last Modified: Sat, 11 Feb 2023 05:41:08 GMT  
		Size: 425.2 KB (425170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59517ebedc9de50e001a4e1eaf3a4353d969c4c03fcd9f0e47f5310fe624f802`  
		Last Modified: Sat, 11 Feb 2023 05:41:07 GMT  
		Size: 10.1 KB (10137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f8b6741830d20a124265e7b28ce1509e77888378409a49637fa284d3990a80`  
		Last Modified: Wed, 08 Mar 2023 22:56:58 GMT  
		Size: 35.8 MB (35809988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f98f79faebfbe4d842a7bad5c8848439ae0610fa907807a8a3421d84fa1d73`  
		Last Modified: Tue, 21 Mar 2023 00:13:21 GMT  
		Size: 1.5 MB (1486757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f1e284734e9e154ee409446e0578dc68d62b768ec5d5776ffa0847cf0168cf`  
		Last Modified: Tue, 21 Mar 2023 00:46:06 GMT  
		Size: 22.9 MB (22917650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47df087161b3a8012f3c0b675ae036ec80ee4d03bff1756191d2ad8610e79667`  
		Last Modified: Tue, 21 Mar 2023 00:46:05 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0ec4b264b0e02b9579a25dd860fdbb1fa7adb5028f735c54b5a1d0d108db8`  
		Last Modified: Tue, 21 Mar 2023 00:46:05 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655e7e39eb19f550f31768878b3e2a4c7c0d9499290fa292ab8fd678bbf82dd`  
		Last Modified: Tue, 21 Mar 2023 00:46:04 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c96c382933eb224454d27f849f3b9b2d47e5da5b82eb7f47cb1ac38dd4c3a1f`  
		Last Modified: Tue, 21 Mar 2023 00:46:05 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
