## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:16e48198397dc2fd97ab14e1f0d8c9bf756760012e96d2e057c5de7bdaee6ac5
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

### `rabbitmq:management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:3d95b449ccf0332b785c804cf5a440d006b8f6c3c5a6c4fc713b57249302a8fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.1 MB (89058532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e800e42f2cfddc66b813af97f79dd80f89af6017051a6801a86727f1cd5add1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_VERSION=3.11.14
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 22:17:10 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 22:17:10 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 22:17:10 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:fb0b07c7c8eb8285cc14310bcac6068565f44adffa63d05e13098c306dd898c6`  
		Last Modified: Fri, 28 Apr 2023 00:22:24 GMT  
		Size: 22.9 MB (22945456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86905aeff320c343fb8e7bb53693aad8db7166b3dbfeaf8a964e447691875bdf`  
		Last Modified: Fri, 28 Apr 2023 00:22:22 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83996a1eb4d22e58ebb7a34a5225eefa8b200c01a54ae304d6fc9fb40bca8dcd`  
		Last Modified: Fri, 28 Apr 2023 00:22:22 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f483f0d28efbd0bcdef85ea95e4f236759ffb074d06151af3e0564a2b2f942`  
		Last Modified: Fri, 28 Apr 2023 00:22:22 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd2eaecfe9632b5d1d97f56854497d9548b8629eee8a90b7a0c754307b39071`  
		Last Modified: Fri, 28 Apr 2023 00:22:22 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7167eadfd7e9ffb60d963ecac3386695ce7900596420e973ebc4c1c49daa`  
		Last Modified: Fri, 28 Apr 2023 00:22:38 GMT  
		Size: 16.0 MB (16009119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:2da13b75d71986ccc732d2fe49de1c936ca071ac9bb9a449b8d6630da16b7c8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85676851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd88ce00762aa3512e29ebdc7310497e3fe15f3b2791c4dce0edfbff273c034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_VERSION=3.11.14
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 22:17:10 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 22:17:10 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 22:17:10 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:76cc946d1f95acbc548e954eeb66740dfe4ac8dfd0522c87329c674629b30e5a`  
		Last Modified: Thu, 27 Apr 2023 23:50:09 GMT  
		Size: 22.9 MB (22945108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e3a9904dd9394de702577ae3e8c5d0673278f4e2cc41fc6f0c56b744fc0fd8`  
		Last Modified: Thu, 27 Apr 2023 23:50:07 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0103c58e0787afbe6e6cafe83828820cb05e90acc7cb2997466f3709c677f3b7`  
		Last Modified: Thu, 27 Apr 2023 23:50:07 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12255a5bbfc8799a08e592400ae7a5cdac7ad2f769c5ed4d9db1f222c1cb8394`  
		Last Modified: Thu, 27 Apr 2023 23:50:07 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95316742eaf5f2149f84d8a104530640335723cf4d533c3e37597cb6bd73fc6`  
		Last Modified: Thu, 27 Apr 2023 23:50:07 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123133fc64de0ba8e191d6553cca6bac2ea31bc6227726c3bf5bb00564f459bb`  
		Last Modified: Thu, 27 Apr 2023 23:50:25 GMT  
		Size: 16.4 MB (16413580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:e078ddf36e87b8bead5f44ddf228b85e6c9ae39dea05d340ca05f00d7f89b8b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84436198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e98b87a64e7cee5a2f98775a9162c225c28c3e80480df2917b12fc13fc51102`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_VERSION=3.11.14
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 22:17:10 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 22:17:10 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 22:17:10 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:527b0c5dd15d7d2c7c5e934d8e487854ca1356b7f4cc5a1bf7d45a95e406be5e`  
		Last Modified: Fri, 28 Apr 2023 00:17:14 GMT  
		Size: 22.9 MB (22945003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad820d89ffe5a390b14d3d8bd9cda1722ba778fd686f49249de0b6a0b7b77cf`  
		Last Modified: Fri, 28 Apr 2023 00:17:12 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ff384d0e20362ed8b6ebd94a56fd801c989f111ab159f589940452ad8241`  
		Last Modified: Fri, 28 Apr 2023 00:17:12 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03261e357073596f2a97fcfbabd7da627b4646f4c09fe03f47bdb3daedb31be`  
		Last Modified: Fri, 28 Apr 2023 00:17:12 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0150f7af5671267dc670a3f6fe7c2bbe7acf2e07879602812e9995e92a8a326d`  
		Last Modified: Fri, 28 Apr 2023 00:17:12 GMT  
		Size: 827.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfd54f9cc956afa1ac30d6f1fc2e87ee6b22992025e0348479a41011f13c052`  
		Last Modified: Fri, 28 Apr 2023 00:17:30 GMT  
		Size: 16.1 MB (16095544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:68d6da69e58b4ab34f5d88c3c9eaf15f321631e7b06a2a8dbe8967e82f897072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92734636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c1df50beacefa974fc90f4750ee12bfad8c91675d6f88bf18c043fd3629b634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_VERSION=3.11.13
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 11:25:57 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 11:25:57 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 11:25:57 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:dcc868eec58ff1d1b72e290931eebafe410e4945dad97a3290f49c086100e4f4`  
		Last Modified: Thu, 27 Apr 2023 22:13:40 GMT  
		Size: 22.9 MB (22921978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623bd9e59ba4eac9489621ba49c4d36583dfdf8b6419fda3eb1819d2cf28377a`  
		Last Modified: Thu, 27 Apr 2023 22:13:38 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d4afcd1454ad681005dd5644a88337eebd1ab57e55a8b67b05a44a59567c53`  
		Last Modified: Thu, 27 Apr 2023 22:13:38 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba64098d8fa42afac128997602d032b474e626bb214016a0992bc743c30bc8c`  
		Last Modified: Thu, 27 Apr 2023 22:13:38 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57501940d20e1a59324d17ce9c48cff492f816cd3aa56aa777b6625cd6c3fd`  
		Last Modified: Thu, 27 Apr 2023 22:13:38 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c78abd67b1a82f0f5dba25094d0787f8dec3a296ceb3860e81634c83268ee`  
		Last Modified: Thu, 27 Apr 2023 22:13:53 GMT  
		Size: 15.9 MB (15931244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:3b605df9b949b922236e26639b5584aa4776aba54c3331a6f086b3f2188ceef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.5 MB (88508471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a306b4fbc4db8b293cb3e633c679cc61de87be815af25e422aac3c16c646c385`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_VERSION=3.11.13
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 11:25:57 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 11:25:57 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 11:25:57 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:989310beb684edeb87b2f0527b980b7303d13807bd5b78248a4b85d134bbcdf7`  
		Last Modified: Thu, 27 Apr 2023 22:22:25 GMT  
		Size: 22.9 MB (22922042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c907122a00a14323decb9659e6734a7bb2e455869888a01ec09f5e3a24f64791`  
		Last Modified: Thu, 27 Apr 2023 22:22:23 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5551560cf83284cdd03e6592cf6e8d59ea21f100a587b29c142729210e31fa67`  
		Last Modified: Thu, 27 Apr 2023 22:22:23 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df3d67036182f524d2eb233ac8460537361f3f5d247c8cd95d4e507fcabc458`  
		Last Modified: Thu, 27 Apr 2023 22:22:23 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ef7bdc14dd715f4862c492fea45178f8a4b103f816e7b9f7e955dcd9d2082d`  
		Last Modified: Thu, 27 Apr 2023 22:22:23 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cba9dbe3951a97d710cf3f1bf294ecd8b39339188a1906fea58f1e70c29275`  
		Last Modified: Thu, 27 Apr 2023 22:22:41 GMT  
		Size: 17.1 MB (17114658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:c1bbf7579f2188862c1c8dd2bc6277f75f5ecd522b8257d463d7c5d4cba9c79a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89566967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc024cc5bd4af23ef55c92b7956868c825c015782b254dd25e31accc3750a749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_VERSION=3.11.14
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 22:17:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 22:17:10 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 22:17:10 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 22:17:10 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 22:17:10 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 22:17:10 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 22:17:10 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:9861a5c3329dcb590f42d9e78b3dbdd0d30b6b216688b53dd07472021b368edb`  
		Last Modified: Fri, 28 Apr 2023 00:20:30 GMT  
		Size: 22.9 MB (22945130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74973216a37cccc49fd5bff20d15cff7f504c587458f6295ce725e8116e8ce6`  
		Last Modified: Fri, 28 Apr 2023 00:20:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ac4b371902a7e64be25570cd1468eca35e98b1d95b48d0a617f786341cc02d`  
		Last Modified: Fri, 28 Apr 2023 00:20:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f89294692d45e551c0d726db8f521affcec369575bccc69efee87a1fc1c087`  
		Last Modified: Fri, 28 Apr 2023 00:20:27 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50ad78a871ffdfac1949a619890092461737147eb81f598966196a57e876ea1`  
		Last Modified: Fri, 28 Apr 2023 00:20:27 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfdda9dd6323a5670b1274e9cb50a14fe5a562e088cb47edb5573d4e16138f0`  
		Last Modified: Fri, 28 Apr 2023 00:20:48 GMT  
		Size: 17.2 MB (17209905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:35dfbd8b64350457b7fe139c8c5a7352aef45199cd8e8a7daeb4f754ce8f3b71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80645122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700a10ee0a93e24a3c5f73329fae1854f942b0781d31f5a9214d4862a55b7879`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_VERSION=3.11.13
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 27 Apr 2023 11:25:57 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 27 Apr 2023 11:25:57 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 27 Apr 2023 11:25:57 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 27 Apr 2023 11:25:57 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 27 Apr 2023 11:25:57 GMT
CMD ["rabbitmq-server"]
# Thu, 27 Apr 2023 11:25:57 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 27 Apr 2023 11:25:57 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:5c0aefc8b139aebecde6cb65cdfd3c2a3127e771a02c8135965acf53ebe3ea8d`  
		Last Modified: Thu, 27 Apr 2023 22:16:23 GMT  
		Size: 22.9 MB (22922112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe52e8965b105fe628207c5403f92fb23c45f8d5155e2e29bdbf1d330589ee94`  
		Last Modified: Thu, 27 Apr 2023 22:16:22 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f3180493e9c7511535fcbd9aa6fd6b39ff9a3099d9a917dbd18cafc71384d6`  
		Last Modified: Thu, 27 Apr 2023 22:16:22 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8daa6cc934dc5002aaca3dba0f1e37962fb3ed499c244efe561146aba4252e98`  
		Last Modified: Thu, 27 Apr 2023 22:16:22 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b9f7b18ca197cd3ea6e47beeec21e396e823587fd6637aa5e8f7f846baeb0`  
		Last Modified: Thu, 27 Apr 2023 22:16:22 GMT  
		Size: 827.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2660cbcc933b938cac1f029d6a67dd1916a145239915f412d97392c14b3abefb`  
		Last Modified: Thu, 27 Apr 2023 22:16:32 GMT  
		Size: 16.8 MB (16813736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
