## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:728aae3676afac518c47abde61b60569cbdf36e406e4e279dcea3d4cd1901bab
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
$ docker pull rabbitmq@sha256:7f3a2ccf85d0011f7c9afdf31fb2ed0bad7859517f8a229d28c7de91cb3d55d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73011756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2e2b5ad950af858c2840ef7f9fdf4a09ecd79cdd2f8d1dbde062103b71b62b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:16d9da1c7ea541df2588953dfd1ab595c0d90004dac272915711d84f0c6145ea`  
		Last Modified: Tue, 21 Mar 2023 23:32:40 GMT  
		Size: 22.9 MB (22917212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb4f62bb50a3812c68bf4a8a0b53a44ae8c8818f8914b4401d9cee606591adf`  
		Last Modified: Tue, 28 Mar 2023 18:29:29 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6233df3aea7ca200caeeeca08900c9cfd8c312ea837a088941f71bb611c64`  
		Last Modified: Tue, 28 Mar 2023 18:29:29 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52cd81bfcfd852fbe7848a335fbdf5ef7a340424300e68c16a6aa11ca598501`  
		Last Modified: Tue, 28 Mar 2023 18:29:29 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab74cf5c9b781535921488688cdef5e15cc4e78dd7074b69347f77446426b3`  
		Last Modified: Tue, 28 Mar 2023 18:29:29 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:2b1288105938519c8a583d258907d47434012e43bdf7ddedd40fdbe1b282579d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69232331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc01a7997f14efabe6dbb1f42af82dcce17d2a609685b08c2a9bdb2b600d0f48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:aa6e07ccab2fe5a0c4d655f715fccb78afefb5b68b7cf78dff32c9a415b9333c`  
		Last Modified: Tue, 28 Mar 2023 18:50:59 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2f7b54dc1bab307afcc56463b3662a217cc823c0af23751b4d16753c1b215f`  
		Last Modified: Tue, 28 Mar 2023 18:50:59 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e2db33b11d858636011cc26f63ba2e51ade482314f7c0f3ae2c3406dbf4ae`  
		Last Modified: Tue, 28 Mar 2023 18:50:59 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e7c516873e6f2f0ff8324a7996686499dbd4607b389981b44576afd2474685`  
		Last Modified: Tue, 28 Mar 2023 18:50:59 GMT  
		Size: 838.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:1082966009c109eeaad175c4d872558db97d9c8d23b7899a70fccae5a74a3bb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68301630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1130771a20a3783100c40d2ede45b3fee6a3521c085476cd4661eb5cc302a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:21a1c8a9e7ac03807dbecdfc294f549504a69f6652cffea3ad5dd31175b762e4`  
		Last Modified: Tue, 21 Mar 2023 01:23:56 GMT  
		Size: 1.4 MB (1365045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a9104e1a7cefc3fe0de20a5c2df31ed1d6c6d8798703428c8550f4989d30ba`  
		Last Modified: Tue, 21 Mar 2023 01:24:48 GMT  
		Size: 22.9 MB (22917698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cd7bba355a6d5c7526abe45b81935794b203b7c834255b71969a785e56a962`  
		Last Modified: Tue, 28 Mar 2023 19:19:15 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69081a3a685efc7dc2cad8142ad0c392ebb5798a28855e5aa47b1bb0da2ea3d6`  
		Last Modified: Tue, 28 Mar 2023 19:19:16 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e660c6aa89ceddeae96e0694a624cfa9f850c3c08cdb66b7738f4e5362adb16`  
		Last Modified: Tue, 28 Mar 2023 19:19:16 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e095f0fa59569a975b0a99b7e43f5f4df41e8d7a419877bcb100f10844e7fd1c`  
		Last Modified: Tue, 28 Mar 2023 19:19:16 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:c9524e9d3e0c5d419e2c49888e7408fb077aa7a849b1d021363195d95a153e85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76787567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32e2837aa1dbee67fba2b32f6e8a5bfcd4cda1c76a80af6277515469b9e1c619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f83dd11ba98222a308d6b1c8e3fbcc614be08b5b343c231502b807b3f65c78b`  
		Last Modified: Sat, 11 Feb 2023 05:10:08 GMT  
		Size: 406.3 KB (406251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984a5d4845a76d4f0a96bc3250027e6623b98d1e6aabb4801d307321859c93cc`  
		Last Modified: Sat, 11 Feb 2023 05:10:08 GMT  
		Size: 10.1 KB (10123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8a839f9cefa110a333c76b0e1ebea937c9076633d7a5be4299746b57d3588`  
		Last Modified: Thu, 09 Mar 2023 00:17:44 GMT  
		Size: 47.8 MB (47810892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a17de3ccc24293218c82ad08076d4613b9061a80f2690965a62fd79d269a954`  
		Last Modified: Tue, 21 Mar 2023 00:17:27 GMT  
		Size: 2.4 MB (2379260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb7502252e2f85b8599f59e206eb131314b59faca4db9b0af39d816e68f4d5`  
		Last Modified: Tue, 21 Mar 2023 22:50:06 GMT  
		Size: 22.9 MB (22917298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e818661bee85dbc480c384c9f253d0219e3a6f48682c91aa4343f5e11cab594e`  
		Last Modified: Tue, 28 Mar 2023 18:53:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a855c93a8841358be19f41e7adff0966100ff78c784faf6df90921ea7feac73`  
		Last Modified: Tue, 28 Mar 2023 18:53:25 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91be2a2141d4f135d81e5e9ac40f5decdca06aa28213459c380f315625297bb`  
		Last Modified: Tue, 28 Mar 2023 18:53:25 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf88a8e47adeca0658f8c7729539e409a2ef76fff727a1921c3d289b3a387053`  
		Last Modified: Tue, 28 Mar 2023 18:53:25 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:702b8d32ed0e08e26baf175ae199ef5b45b100419dc9232a12fdc0a2ead2c32f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71383439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c992c40da74353fad93786c7b4bc99f4c4312cdc7689b171579dc1e26c6d72f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:346ac527d622e7089740aeff8a1112715c270320b8cb5e555993554fc68d4fb6`  
		Last Modified: Tue, 28 Mar 2023 18:39:56 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68a40121b50c5d0df5ef83babf76aa6604f31c661df3124805d12db349cf736`  
		Last Modified: Tue, 28 Mar 2023 18:39:55 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d428a5aa5cdc272f71ae435e7d23daac4c34cb9b3f967b974abd329535495368`  
		Last Modified: Tue, 28 Mar 2023 18:39:56 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb456de4ddbb302334ba5e72fa223e2585b526cd0732d27b0e2622ec89718f72`  
		Last Modified: Tue, 28 Mar 2023 18:39:56 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:d58a304e79d79fb38e9e2c0cbd43bc60748beba4d9217e91fa5f6c933f979f10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72329180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8ca40face4cf67ddc274127588d65e9b9ca1ae3ca29fa0520a04f69d2111afc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:b1f44e85a248111b0f9d84b72b78209edf4f387b5f70995804b57123025f3c55`  
		Last Modified: Tue, 21 Mar 2023 01:13:52 GMT  
		Size: 22.9 MB (22917691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5e10c1a5c696a4c10ad0eb5a34f38001b744ac11f6ad4bd61ce2ef30d1b89a`  
		Last Modified: Tue, 28 Mar 2023 18:23:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ceef775677a31963622a979609532030ded5501ca9c05b54dcd954d9dd2713`  
		Last Modified: Tue, 28 Mar 2023 18:23:51 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15390165345e2568fa508773edb91c9fa2d0c9db610ac4da485c9e6be67fceef`  
		Last Modified: Tue, 28 Mar 2023 18:23:51 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292d4ca894e9a6f1febfdb18eb0377d122eb4133a14a001fb149b86dfd6242f7`  
		Last Modified: Tue, 28 Mar 2023 18:23:51 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:6bc3b0a5bc26721e7634df91289446b79617e24f5741f4744ec76ef520e52954
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63826596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3a40354377c4a6e45a71254aebf90735684a08230be77b3166bceea171391f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_VERSION=3.11.11
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 24 Mar 2023 18:45:07 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 24 Mar 2023 18:45:07 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 24 Mar 2023 18:45:07 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 24 Mar 2023 18:45:07 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 24 Mar 2023 18:45:07 GMT
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
	-	`sha256:d5e05276f358a6bc5554c10b07a99c7f94c1e1ab20150450686e6c2a97030c89`  
		Last Modified: Tue, 28 Mar 2023 18:46:38 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14682eeaa62550a344cca450e2436b5482879d98987f357e242ecadc1e2468`  
		Last Modified: Tue, 28 Mar 2023 18:46:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f099d389a5744d6c067daf340bba17f03328f2a9c709292202b88ae8bffdddb`  
		Last Modified: Tue, 28 Mar 2023 18:46:38 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f8896724c930697837cdb3f569e8efb5b36dc0683efb9b9d622af7b3a68a7`  
		Last Modified: Tue, 28 Mar 2023 18:46:38 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
