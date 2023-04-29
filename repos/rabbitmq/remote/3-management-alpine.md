## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:78b7f840c111fbf55b0d506ba50fb40d7c974326b4bfcf0cb57acf1a774d4e05
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

### `rabbitmq:3-management-alpine` - linux; arm variant v6

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

### `rabbitmq:3-management-alpine` - linux; arm variant v7

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

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:d129f2dd9235ccc1acda2fea3176cfbae6d209bea92b148515be80319df341fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92758136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1da2f83b58adbd5075c6fa85b636755257c17b7ada05bbcd729be75f7e3e9c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
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
	-	`sha256:b3a1bee6bbc2792b51d36202bf8608e5da01b97a7ed66298dd3f00b1dbb01689`  
		Last Modified: Fri, 28 Apr 2023 00:49:34 GMT  
		Size: 22.9 MB (22945429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aed1bd67c51ed871a5ad4e1121fdc73963bc1b6593b19a9d641e2c8ec79869`  
		Last Modified: Fri, 28 Apr 2023 00:49:33 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c69ff2794ce7297bcf06ad209d46195d111f3b06d50d3c2a71291a5e4fd595`  
		Last Modified: Fri, 28 Apr 2023 00:49:33 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae8815f94b839cda5662d31370f36fbcb1fa411456b389d34bc63ceaa81f881`  
		Last Modified: Fri, 28 Apr 2023 00:49:33 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08555dfc6cac2182c280275ad4286453d814cae9ba45f5e599d38e3e03ef096f`  
		Last Modified: Fri, 28 Apr 2023 00:49:33 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d29a254fdd85f3b09dbaca23e332b04df44c8e175e7e91fae8283a74c3c0ed9`  
		Last Modified: Fri, 28 Apr 2023 00:49:49 GMT  
		Size: 15.9 MB (15931286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:4cf380da373674c0690adde6e9284cf7bb5a0091f5130205cd7574f7d2162b4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.5 MB (88531427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3126f8f251a2b344344119a0b445de43cc5255bc4fb09f6b9b336a8a63b428`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
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
	-	`sha256:3e1495baf43d814d7f6cd7cffa198b915aaf72d490ee5cc3b1efdec791bb323a`  
		Last Modified: Fri, 28 Apr 2023 00:39:09 GMT  
		Size: 22.9 MB (22945012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9469f85e97152d355038151611a22dd464615f2b982a1a9e736ca41109f9ad2`  
		Last Modified: Fri, 28 Apr 2023 00:39:07 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f10be7f5a61f735eafbcd886b65fca5c23f84891713bc562cf3ac98d8357d`  
		Last Modified: Fri, 28 Apr 2023 00:39:06 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dae6de715727affcf6c3d4245ca0cb895cbbffbf071ef8ac0df6179ffb9de7e`  
		Last Modified: Fri, 28 Apr 2023 00:39:07 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bde64a242fad4290579d258e289abef0cc8a2c2e4baf3279259aae3b7ed34`  
		Last Modified: Fri, 28 Apr 2023 00:39:06 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1269aa08e14ad3e92891a5cb0372cac36d60b58dd06ee78fd2333f73ec0d69f`  
		Last Modified: Fri, 28 Apr 2023 00:39:26 GMT  
		Size: 17.1 MB (17114644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

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

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:e267ed83e07395eddf02d8650fbf43f849203eb1f5f19360f5103f4733043e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80668278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:460fc080f7f2a7dd8fe65e70eb65f1f7733e41f0fc27fcce2121262d118bebd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
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
	-	`sha256:6d65491c3b51ccf6b6e63aafb0970da419f800b480510d986f9edc024c16af59`  
		Last Modified: Sat, 29 Apr 2023 03:28:50 GMT  
		Size: 22.9 MB (22945261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef75aa319136184dd49101f213ab4ab8505ed3d610aca6a6d1cd51700f05047`  
		Last Modified: Sat, 29 Apr 2023 03:28:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0491ac404ea00d6bf644a0570ca90f229d2c228314944253a8f87882bf0e2f`  
		Last Modified: Sat, 29 Apr 2023 03:28:48 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b64cfd839c0d127737bf3aa228e07c0155bac96ca588a3a45e0ff9a5c76bb1d`  
		Last Modified: Sat, 29 Apr 2023 03:28:48 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a583079e1bb4df2a8a1f9eeea5f44e877e6bb5cea530702179c42bdf12bb0dd`  
		Last Modified: Sat, 29 Apr 2023 03:28:48 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2409cbc383c043d3688b9541455523a5f2c8d8034cdfa444cb09d55793f72b29`  
		Last Modified: Sat, 29 Apr 2023 03:29:00 GMT  
		Size: 16.8 MB (16813732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
