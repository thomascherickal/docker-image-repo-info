## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:1d08beb313d4a01f7746a7d97242ba6a19bcc37da03f796b5bf321fbcdc47f5b
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
$ docker pull rabbitmq@sha256:30b658d3fcd9e46a356ac367d892b7ee4883154fdbcf5afc973a1749035f6a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89685587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058176412b729d933c43d2f4e29727ed7c0be6df613389d38525f43739d336be`
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
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:83a5340e83cf9b9d9f813076b31e7f8acf951031fdb788c94e4461af64446de1`  
		Last Modified: Wed, 21 Jun 2023 20:58:41 GMT  
		Size: 15.1 MB (15073886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:fb54893a1f95569d803b65f73d25a21f56f69b1587b412d5b2b25e1c858c9a78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79433770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac45d9e457246ed770c3db953e7360f6f037e1de3413686c9a9d877af3ccd2b6`
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
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:576322c5e70ccaafd6772275a4b945129d3dde2bbddfaeb0ed1438becc96d608`  
		Last Modified: Wed, 31 May 2023 00:12:03 GMT  
		Size: 15.6 MB (15577873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:fc200efc71f4cf18d7fc474b03471fc7b04ffffea9e399f6d9ab34256ae01fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.0 MB (78034038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39be7de95676bdaeea6ea4a1fa39f8e788b34c1053494d7d06963716406efc90`
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
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:5635cc9bf5d92ca7ef100e32d79555ad0b1905187913fbb7294725c8f7869e40`  
		Last Modified: Tue, 30 May 2023 23:43:12 GMT  
		Size: 15.2 MB (15184549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:ef4c8c1ac47fbc54198b7ae423660868d70f538ed27f670ff1b3ec98a8cbbc4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86666832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d750b8061236d2fb6b168da95aa344caf31b9341c4a8b827c9a1a4c4d4c28a`
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
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:22237d4ed7183096a5b84d08f94b33e0da9957f92cb625d729fc8539116476b0`  
		Last Modified: Wed, 31 May 2023 00:23:07 GMT  
		Size: 15.2 MB (15198089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:d8f3f475c36e7b80964fcdf166c2a6d1920b42a67a5839c9134d323966b68450
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81952617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08360fb00162d8e0ca227f20a03996a7d12c5ca8684ceb8ba2b235abce84d55a`
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
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:8af3221d33c0d2f5ccf2528676d4433b1d18fc572016df55e9ba38da594d1f8a`  
		Last Modified: Wed, 31 May 2023 00:32:34 GMT  
		Size: 16.2 MB (16218037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:cfbb3fa67433c44cd862bbcc6d4219f7ba2d5203727f3da74b50120e4017902c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83147921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c6046a4157ebd1e30cf7a0f981f279cfb79b802d497de84ae607e651e04ebb`
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
# Fri, 24 Mar 2023 18:45:07 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 24 Mar 2023 18:45:07 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:2432dcfb1242ededb05924aa377dae4da249ae493120135db2b84941951f8621`  
		Last Modified: Wed, 31 May 2023 00:09:57 GMT  
		Size: 16.3 MB (16268233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:6d987a46d5a9bbcdf7548f7f1f1cdddc0fb82b65e02f51208ea763252a284a42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80296351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288b51d0639c40eb5850097e90fee6a46f3da82cc874707268116078fa40f705`
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
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:cf164d349a2bc2e0dfcc53944fb41230d5e302bbd385aa98d962a9bcebfbd2a5`  
		Last Modified: Thu, 22 Jun 2023 10:36:17 GMT  
		Size: 16.1 MB (16100723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
