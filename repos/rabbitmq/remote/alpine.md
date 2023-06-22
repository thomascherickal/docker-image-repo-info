## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:fb70ea4fbb74e588ce0db0fe08a04585ff9f7788b69eecf676269af757ddfbfe
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
$ docker pull rabbitmq@sha256:fe25da8ec98fc23822ec40bc506d9e5450ba65b0f0f6186110e614ba650fa2d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74611701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144724c33a8ac3ef9432a363c881198023c2143d22b5b044f3e849a1057fa3ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/lib64/ /usr/local/lib64/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib64/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_VERSION=3.12.0
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jun 2023 22:29:47 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 20 Jun 2023 22:29:47 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 20 Jun 2023 22:29:47 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 22:29:47 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 20 Jun 2023 22:29:47 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7105f38de14903b07b75dc70b92141964ee14216511b1672bbd8ff3fb8751fc1`  
		Last Modified: Wed, 21 Jun 2023 20:58:21 GMT  
		Size: 430.0 KB (430010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fa4f60e0f1b206b4236b505907b10de056242813287537ea6aaa8e9638d2b7`  
		Last Modified: Wed, 21 Jun 2023 20:58:20 GMT  
		Size: 10.2 KB (10169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079995203f44e7c162dc73a9523f0d104f286ee7e8dde2673823b9c5864dd6d2`  
		Last Modified: Wed, 21 Jun 2023 20:58:24 GMT  
		Size: 44.2 MB (44161851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6c516fbae7b989379c0feddf09daab500d6f8c81c37c8212835c4d4226cbfe`  
		Last Modified: Wed, 21 Jun 2023 20:58:21 GMT  
		Size: 6.8 MB (6757632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abdf601b834e899d45203d7e8d88cf5192868d96d591a9662e5bf1d9d02e818`  
		Last Modified: Wed, 21 Jun 2023 20:58:20 GMT  
		Size: 2.3 MB (2296294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8c44fc89c91daefbcd3b11a866ecdd84e949ef550c3145ddf3b82624d7729f`  
		Last Modified: Wed, 21 Jun 2023 20:58:19 GMT  
		Size: 17.6 MB (17556085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6acaef3ede2f81d7c85dda0140c7b75bfd4e003de0ebbd54748408a780c87c9`  
		Last Modified: Wed, 21 Jun 2023 20:58:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b284821e75cd41dd350b15a76a1b907e61c8da60cf9e1b19e2b9290812e5cd`  
		Last Modified: Wed, 21 Jun 2023 20:58:17 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4af487dc82a5fa916d5d739cef7d70c1860be677cf3c4b4582a9a4f3375f3b`  
		Last Modified: Wed, 21 Jun 2023 20:58:18 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d766156761a4b0d27a58a3b63c2c77521ac5cac59bfd0862d317e31ed77563`  
		Last Modified: Wed, 21 Jun 2023 20:58:17 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:0d8b5193cdad88315f5233c02191ec3ee653ff4d0d81205c8d41f073ab317f5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63855897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278f5c89dc35de871aa23ac65f52cbce4ec3b5dd12eb264fd2e82589c1c0a9fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_VERSION=3.11.17
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 29 May 2023 23:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 29 May 2023 23:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 May 2023 23:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 29 May 2023 23:05:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044bc9a334ea1337e9930de4b6203b76be99c8dd2dffad0f20ced4a9042f5a1d`  
		Last Modified: Thu, 11 May 2023 20:54:38 GMT  
		Size: 404.5 KB (404523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafc2bcc96b6e2a8bc5bbfe3fea26022f81cccd469bf60f43d5f1d2111544656`  
		Last Modified: Thu, 11 May 2023 20:54:38 GMT  
		Size: 10.1 KB (10139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc4a24ae25c70bb88452490b773d177e48c9fe1888d27da65878981ba94e36d`  
		Last Modified: Thu, 11 May 2023 20:54:43 GMT  
		Size: 41.3 MB (41325520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202c916a3580d2e374b493ea9baa44fba8dcae3e4efa83ba91c09e813b57983`  
		Last Modified: Thu, 11 May 2023 20:54:38 GMT  
		Size: 1.5 MB (1452160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0c6acf112368d9ba348f7c56de81ac10b3ea9248bebcf907ff50857f34b2be`  
		Last Modified: Wed, 31 May 2023 00:11:48 GMT  
		Size: 17.5 MB (17506099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c7f0bfd5894ac75984685889bb9c0a23fb9be95017cf61601c2c2848870e37`  
		Last Modified: Wed, 31 May 2023 00:11:47 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43850d1debc6efe1994011af493ec57b6687db3fcb80a8f021ba07360c5b5dbe`  
		Last Modified: Wed, 31 May 2023 00:11:47 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e45a80132270eacf4110736d01b9ab452b16b5d21cd1c54229a7b2ce61384`  
		Last Modified: Wed, 31 May 2023 00:11:47 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abf86e99b7c0315ce8ee6bd5ce0751195b6a7fdb1e68dbe0266272d78d4583`  
		Last Modified: Wed, 31 May 2023 00:11:47 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:830f321fa7850c61df0332e7eaa498cfd75847247f8af2c24d44d891af05339c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62849489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7dc55cdb22179996fb96d29db0cd965db768595fb455e22869522c7e6cc0fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_VERSION=3.11.17
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 29 May 2023 23:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 29 May 2023 23:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 May 2023 23:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 29 May 2023 23:05:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d58005416a901ff5dbb19260fc9baabc38d474d27b4eca05e98bfc6f8fdd28`  
		Last Modified: Thu, 11 May 2023 23:06:28 GMT  
		Size: 385.9 KB (385883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885630bb46e4cc2babe293d3963ba05e1084385f406f1ed683205463c385e367`  
		Last Modified: Thu, 11 May 2023 23:06:28 GMT  
		Size: 10.1 KB (10136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4547e1dc1d6bd3fa59debbb887ad9df2a562b8bd122ecc9e5f1b721b5045a16`  
		Last Modified: Thu, 11 May 2023 23:06:32 GMT  
		Size: 40.7 MB (40736068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe69a85e561c45c11dd2d16784262d4a1db96bf1ddf1d61c03782866d08a7968`  
		Last Modified: Thu, 11 May 2023 23:06:28 GMT  
		Size: 1.3 MB (1298389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a7cfcd9c57da5af7f2c4f20bb1198e07c81e9ee8f6d67e49d4a98103b58b2a`  
		Last Modified: Tue, 30 May 2023 23:42:58 GMT  
		Size: 17.5 MB (17506123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc90f51d017b38f81c09fd2d1361db649fbdcf78f73a2645f5b014143713d50`  
		Last Modified: Tue, 30 May 2023 23:42:56 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c351bc4190ef4074983d6ab780d64cb850790465d892e1f2aaec2875631dcb`  
		Last Modified: Tue, 30 May 2023 23:42:56 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d798e138e24af6c63905f8db3a08976806d6dbcd35d615f9cb40d1d7312e3`  
		Last Modified: Tue, 30 May 2023 23:42:56 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc4ac78e5a3e5d1ab054fca73e1553613d76d6824c54d5c83ee91c36f854c03`  
		Last Modified: Tue, 30 May 2023 23:42:56 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:9dcb2bbac08c1184050cff4356f7b2ee6e8a62a348ba309ff8c466c1be867a59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71468743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd7807dfa8c3cbddfff0d09ac74030d7c354f6bbef23248939574c01087d0e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_VERSION=3.11.17
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 29 May 2023 23:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 29 May 2023 23:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 May 2023 23:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 29 May 2023 23:05:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc09cb57e7622aa5392403c0213487213cf0876bc3bce2482a940f102ca4f90`  
		Last Modified: Thu, 11 May 2023 21:32:26 GMT  
		Size: 406.3 KB (406263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468b4bb7c0fd3d362d0e2e6e082d76da5611ec3de01caca840fc7d526812cb2c`  
		Last Modified: Thu, 11 May 2023 21:32:26 GMT  
		Size: 10.1 KB (10135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effcd4314ff0fa70880398a1bf8a72b71e55d27cff3b89af36c0f06fa6087a1d`  
		Last Modified: Thu, 11 May 2023 21:32:31 GMT  
		Size: 47.8 MB (47824561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa026b4be19d2442f9e418ee1f281d124810044dcf133cac545b232d3fc9e943`  
		Last Modified: Thu, 11 May 2023 21:32:27 GMT  
		Size: 2.4 MB (2376679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bee420b5bdf33ea1625ba9e5a596a6b5bfc6760d09a67a6271e165db48dae63`  
		Last Modified: Wed, 31 May 2023 00:22:53 GMT  
		Size: 17.5 MB (17506484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cc3b3772a52892caa2c36a8b471179b9f280ee957c7a734d0770f9266cd691`  
		Last Modified: Wed, 31 May 2023 00:22:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274935d2a6385f6ae328f6445db1e0164d9c29e25cd0c517376a97058b278f33`  
		Last Modified: Wed, 31 May 2023 00:22:52 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad35dbd83858de0bed21aa2c755999d6db378027e98f66a0172f292c076bd61`  
		Last Modified: Wed, 31 May 2023 00:22:52 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7bf7a46fe3dcc3de5a5be36327a9c02e9b0acc21a1f85cbb8b5f584e8aa2b`  
		Last Modified: Wed, 31 May 2023 00:22:52 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:56705711a26f23e2e9bf56f2d595af44145d5b1b594034b77473cd11137001ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65734580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd41fff6f38a286c2aa6a1ceff0e9ee2529c90dd31ac8ce9a51e9efbf0cad6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:03 GMT
ADD file:cfe47ebe49c4a75094234cafa52aa13aa26abcdad49b89293585884b3a8faeae in / 
# Tue, 09 May 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_VERSION=3.11.17
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 29 May 2023 23:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 29 May 2023 23:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 May 2023 23:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 29 May 2023 23:05:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:613767c5530f4016482e81288d0efdca4e58c62031252130d8fccd6f6260a068`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.3 MB (3264862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3797653406942fcff56ed03ae7b553a86f4e10d0935bff482c7f2ba80909980`  
		Last Modified: Thu, 11 May 2023 22:16:56 GMT  
		Size: 442.2 KB (442227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d111c45db65d48cc0f0b14dea381372adf6da4ebf97747ddfad1e85d65ce018`  
		Last Modified: Thu, 11 May 2023 22:16:56 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438229541bd2d1b74501cf3dcdee73545417fd17689a0f9d2ce50e82625eaf1a`  
		Last Modified: Thu, 11 May 2023 22:17:02 GMT  
		Size: 43.1 MB (43109304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f1606d9a77c5eeaa17acec5bda78a169da54845327af26326765f6cab4c506`  
		Last Modified: Thu, 11 May 2023 22:16:57 GMT  
		Size: 1.4 MB (1400174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00ef8416007fefe835aa2166ebeb401476ca6790f013dd706ea08d9d17bc358`  
		Last Modified: Wed, 31 May 2023 00:32:18 GMT  
		Size: 17.5 MB (17506095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6d3585d1bbb3b5aa27134b9616eefeea46c5ff91988bd058626255c716e576`  
		Last Modified: Wed, 31 May 2023 00:32:16 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3aa9d7a9db162e7c66414396fe1cf8f6bc47b3e217228d64c64cde121d4a2a7`  
		Last Modified: Wed, 31 May 2023 00:32:16 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1449ca5c1c820514410c726b822b29d4b0758cf3a0426ae2127a149d304da706`  
		Last Modified: Wed, 31 May 2023 00:32:16 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2b45a7f5544e91557251e19d14066e5aaff7e23cf09736faf792057260137`  
		Last Modified: Wed, 31 May 2023 00:32:16 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:9d3823e9443ed6594dfd7d5a98b9cfbd84e9ee5577d9719cff0d88a336f6aed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66879688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b29f9ae05b0eb2512d0bb2073661a49651574e3753f4c45a7211db336b4f60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_VERSION=3.11.17
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 29 May 2023 23:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 May 2023 23:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 29 May 2023 23:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 29 May 2023 23:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 29 May 2023 23:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 29 May 2023 23:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 29 May 2023 23:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 May 2023 23:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 29 May 2023 23:05:18 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18915bb583dfce226748c270e7824d69c61aeb820261d7c27b725c9fee4700`  
		Last Modified: Thu, 11 May 2023 19:33:51 GMT  
		Size: 470.5 KB (470476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb45a6a57dff9eeadf63bdc3ba2c605d79b6a5d9568b5f75afe31af643a5de2`  
		Last Modified: Thu, 11 May 2023 19:33:51 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67f933735047f6288b8593f5b4f9e115586f56081a27829a5219d3363e979b7`  
		Last Modified: Thu, 11 May 2023 19:34:01 GMT  
		Size: 44.0 MB (43986035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668a8194fa7ad03f983ae32b687334b792b8ec586dbb7c72f4e26412c59b329c`  
		Last Modified: Thu, 11 May 2023 19:33:51 GMT  
		Size: 1.5 MB (1519560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f75319b95d597671b31331fb474096bb83a9b9bc423f4dd5c5c218f8503e2d`  
		Last Modified: Wed, 31 May 2023 00:09:39 GMT  
		Size: 17.5 MB (17506064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd686c7c2dfb28ee3c41fbf73d36bc9b4a84026a0eedaf0b42f03b48f30359fb`  
		Last Modified: Wed, 31 May 2023 00:09:36 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1f2ff79b1738ac2cd3cc917853b33feafd632ef997f813745b130598d7fc7d`  
		Last Modified: Wed, 31 May 2023 00:09:36 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0afede128715b339f5c832cce4bf2ceadc75747eaf1b1af8b2c0f0cf8dbdcb`  
		Last Modified: Wed, 31 May 2023 00:09:36 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494dc26a4e148543cd906b6d809bd5e13eba2d585aef91de0afe8e1396d15c03`  
		Last Modified: Wed, 31 May 2023 00:09:36 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:f591545d7728446cd6a319ee52691d0aa429a9249e2262caad5991a3d38f72e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64195628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebf12d87d222f408bebb15eaa79ce5643ea7f7c3a716378f48fdc8fab284f01e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY /usr/local/lib64/ /usr/local/lib64/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib64/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_VERSION=3.12.0
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 20 Jun 2023 22:29:47 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jun 2023 22:29:47 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 20 Jun 2023 22:29:47 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 20 Jun 2023 22:29:47 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 20 Jun 2023 22:29:47 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 20 Jun 2023 22:29:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 22:29:47 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 20 Jun 2023 22:29:47 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58496898bbbb3e0dee1aa4efc2c7bfbfa9f45cce58598506b1844f5b1438b6f`  
		Last Modified: Thu, 22 Jun 2023 10:36:04 GMT  
		Size: 428.1 KB (428061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d173ce7ab7182bcf7a28630e1bba3fe303f677caa71d108e67506b3ce972b9`  
		Last Modified: Thu, 22 Jun 2023 10:36:02 GMT  
		Size: 10.2 KB (10175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8828f2a30ea70d61e6576f883c2ad7e7472a0aa293bcaf75c38073ecbba89`  
		Last Modified: Thu, 22 Jun 2023 10:36:06 GMT  
		Size: 35.8 MB (35848844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494a23f33cc668899d3f98053aff5f7068724ce5e0ced4e48c4d7eba75b55084`  
		Last Modified: Thu, 22 Jun 2023 10:36:03 GMT  
		Size: 5.6 MB (5642845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a055543ccb4c0b544a78ab84b9b7ed06904f192770bc3a0385bf26ac71121d7f`  
		Last Modified: Thu, 22 Jun 2023 10:36:04 GMT  
		Size: 1.5 MB (1494942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f901afabe35313ff7876e479fbb5e2d5102fd29c7c684443a556c51fddfd2`  
		Last Modified: Thu, 22 Jun 2023 10:36:02 GMT  
		Size: 17.6 MB (17555482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6244c4b2ab687264595ebe069fd4696b935c4470d2ce86f19bff83c8575668f`  
		Last Modified: Thu, 22 Jun 2023 10:36:01 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a164179b8316f0d04d02defe1e3c6acb3a048a86648cb654ec1840342c039dc`  
		Last Modified: Thu, 22 Jun 2023 10:36:01 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c485a8c641f2653e3ee3fc8b03a379aff2ffb2418438a21ecc472049d0ca7c`  
		Last Modified: Thu, 22 Jun 2023 10:36:01 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529fac78aa4083c806c9c8f78aad04c466e09b0de276b5bc1d93419825ea27a7`  
		Last Modified: Thu, 22 Jun 2023 10:36:01 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
