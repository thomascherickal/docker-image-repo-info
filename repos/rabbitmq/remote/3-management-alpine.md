## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:926bc6382f78965fd404f7535947a4743d04f71a50c384f69953f9384c505a70
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
$ docker pull rabbitmq@sha256:b50d126e93477cbcb4c58e0c6cfd32046fcd343a2cebdc2241e3251d51cbe667
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83441028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fdc90b9bf2b324452dfd9103f4cb691d8c5c5f2517617cf6153430b5a520a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 23:43:00 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 07 Feb 2023 23:43:00 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 07 Feb 2023 23:43:01 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 07 Feb 2023 23:43:03 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 07 Feb 2023 23:43:03 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 07 Feb 2023 23:43:03 GMT
ENV RABBITMQ_VERSION=3.11.8
# Tue, 07 Feb 2023 23:43:03 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 07 Feb 2023 23:43:03 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 07 Feb 2023 23:43:03 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 23:43:13 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 07 Feb 2023 23:43:14 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Tue, 07 Feb 2023 23:43:14 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 07 Feb 2023 23:43:14 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 07 Feb 2023 23:43:14 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 07 Feb 2023 23:43:14 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 07 Feb 2023 23:43:14 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 07 Feb 2023 23:43:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 07 Feb 2023 23:43:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 23:43:14 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 07 Feb 2023 23:43:14 GMT
CMD ["rabbitmq-server"]
# Tue, 07 Feb 2023 23:43:25 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Tue, 07 Feb 2023 23:43:25 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0989362bd9eb38b9d5b93303546a7e63baff454f603b1a9f7c4ccbe0b0964be6`  
		Last Modified: Tue, 07 Feb 2023 23:46:56 GMT  
		Size: 427.1 KB (427053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff349e9ae57933c243a7fa28abfc192709eee62197cd42ffe78651b84df28c72`  
		Last Modified: Tue, 07 Feb 2023 23:46:55 GMT  
		Size: 10.1 KB (10138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c7c827d14e9032e87bc1ee20ab40d44e9cf32e64a450a3a894094e84835eb6`  
		Last Modified: Tue, 07 Feb 2023 23:47:00 GMT  
		Size: 43.9 MB (43886492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828e779b5c3fab8f2e8cc3482a1619c3e4891cacf56c2845c4fa443283891fe0`  
		Last Modified: Tue, 07 Feb 2023 23:46:56 GMT  
		Size: 2.3 MB (2326150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023996e41769881aebbe583672008532a616e6e0f75d4bc4ddc4f69ccf8878a`  
		Last Modified: Tue, 07 Feb 2023 23:46:55 GMT  
		Size: 17.4 MB (17425533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb94a6970f69ba0c30dba12baa6e6c2d66c0245ff3a1defede4741207302bf`  
		Last Modified: Tue, 07 Feb 2023 23:46:53 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ba2aa6dfea920692d631670dd86a9b4893f901ab9e110449c84928a6fc351b`  
		Last Modified: Tue, 07 Feb 2023 23:46:53 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc5e234ab15bd05b5bfc994311ba5592117684dc13df0c1db4597d48ab62f98`  
		Last Modified: Tue, 07 Feb 2023 23:46:53 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5515b6f67e96ebb87c31eee0c05befe5230078708a0d549880cee7d13b31b1f6`  
		Last Modified: Tue, 07 Feb 2023 23:46:53 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692e829716222b7d14504dac7a5f5a17534a603d8d5774ddb71c5a314ae00779`  
		Last Modified: Tue, 07 Feb 2023 23:47:17 GMT  
		Size: 16.0 MB (15993299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:1944fd47d081fcba82cbee31e6d3c14cf351bb51fd37e7f6cf8a9b60b3e0bf2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80116904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784a519c9692b573b3914c2f3e43411e3ea0a1bc516a717b9a33b47a5e9f6429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:41:37 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 06:41:37 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Feb 2023 06:41:37 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Feb 2023 06:41:40 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Feb 2023 06:41:40 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Feb 2023 06:41:40 GMT
ENV RABBITMQ_VERSION=3.11.8
# Sat, 11 Feb 2023 06:41:40 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Feb 2023 06:41:40 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Feb 2023 06:41:40 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 06:41:52 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Feb 2023 06:41:55 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Feb 2023 06:41:55 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Feb 2023 06:41:55 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Feb 2023 06:41:55 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Feb 2023 06:41:55 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Feb 2023 06:41:55 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Feb 2023 06:41:55 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 06:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:41:55 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Feb 2023 06:41:55 GMT
CMD ["rabbitmq-server"]
# Sat, 11 Feb 2023 06:42:14 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 11 Feb 2023 06:42:14 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d0c3f7a4a33b2a924b66291480c1a3e4e061263cf72e1c534039b85c82f19c`  
		Last Modified: Sat, 11 Feb 2023 06:44:35 GMT  
		Size: 404.5 KB (404538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57ddef1f437c995fcce4ee02164ab60665394456d0aceea0595000f9eed07e`  
		Last Modified: Sat, 11 Feb 2023 06:44:34 GMT  
		Size: 10.1 KB (10110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13de07a5207117e484c8c9e64e058205c3da25eaf9b602edf18bec66a2092c0a`  
		Last Modified: Sat, 11 Feb 2023 06:44:40 GMT  
		Size: 41.3 MB (41295213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07299dd1e4e60e0addbed528d5fd8fcce4401fddd1910852c26a99de175172a`  
		Last Modified: Sat, 11 Feb 2023 06:44:35 GMT  
		Size: 1.5 MB (1455943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48876c3000f97f9b40ad72b68152a461516c99f699fad13c1db1d2a0d91af023`  
		Last Modified: Sat, 11 Feb 2023 06:44:35 GMT  
		Size: 17.4 MB (17424706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c043f876bdf2dfc8713f895a7b28dde30c60f3b386c6a88c967fd01a71809650`  
		Last Modified: Sat, 11 Feb 2023 06:44:33 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b16bbd3601e419640a0249da9bc06a76f49b07557114603e5c36c8097b5c9d`  
		Last Modified: Sat, 11 Feb 2023 06:44:33 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405f6cb567e1c98fa6cff08c61ee418fe5f4d659224338926421e98daf87d909`  
		Last Modified: Sat, 11 Feb 2023 06:44:33 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c22b7b368496b40d8f1edab3ad63b05c52e1ed9125f3207f9b912a1e2eb79ad`  
		Last Modified: Sat, 11 Feb 2023 06:44:33 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d3a8cf9db16b8eff78617fc5a447886221c33212c5b87f7bd2207d3e62de37`  
		Last Modified: Sat, 11 Feb 2023 06:45:02 GMT  
		Size: 16.4 MB (16413768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:1e77c32589b5083a21b4cfba5420e89a9d1554ffbf2d95cdd59057f3a113534c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.9 MB (78869071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e3b360d450463386ea2772ecef911f4daf91f136c87f2ac1a0da9136143e92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:53:48 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:53:48 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Feb 2023 05:53:49 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Feb 2023 05:53:52 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:53:52 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Feb 2023 05:53:52 GMT
ENV RABBITMQ_VERSION=3.11.8
# Sat, 11 Feb 2023 05:53:52 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Feb 2023 05:53:52 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Feb 2023 05:53:52 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:54:00 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Feb 2023 05:54:01 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Feb 2023 05:54:01 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Feb 2023 05:54:01 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:54:01 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Feb 2023 05:54:01 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Feb 2023 05:54:01 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Feb 2023 05:54:01 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:54:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:54:01 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Feb 2023 05:54:01 GMT
CMD ["rabbitmq-server"]
# Sat, 11 Feb 2023 05:54:19 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 11 Feb 2023 05:54:19 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c223d653a10296031ebb24c233604190abc7a4092bc236ed2ca07f2f7f57a364`  
		Last Modified: Sat, 11 Feb 2023 05:57:24 GMT  
		Size: 386.0 KB (386008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9f138c26765dbc8068c592053079154c08aba34e5f6a5e5669783f2c1ff0f`  
		Last Modified: Sat, 11 Feb 2023 05:57:24 GMT  
		Size: 10.1 KB (10117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76bdb29174e449d1c579c2294f75ca2cf341d03f5a6769278b41464a865e8f7`  
		Last Modified: Sat, 11 Feb 2023 05:57:30 GMT  
		Size: 40.7 MB (40712985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567d8a5a99a99466fcba50bbbb791a89548fcd7174d9c74e926788efa12d199f`  
		Last Modified: Sat, 11 Feb 2023 05:57:25 GMT  
		Size: 1.4 MB (1364890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2dcd764d2afe3248cb113bf02cf175b3487bd90a18fb3e971fa1668bb64ea6`  
		Last Modified: Sat, 11 Feb 2023 05:57:24 GMT  
		Size: 17.4 MB (17424712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08194dd8ba29186653f5fecc6c2254757255580ea266bb8079b9364969e8261d`  
		Last Modified: Sat, 11 Feb 2023 05:57:22 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908adb0944ebb489b20e91325853db2c791665d04573f99b21379ef1c9d7109`  
		Last Modified: Sat, 11 Feb 2023 05:57:22 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578f6f62c6100370b7c61bada5c6a4ccfd13644ffaa89b1026f171b4998bf68e`  
		Last Modified: Sat, 11 Feb 2023 05:57:22 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f282d355f9327a49e407b379fc4610489726e62b2f07cb6a9ae424408af69a6d`  
		Last Modified: Sat, 11 Feb 2023 05:57:22 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c6da53f963ad8732637c89367efc5c180dfce3ab13d74b683088e58b2d8697`  
		Last Modified: Sat, 11 Feb 2023 05:57:51 GMT  
		Size: 16.1 MB (16100130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:78ae46f419c065e13267f9a2ef3caf995e46ae7ae85657e2d85de6e7bf5537a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87191251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10616ecbd762c1f7b997860d56b916a976417e105daf97182aff9d7910fda182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:08:11 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:08:11 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Feb 2023 05:08:11 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Feb 2023 05:08:14 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:08:14 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Feb 2023 05:08:14 GMT
ENV RABBITMQ_VERSION=3.11.8
# Sat, 11 Feb 2023 05:08:14 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Feb 2023 05:08:14 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Feb 2023 05:08:14 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:08:30 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Feb 2023 05:08:31 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Feb 2023 05:08:31 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Feb 2023 05:08:31 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:08:31 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Feb 2023 05:08:31 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Feb 2023 05:08:31 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Feb 2023 05:08:31 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:08:31 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Feb 2023 05:08:31 GMT
CMD ["rabbitmq-server"]
# Sat, 11 Feb 2023 05:08:38 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 11 Feb 2023 05:08:38 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:3648792bdddf74ba1822a232325ba21b10276e2e769ad790e813fd9a68677c6f`  
		Last Modified: Sat, 11 Feb 2023 05:10:12 GMT  
		Size: 47.8 MB (47775974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe8107da25e33a5138ed2623609df2927772d84453048e7763c027d6359e4a`  
		Last Modified: Sat, 11 Feb 2023 05:10:08 GMT  
		Size: 2.4 MB (2379193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478b20b79ff2c2d7434b24e75b2cef3a64b4c1936f631d8d64164f292d82d4b7`  
		Last Modified: Sat, 11 Feb 2023 05:10:07 GMT  
		Size: 17.4 MB (17425407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b70989902a3ef22d771cf82781ac5cc0998c966c4aa2deaf3cc0438e0ca313`  
		Last Modified: Sat, 11 Feb 2023 05:10:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5f32d19faf5bab43eaf67bd4644402df925ffb174abee19a92b848c995a3ed`  
		Last Modified: Sat, 11 Feb 2023 05:10:06 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adea1063ba6cc1865ada98574918be7c8ad98ca0dc4af42eaf9d8ca1dbb722f`  
		Last Modified: Sat, 11 Feb 2023 05:10:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e271a9efef733008858b4bd8619a8f8fce6169e7bf8877cc6b01868727e9fe`  
		Last Modified: Sat, 11 Feb 2023 05:10:06 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d099fd998443750374a38ff6bfcfbc25144a22ea67b382503bfc3df475e6c`  
		Last Modified: Sat, 11 Feb 2023 05:10:28 GMT  
		Size: 15.9 MB (15930605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:b24617ac79fbbf770e69574236facb668170ffcf24349eb81f0202f74a032587
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79089770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c25c8c0752e88c7b2a05a866d679c0e00c568dd930011b00388afa5654b41e50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Fri, 02 Dec 2022 20:38:50 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata
# Fri, 02 Dec 2022 20:38:51 GMT
ARG PGP_KEYSERVER=keyserver.ubuntu.com
# Fri, 02 Dec 2022 20:38:52 GMT
ENV OPENSSL_VERSION=1.1.1s
# Fri, 02 Dec 2022 20:38:53 GMT
ENV OPENSSL_SOURCE_SHA256=c5ac01e760ee6ff0dab61d6b2bbd30146724d063eb322180c6f18a6f74e4b6aa
# Fri, 02 Dec 2022 20:38:54 GMT
ENV OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0xB7C1C14360F353A36862E4D5231C84CDDCC69C45 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x95A9908DDFA16830BE9FB9003D30A3A9FF1360DC 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xA21FAB74B0088AA361152586B8EF1A6BA9DA2D5C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D
# Fri, 02 Dec 2022 20:38:55 GMT
ENV OTP_VERSION=25.1.2
# Fri, 02 Dec 2022 20:38:56 GMT
ENV OTP_SOURCE_SHA256=5442dea694e7555d479d80bc81f1428020639c258f8e40b2052732d1cc95cca5
# Fri, 02 Dec 2022 20:41:09 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		dpkg-dev dpkg 		g++ 		gcc 		gnupg 		libc-dev 		linux-headers 		make 		ncurses-dev 	; 		OPENSSL_SOURCE_URL="https://www.openssl.org/source/openssl-$OPENSSL_VERSION.tar.gz"; 	OPENSSL_PATH="/usr/local/src/openssl-$OPENSSL_VERSION"; 	OPENSSL_CONFIG_DIR=/usr/local/etc/ssl; 		mkdir /usr/local/src; 		wget --output-document "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_SOURCE_URL.asc"; 	wget --output-document "$OPENSSL_PATH.tar.gz" "$OPENSSL_SOURCE_URL"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $OPENSSL_PGP_KEY_IDS; do 		gpg --batch --keyserver "$PGP_KEYSERVER" --recv-keys "$key"; 	done; 	gpg --batch --verify "$OPENSSL_PATH.tar.gz.asc" "$OPENSSL_PATH.tar.gz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	echo "$OPENSSL_SOURCE_SHA256 *$OPENSSL_PATH.tar.gz" | sha256sum -c -; 	mkdir -p "$OPENSSL_PATH"; 	tar --extract --file "$OPENSSL_PATH.tar.gz" --directory "$OPENSSL_PATH" --strip-components 1; 		cd "$OPENSSL_PATH"; 	MACHINE="$(dpkg-architecture --query DEB_BUILD_GNU_CPU)" 	RELEASE="4.x.y-z" 	SYSTEM='Linux' 	BUILD='???' 	./config 		--openssldir="$OPENSSL_CONFIG_DIR" 		-Wl,-rpath=/usr/local/lib 	; 	make -j "$(getconf _NPROCESSORS_ONLN)"; 	make install_sw install_ssldirs; 	cd ..; 	rm -rf "$OPENSSL_PATH"*; 	rmdir "$OPENSSL_CONFIG_DIR/certs" "$OPENSSL_CONFIG_DIR/private"; 	ln -sf /etc/ssl/certs /etc/ssl/private "$OPENSSL_CONFIG_DIR"; 	openssl version; 		OTP_SOURCE_URL="https://github.com/erlang/otp/releases/download/OTP-$OTP_VERSION/otp_src_$OTP_VERSION.tar.gz"; 	OTP_PATH="/usr/local/src/otp-$OTP_VERSION"; 		mkdir -p "$OTP_PATH"; 	wget --output-document "$OTP_PATH.tar.gz" "$OTP_SOURCE_URL"; 	echo "$OTP_SOURCE_SHA256 *$OTP_PATH.tar.gz" | sha256sum -c -; 	tar --extract --file "$OTP_PATH.tar.gz" --directory "$OTP_PATH" --strip-components 1; 		cd "$OTP_PATH"; 	export ERL_TOP="$OTP_PATH"; 	./otp_build autoconf; 	export CFLAGS='-g -O2'; 	export CFLAGS="$CFLAGS -Wl,-rpath=/usr/local/lib"; 	hostArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)"; 	buildArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	dpkgArch="$(dpkg --print-architecture)"; dpkgArch="${dpkgArch##*-}"; 	jitFlag=; 	case "$dpkgArch" in 		amd64) jitFlag='--enable-jit' ;; 	esac; 	./configure 		--host="$hostArch" 		--build="$buildArch" 		--disable-dynamic-ssl-lib 		--disable-hipe 		--disable-sctp 		--disable-silent-rules 		--enable-clock-gettime 		--enable-hybrid-heap 		--enable-kernel-poll 		--enable-shared-zlib 		--enable-smp-support 		--enable-threads 		--with-microstate-accounting=extra 		--without-common_test 		--without-debugger 		--without-dialyzer 		--without-diameter 		--without-edoc 		--without-erl_docgen 		--without-et 		--without-eunit 		--without-ftp 		--without-hipe 		--without-jinterface 		--without-megaco 		--without-observer 		--without-odbc 		--without-reltool 		--without-ssh 		--without-tftp 		--without-wx 		$jitFlag 	; 	make -j "$(getconf _NPROCESSORS_ONLN)" GEN_OPT_FLGS="-O2 -fno-strict-aliasing"; 	make install; 	cd ..; 	rm -rf 		"$OTP_PATH"* 		/usr/local/lib/erlang/lib/*/examples 		/usr/local/lib/erlang/lib/*/src 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 	apk del --no-network .build-deps; 		openssl version; 	erl -noshell -eval 'io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'
# Fri, 02 Dec 2022 20:41:09 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Dec 2022 20:41:10 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie
# Fri, 02 Dec 2022 20:41:11 GMT
ENV RABBITMQ_VERSION=3.11.4
# Fri, 02 Dec 2022 20:41:12 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Dec 2022 20:41:13 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Dec 2022 20:41:14 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Dec 2022 20:41:24 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie"
# Fri, 02 Dec 2022 20:41:26 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf
# Fri, 02 Dec 2022 20:41:27 GMT
# ARGS: PGP_KEYSERVER=keyserver.ubuntu.com
RUN ln -sf /opt/rabbitmq/plugins /plugins
# Fri, 02 Dec 2022 20:41:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Dec 2022 20:41:29 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Dec 2022 20:41:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Dec 2022 20:41:32 GMT
COPY --chown=rabbitmq:rabbitmqfile:1010d75e6e011d4f35a78624739f459bbc98829ae9696991358350d1bd6a12ac in /etc/rabbitmq/conf.d/ 
# Fri, 02 Dec 2022 20:41:33 GMT
COPY file:0667537cb067f2e42e0e1d5c1def14391eaf4bfe791bc7f23fd95a83eff81025 in /usr/local/bin/ 
# Fri, 02 Dec 2022 20:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Dec 2022 20:41:34 GMT
EXPOSE 15691 15692 25672 4369 5671 5672
# Fri, 02 Dec 2022 20:41:35 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Dec 2022 20:41:49 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version
# Fri, 02 Dec 2022 20:41:49 GMT
EXPOSE 15671 15672
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106b135302086d80cf3de30889854de32936475a67a9ed15c8205ff63b87fa47`  
		Last Modified: Fri, 02 Dec 2022 20:43:54 GMT  
		Size: 1.5 MB (1488436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357847e173988bd23ac6a111a3c0a7dd6e12c0b75185598db3bb71aac80a0a5e`  
		Last Modified: Fri, 02 Dec 2022 20:43:57 GMT  
		Size: 39.7 MB (39710207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e709778216bf6355663a739ec99dfd3312cf3537174949e267cf77fb54129d8`  
		Last Modified: Fri, 02 Dec 2022 20:43:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7a43c8aeb64114009c17fb0ddfd3f65a0753d5b537823e6e08cd2ad83e640`  
		Last Modified: Fri, 02 Dec 2022 20:43:54 GMT  
		Size: 17.4 MB (17394666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cb6fafe389215c18c61a6eeed8575ef4c2da2c2cd44b9a63d8619a9800fc60`  
		Last Modified: Fri, 02 Dec 2022 20:43:51 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068448666bae629bbce0504374b7b6d69916183f3d5cfe8b63573e9f4163b0f6`  
		Last Modified: Fri, 02 Dec 2022 20:43:51 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76914ddad249374f5fc5e1163226b125f32a2fcd81977b77d6363fd6de669c`  
		Last Modified: Fri, 02 Dec 2022 20:43:52 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749dc08e8d71567a70b83e8c7b8ee7085b07463c857fb76cf22b642172573b86`  
		Last Modified: Fri, 02 Dec 2022 20:43:51 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0258aecc01cb6501438768fa135b6dc375a0595d1f9876ace73488895c05d`  
		Last Modified: Fri, 02 Dec 2022 20:44:16 GMT  
		Size: 17.1 MB (17084834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:acae8cfe69a3747df31fbe0768d9633f04b0cde4beedf5b59f4fbc00fb1ff0e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.0 MB (83994143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd9bbc9b231813a7132c5b6e742db7603fe3b24fc7d62935c3d9112a5dd7c96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 04:56:11 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 04:56:12 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Feb 2023 04:56:14 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Feb 2023 04:56:20 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Feb 2023 04:56:20 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Feb 2023 04:56:20 GMT
ENV RABBITMQ_VERSION=3.11.8
# Sat, 11 Feb 2023 04:56:20 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Feb 2023 04:56:20 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Feb 2023 04:56:20 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 04:56:37 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Feb 2023 04:56:40 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Feb 2023 04:56:41 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Feb 2023 04:56:41 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Feb 2023 04:56:41 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Feb 2023 04:56:41 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Feb 2023 04:56:41 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Feb 2023 04:56:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 04:56:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 04:56:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Feb 2023 04:56:42 GMT
CMD ["rabbitmq-server"]
# Sat, 11 Feb 2023 04:57:04 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 11 Feb 2023 04:57:04 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:5fcd739344ee80df975fe0dbab9cb0a190f5555b294b80c66d576fd554c477f8`  
		Last Modified: Sat, 11 Feb 2023 05:00:50 GMT  
		Size: 43.9 MB (43928883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ac8762fbcf4bf8eee488ab971cdd2ec2b2c0e9b35705fad18b7a614953177`  
		Last Modified: Sat, 11 Feb 2023 05:00:42 GMT  
		Size: 1.6 MB (1555388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cd26ea7f82da9e05fe413ab303749cd65bab751a078bf59eabaf8b154b0e56`  
		Last Modified: Sat, 11 Feb 2023 05:00:42 GMT  
		Size: 17.4 MB (17424787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de2d95ccc852e5283a31f182f275a33a6dc4e3f3a66914bd613976f2b5f887f`  
		Last Modified: Sat, 11 Feb 2023 05:00:39 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a718744a5e3d092cb228be52ef0bea11543a70e260027e0ca9ad87ec8670c1`  
		Last Modified: Sat, 11 Feb 2023 05:00:39 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a8bf8181db6fd972fbcd286962bbc801d379d25dbb2c7c2bb82dbbae6b8bc`  
		Last Modified: Sat, 11 Feb 2023 05:00:39 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10028e22e195fb28a7257e727fdd3f4e70b51ea5423a1263f7c63c3e20fba3ff`  
		Last Modified: Sat, 11 Feb 2023 05:00:39 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a71c7da8dfec68e5c5b9ec3a6f403eca036095943deb7298aac9e7b40d9afb3`  
		Last Modified: Sat, 11 Feb 2023 05:01:14 GMT  
		Size: 17.2 MB (17211976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:ea92bcb8c5a391802b2255362a5e2d5e2ea029c59835f2cd5d41a93060cb0c81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75103133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:931868c6871c8943a2c656da6fc198193db04dc99b9dba35aa165d98f879a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:37:54 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:37:54 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 11 Feb 2023 05:37:55 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 11 Feb 2023 05:37:58 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:37:58 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 11 Feb 2023 05:37:58 GMT
ENV RABBITMQ_VERSION=3.11.8
# Sat, 11 Feb 2023 05:37:58 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 11 Feb 2023 05:37:58 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 11 Feb 2023 05:37:58 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:38:04 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 11 Feb 2023 05:38:05 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Sat, 11 Feb 2023 05:38:06 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 11 Feb 2023 05:38:06 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 11 Feb 2023 05:38:06 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 11 Feb 2023 05:38:06 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 11 Feb 2023 05:38:06 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 11 Feb 2023 05:38:06 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 11 Feb 2023 05:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:38:06 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 11 Feb 2023 05:38:06 GMT
CMD ["rabbitmq-server"]
# Sat, 11 Feb 2023 05:38:33 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 11 Feb 2023 05:38:33 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:303753df8aea15ac84ad7324b8cc865c62d54f576ab6969ac051fea1e480f418`  
		Last Modified: Sat, 11 Feb 2023 05:41:11 GMT  
		Size: 35.8 MB (35761405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a8dd5824417e96b312d56654507cbe5c03b30ea7a7dfed4758916ecf32d814`  
		Last Modified: Sat, 11 Feb 2023 05:41:07 GMT  
		Size: 1.5 MB (1486723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda22402202ee8f9153d4e90b183b260556f4b75adf66dae624d058ff115404`  
		Last Modified: Sat, 11 Feb 2023 05:41:08 GMT  
		Size: 17.4 MB (17424801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb210d9f03a2453254de539fe5b2d9dde4aa6436df97715693d3e54c144dd4`  
		Last Modified: Sat, 11 Feb 2023 05:41:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d60279d1210dedf159e971f7c0f09602b7b1a10907088c40df6c76b46eef20`  
		Last Modified: Sat, 11 Feb 2023 05:41:06 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d3cc8fdc9cc25593fe3f94e4ebfbf91b61a8a37bdd1a3bedc4d98c56e89cd7`  
		Last Modified: Sat, 11 Feb 2023 05:41:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24de22f20884216a162d53368ad12bad1736e600b31e6db8184f3857588506f8`  
		Last Modified: Sat, 11 Feb 2023 05:41:06 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153bce8d6f51e20278610da7bef4da2324abb4f27e3fd0dade088e050def0805`  
		Last Modified: Sat, 11 Feb 2023 05:41:23 GMT  
		Size: 16.8 MB (16818042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
