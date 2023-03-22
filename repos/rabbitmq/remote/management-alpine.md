## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:edff8ef64a5cb93991672c4fc137c656dee6d17fa5598069286ca1fe0bcce279
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
$ docker pull rabbitmq@sha256:0f7fc0feef977d7b07ec9dc4a961588bb142068a4358694c70b73557893c90dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (89024861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79fee5bd2df99166e7d8aa595e79e3ed31a0991339f10eb490a52add7ae23104`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:b58970b6eea7d537cc98ff3919ef60d8e226d6cb3802a3e41a434e86bffea217`  
		Last Modified: Tue, 21 Mar 2023 23:32:38 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3211f5fde64cbc361976e5f131e187dbb8cb33b32b7a1d5ed4bea1973e0aa80a`  
		Last Modified: Tue, 21 Mar 2023 23:32:39 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacfc6bb4923fab62b453e8cc9d14e1c265b8d61ac6340ce9b89e94ab3617b72`  
		Last Modified: Tue, 21 Mar 2023 23:32:39 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1fbdc3d6def5e52897515ac88619631364ab19ab5a10c6c4029add4cd86d86`  
		Last Modified: Tue, 21 Mar 2023 23:32:39 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a11f0c368d248c6744dd3dbda85fca76084fa8c859e0f10cc56ecb732c59ee`  
		Last Modified: Tue, 21 Mar 2023 23:32:55 GMT  
		Size: 16.0 MB (16013150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:a6cd6a821d1d35bc7c2667a3a6d165129bbed8bc2725628e6e492c77fc0e78fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80173118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1e2e336e66665dfac79bb553e6d4ff821735acb373072159b1377497e621e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 23:20:13 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Thu, 02 Mar 2023 23:20:13 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Thu, 09 Mar 2023 00:39:35 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Thu, 09 Mar 2023 00:39:39 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Thu, 09 Mar 2023 00:39:39 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Thu, 09 Mar 2023 00:39:39 GMT
ENV RABBITMQ_VERSION=3.11.10
# Thu, 09 Mar 2023 00:39:39 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 09 Mar 2023 00:39:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 09 Mar 2023 00:39:39 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Mar 2023 00:40:38 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Thu, 09 Mar 2023 00:40:40 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Thu, 09 Mar 2023 00:40:41 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Thu, 09 Mar 2023 00:40:41 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 09 Mar 2023 00:40:41 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 09 Mar 2023 00:40:41 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Thu, 09 Mar 2023 00:40:41 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Thu, 09 Mar 2023 00:40:41 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Mar 2023 00:40:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 00:40:41 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Thu, 09 Mar 2023 00:40:41 GMT
CMD ["rabbitmq-server"]
# Thu, 09 Mar 2023 00:40:55 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Thu, 09 Mar 2023 00:40:55 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:49637e592c9731c9f228f3634a23009e198ef6508e6df433d8ac1f77ced2e02f`  
		Last Modified: Thu, 09 Mar 2023 00:43:17 GMT  
		Size: 1.5 MB (1456203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cd2d89ab2be7639ed8767fa9f4031d027271fcdee8379ea4f973769c61a464`  
		Last Modified: Thu, 09 Mar 2023 00:43:49 GMT  
		Size: 17.4 MB (17444032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361634185472f4710e315c38b4ab54b51eb49ff3c9c424488e5a7b7368ca81b`  
		Last Modified: Thu, 09 Mar 2023 00:43:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc1bb15cde2eb8caaf5be7fa9854c5c76fa81bf7aefa805cbfa602365032ed6`  
		Last Modified: Thu, 09 Mar 2023 00:43:46 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff56e85a5e9f6087c11411fb2aad40824fe55e7e6f9c19533840e3527f8d3c7f`  
		Last Modified: Thu, 09 Mar 2023 00:43:47 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb1632fbd0807dc373925321c6d80ae6609a07e2fe3d3b0dbc25bfd25046442`  
		Last Modified: Thu, 09 Mar 2023 00:43:47 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdff63e3c2fbe4f62c59d3357194e3de4dc3e8ca4aa3c3015224ae47b9e50e68`  
		Last Modified: Thu, 09 Mar 2023 00:44:09 GMT  
		Size: 16.4 MB (16414389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:74f84531081f01a2eded92be63246ae003e04672ede26ec3989f05544f817b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84402095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878eb1eabc1781b84eb0a18dd6481d9aed68595fed953bbfc4abf99b5f1ad74e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:f697b1307fa715a8bf3d03b4f8906df4dd95aa0b28d483ad4795e3b7e28f187d`  
		Last Modified: Tue, 21 Mar 2023 01:24:46 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8969e8bfb8d4ec620612c89e75d2c4c47f892d26a290e65615d52b2ab293a0d4`  
		Last Modified: Tue, 21 Mar 2023 01:24:46 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41217c41eaa579ff8604121bbd9030fda7e9ac715fbd1ec77cb8804fb48ebe40`  
		Last Modified: Tue, 21 Mar 2023 01:24:46 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178fa264e143e74048fc614fd1784f2fe9f201da5237c7e93e2726f40de3077b`  
		Last Modified: Tue, 21 Mar 2023 01:24:46 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61118629a4cd92c18184ebfb28a49cd9e1927d9fc0b8b8cd4306d5a394035deb`  
		Last Modified: Tue, 21 Mar 2023 01:25:04 GMT  
		Size: 16.1 MB (16100511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:ca2c377df3afc302c1ce24f069b63fbf58623360d4a51adc59fb6a128eb822ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92718327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00e9c23d23c6a6384a1d389d841f76adf548b0ada8d8b3a95d5b84273a34cc7`
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
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
	-	`sha256:6fe24d0f9786e5c455665de76e6f051a7cc52f4cdfc77312499dfaae7991bf43`  
		Last Modified: Tue, 21 Mar 2023 22:50:05 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27933e1f01de627020cae45a160bad28073c861f4031a4dd5f602d9ac157809`  
		Last Modified: Tue, 21 Mar 2023 22:50:05 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9dab3b252b14e69618c4c12fc3b8e098b56e22c3ddfa0afed6e7dcb7952ee4`  
		Last Modified: Tue, 21 Mar 2023 22:50:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f719004311da2aee48cd62fe8c47cb744ee537330fa53a56693a9c80c3bea237`  
		Last Modified: Tue, 21 Mar 2023 22:50:05 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45fb7f9af5fdedd73a17a92b5ce856fcf19511e6402f64a2fca40f20499eb3f`  
		Last Modified: Tue, 21 Mar 2023 22:50:21 GMT  
		Size: 15.9 MB (15930809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:7280004bcaa6b2961d54f9658b25f4c9886c5df5c8f61c8e98f59701e3d2aed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.5 MB (88498912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b933f0122ee3505c54543c66ddbd4720ca455faf74371fb54dd7ff7704450c`
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:109bc59051c206356f9ddf3f3df39fe9a5c5976275feeb6e218b7167f4a68315`  
		Last Modified: Tue, 21 Mar 2023 00:43:17 GMT  
		Size: 17.1 MB (17115523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:05e99af8757930cc7b25cb0401150f9feb8e971279aef692cb92563c9f636db9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89541177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe958bc24ab52826c46345e3129aa63e7d74e966ed662fdda98ac6ce7c67b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
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
	-	`sha256:a9e54974249b3052a53c3dc6ead9d412032e74d52db03beef2246e85fa914d0f`  
		Last Modified: Tue, 21 Mar 2023 01:13:50 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7382c3b52ff7be4614e410ed7e9545848bb3670ae40009348aae82d330e3c5`  
		Last Modified: Tue, 21 Mar 2023 01:13:50 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eccfef1abb9e7fee54883e8b22869a07aa1b23ee1f12f70c9f7a99e3135cd3`  
		Last Modified: Tue, 21 Mar 2023 01:13:50 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5869e443c891b7573bf5275c0d8f8f152fcf065922d3b5b723aab48e302fdb7`  
		Last Modified: Tue, 21 Mar 2023 01:13:50 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e9a2960ada4fd0ac9762b4489fa7fcb9cef2baf59347795693f7068f580e8e`  
		Last Modified: Tue, 21 Mar 2023 01:14:12 GMT  
		Size: 17.2 MB (17212042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:1785f788f6801c6d56c5bdfd2d772f43e57462856dd3efd7388d1dd2efd2dde8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80644785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4d23e2a8da969a718e28e2ff9b6dd9d562ee472981b1b814a5f69d16c899159`
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
# Mon, 20 Mar 2023 23:05:20 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Mon, 20 Mar 2023 23:05:20 GMT
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
	-	`sha256:361c798e3ee163f3ce33178027145afd1b0e419c32e25c6da780ee8a03853ee8`  
		Last Modified: Tue, 21 Mar 2023 00:46:16 GMT  
		Size: 16.8 MB (16818230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
