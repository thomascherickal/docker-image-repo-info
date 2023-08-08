## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:3771c1e722bd13628f859f9f9ae160e40041a2c984595859badceecc080a876f
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
$ docker pull rabbitmq@sha256:6b60e8b99037d65983f219de8e1835e5a90b802f54ea81adbe26c021fd786130
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74705157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea424c9ba5a055cfafe79f2dc68d2968142b2ab044a09553c259ddc0f0151311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fed1a6574a104c010807db408eb1b954f7400ee52c6617701f79f54243932e7`  
		Last Modified: Thu, 03 Aug 2023 01:01:15 GMT  
		Size: 430.0 KB (430006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84a4c591794d351f8348c22cedf15f43e6ce236e6f8362c04224fc9df13e39e5`  
		Last Modified: Thu, 03 Aug 2023 01:01:15 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcf969cca126203ce09ea9b7339f4f438a56301d21fc9eebb61f57ed381e27a1`  
		Last Modified: Thu, 03 Aug 2023 01:01:18 GMT  
		Size: 50.9 MB (50902267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c7066e4adf18dfce1b1157ce4a60d9dddb57b90abb573bb3a37a316cb7354e6`  
		Last Modified: Thu, 03 Aug 2023 01:01:15 GMT  
		Size: 2.3 MB (2296123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3106be517870c7de09d1acf073e0f131b7b19c7d830b6ac2f65b5f276adf840`  
		Last Modified: Thu, 03 Aug 2023 01:01:17 GMT  
		Size: 17.7 MB (17666987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f4387180d16ab369b7cefaf1ba0999602931fed768894b65646a0ef8844db2f`  
		Last Modified: Thu, 03 Aug 2023 01:01:16 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c9529180e6837d7d8e63aa427b52b89fb888b394a46389898a0650d2a99ca91`  
		Last Modified: Thu, 03 Aug 2023 01:01:16 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8fb5ed39a39621f7a9c128a444eb1362a1501593bb49f319345d6ad2b5cab01`  
		Last Modified: Thu, 03 Aug 2023 01:01:17 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74577e4b3daee79fe506b5917a938cec08076c47d9660e8c9427fb2b12029a7c`  
		Last Modified: Thu, 03 Aug 2023 01:01:18 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:2d21573a85013b5dec08c56c7f05f5ee0e20e56168b619ee9674442bd6b99af9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **760.5 KB (760485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b4dbce01326accc7f797e7e4bfd06c877ffc8bfda32828e7726074d62390c7`

```dockerfile
```

-	Layers:
	-	`sha256:cdbb845abde33bf4e7edb56975d121c97bc409c78ffb26fee583cdece98f1a3f`  
		Last Modified: Thu, 03 Aug 2023 01:01:15 GMT  
		Size: 701.5 KB (701508 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c030e385202bf99046394c93616fe4f76b16701948af77c67132da456e04d5dc`  
		Last Modified: Thu, 03 Aug 2023 01:01:15 GMT  
		Size: 59.0 KB (58977 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:050bcc25cb0c0cd87ef2cd3ecf470274f824e2e31723ae651ee051898892c78f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64008802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fd31fcb5bd9ca15534febfd8b8ebbd9cc0989d9f1004304e48249ffc87ddb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Mon, 17 Jul 2023 17:37:26 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 17 Jul 2023 17:37:26 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
ENV RABBITMQ_VERSION=3.12.2
# Mon, 17 Jul 2023 17:37:26 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 17 Jul 2023 17:37:26 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 17 Jul 2023 17:37:26 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Jul 2023 17:37:26 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 17 Jul 2023 17:37:26 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 17 Jul 2023 17:37:26 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 17 Jul 2023 17:37:26 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 17 Jul 2023 17:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Jul 2023 17:37:26 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 17 Jul 2023 17:37:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5781bdd6b98f88b6a42e80aac18988828ca6f4df1adb961b82d0699fb035bc7`  
		Last Modified: Mon, 31 Jul 2023 22:30:31 GMT  
		Size: 407.4 KB (407409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce953f5bfeb468181877dd524ff1bee270ca2582c893ddc7083c71409cdbff6`  
		Last Modified: Mon, 31 Jul 2023 22:30:31 GMT  
		Size: 10.1 KB (10138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede374d943a6cbc1f22ea9824bf905b3e367de5c7e5f781313f6724ce2784600`  
		Last Modified: Mon, 31 Jul 2023 22:35:03 GMT  
		Size: 41.4 MB (41374967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22718ecc4d67b3ebc36448e9bea6010ffb253fce8fc30a412ba33c27a1fcd1e4`  
		Last Modified: Mon, 31 Jul 2023 22:34:58 GMT  
		Size: 1.4 MB (1404252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0338c6cb990390cb932e57c97bdaaa051d3342edfb71740e3d1a3b83ad58ed0d`  
		Last Modified: Mon, 31 Jul 2023 22:34:59 GMT  
		Size: 17.7 MB (17666934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a73a52f8e3b50715b13ccfe7eb8fceae460272af9b349a58fdc06fc898830`  
		Last Modified: Mon, 31 Jul 2023 22:34:56 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac57dcc0b9c845c62e03592520de3cdf698472ee5d606f4f999a088f454d0a1`  
		Last Modified: Mon, 31 Jul 2023 22:34:56 GMT  
		Size: 109.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79da68e53abb17d7a7e9e7f3db59c9d54f98f641d195f3a4bb37fe22584d8589`  
		Last Modified: Mon, 31 Jul 2023 22:34:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce1e3281dd8973973247e9d24635df5e95b27daf8bd32d9a6099d5fc4fbe2c6`  
		Last Modified: Mon, 31 Jul 2023 22:34:56 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:ee9d5b41489ad6a98e20ec4c805131923b220f59c3b10877e75965fd38b652da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63068327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9123e45bb17e229f011e68a91a9cd94a33bbe74dbb893851ad8c2a6fe9e9873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca6432ae6ac3a727d9185a7334ab4e98d7100bb1eea1660585b24feacbfd8c49`  
		Last Modified: Mon, 31 Jul 2023 22:30:44 GMT  
		Size: 389.6 KB (389598 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f14cf47721c0357c4b8c1d4d8f46ef520f600a92886f80062a9b8cc045116994`  
		Last Modified: Mon, 31 Jul 2023 22:30:44 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21684b3e40017b6382dc0f3bbe0632753476644242fc2c4f3c9ff56238430001`  
		Last Modified: Wed, 02 Aug 2023 23:59:24 GMT  
		Size: 40.8 MB (40802833 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7f4f29600ab84f42d00fb6b5fde5dbb443f88d5ae72d332af41a811823c1293`  
		Last Modified: Wed, 02 Aug 2023 23:59:22 GMT  
		Size: 1.3 MB (1298629 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4041530ee50be2553b1a385d4baf6ca3ba4eb919c9e53ad94ff4b4a8ec1f4d3a`  
		Last Modified: Wed, 02 Aug 2023 23:59:23 GMT  
		Size: 17.7 MB (17666869 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85601845e236385d1907da8b721bfd0398141aba9a6414b9d344f412b371c9b0`  
		Last Modified: Wed, 02 Aug 2023 23:59:21 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8541e3c252c2a0074016569867db2c1ac94ec69f42ec6065feafa03ca985f5a`  
		Last Modified: Wed, 02 Aug 2023 23:59:22 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d56f990f9f786a79db4768399e07a3a275ae9cbe80b3f9b4a8bf8741f7c2364a`  
		Last Modified: Wed, 02 Aug 2023 23:59:23 GMT  
		Size: 616.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7235b8be7850ea250a697c4cee5c410fdac9fac7d440f76616e175d1f8feddf`  
		Last Modified: Wed, 02 Aug 2023 23:59:24 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:c81a99beb9da52c81aac17bef3f80a5a374775cfa749298f7dcaebcf3cae06bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **756.5 KB (756501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37138c36a79c217f797f8540cbf85cb6b6598c260b9e90fc0c21d96e649e192e`

```dockerfile
```

-	Layers:
	-	`sha256:87cfe3ac189f4e221a0d55155e8d1502e1b0404e256207c27ccf1fcf5f0107db`  
		Last Modified: Wed, 02 Aug 2023 23:59:21 GMT  
		Size: 697.5 KB (697451 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:20dff2a332f561230e128ba6aa90dc19fde41bcc38817c3287dfc0bf0bdc1b4c`  
		Last Modified: Wed, 02 Aug 2023 23:59:21 GMT  
		Size: 59.0 KB (59050 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:a3046c37e203afafcb3c81e22ba86470f29203052231fb60795f335534380980
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71766745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5913d8142332ddd1fffbac56f1a66c2a026dba438a73cef9e0f824b9219b1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 01 Aug 2023 00:34:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27b8384455f1f732d98348aa474c19aef0ac17be4344cba594e4bc885dde071e`  
		Last Modified: Mon, 07 Aug 2023 22:48:59 GMT  
		Size: 408.9 KB (408868 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c2f13a8e684439143928e24fa5f38e34c2f9d616d81558689ce686a598b70f2`  
		Last Modified: Mon, 07 Aug 2023 22:48:59 GMT  
		Size: 10.1 KB (10139 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8604870aa2ff46be668d6365db7570333e5ab19240909ff64042a4723e299a8`  
		Last Modified: Mon, 07 Aug 2023 22:52:13 GMT  
		Size: 48.0 MB (47979883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5bd9def1156aac50f319e16146e04427f69a87e27f020d30f9dd966ae110994c`  
		Last Modified: Mon, 07 Aug 2023 22:52:09 GMT  
		Size: 2.4 MB (2368261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1316ff46bbe2315712fd1b1c52fbffd3ef72a418868833e7dd8dc563c8de6c66`  
		Last Modified: Mon, 07 Aug 2023 22:52:10 GMT  
		Size: 17.7 MB (17667075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0476aae46ee6469aa2d692022dfd168524da6dd3c17abc0e729b9a4757a8f116`  
		Last Modified: Mon, 07 Aug 2023 22:52:09 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:458ad3eddadfb4c5e4fdcef9e8e6264bc0170f546a68783b4824db7bab261450`  
		Last Modified: Mon, 07 Aug 2023 22:52:10 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b40013fc08badaa915223b2532e4806ea4ee6300de23109ab644fae1c233b532`  
		Last Modified: Mon, 07 Aug 2023 22:52:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33e51c3c9b0c60bc15e21a095b50ff28e4788a54471d7c190dea495ac4ecae4b`  
		Last Modified: Mon, 07 Aug 2023 22:52:11 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:976f500f6e981d649eecdb60e9428eefd2ac3c62f030270355c2765462ca10c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **760.1 KB (760130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fbae6fda28a162dad5ac1549e96eef2a93c753d33a63938095ef571d9c509f`

```dockerfile
```

-	Layers:
	-	`sha256:d9de2623c50396c1153802e0d495b19a7704e1e91ad876e3345c6fe63652de82`  
		Last Modified: Mon, 07 Aug 2023 22:52:08 GMT  
		Size: 701.5 KB (701530 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7923a34fec2daa9198c578fe7773cbb2265c17c2f8750db53c56cdda905ae8d2`  
		Last Modified: Mon, 07 Aug 2023 22:52:08 GMT  
		Size: 58.6 KB (58600 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:e4537be76f7e18c4300dc22648136fa3d94a727e29a4dd8583cd47d701f2e3f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65948181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8915eb9fffec0c49044d27b1d6289856718c71510f338e47e5f5a5b93a9671`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c966a9bf368223af1f01ec40bbda8236b09f8f7101735710e3a468fb84f8acff`  
		Last Modified: Wed, 02 Aug 2023 23:59:44 GMT  
		Size: 444.9 KB (444894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffa8b0c3d86d8ed198801ce646d6357c8bf5928077ffab8a4e7af28286f2a239`  
		Last Modified: Wed, 02 Aug 2023 23:59:44 GMT  
		Size: 10.1 KB (10138 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a22fd75ded1a3be57ff7bad37f49577c19301c4c68d0d34fa5e6b4567447e114`  
		Last Modified: Wed, 02 Aug 2023 23:59:47 GMT  
		Size: 43.2 MB (43190341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bec01c298369a3622abfc06ad1cd56c5c6f92027da0eb1151f4a6fc4ad89cd1b`  
		Last Modified: Wed, 02 Aug 2023 23:59:45 GMT  
		Size: 1.4 MB (1400202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b723b9fea82fb7c802d0fe85fab4b3dbbcbe9a58baab8c54952949b60828e206`  
		Last Modified: Wed, 02 Aug 2023 23:59:47 GMT  
		Size: 17.7 MB (17666904 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed1f70f871053000273344c1e47d476402bf7393b0da8eda36354e99b0d948d9`  
		Last Modified: Wed, 02 Aug 2023 23:59:46 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b62391dc86bdf85d0d423e88bcc457821cf011fdec43bd413e16f357549ad84b`  
		Last Modified: Wed, 02 Aug 2023 23:59:46 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ebaefa649bf38074df8daaa76ae365dbc8752f4c1d3c65b2f1893102a367cd4`  
		Last Modified: Wed, 02 Aug 2023 23:59:47 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fbd972877e1def3beb8e262194f88ebf5dd4f54758a420049ec647e38243646`  
		Last Modified: Wed, 02 Aug 2023 23:59:47 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:962225f003ed2c023cf04ce63dd1f0842309c3e2a0d044d11b11b59e35ddb810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.7 KB (58697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a088ff24d3a49c185630fca02608bdab907d54a719f2f7d9ee9ebb43d034b63`

```dockerfile
```

-	Layers:
	-	`sha256:d034eec0e2704c8f8655404e4d46be0030a254fd18006e5c9cd72b48c3912ee2`  
		Last Modified: Wed, 02 Aug 2023 23:59:44 GMT  
		Size: 58.7 KB (58697 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:cd88dc69cb61073a53ed7464305c2b42b069d8cd9a7e9ec381349daed0c80f80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67085443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a279c444f10728beca76b3884ea85748d373eef7c35c67b7f486a538536fc08e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dadd4d8af5ef0cba083200323660ffbe7c8fa18ea5bc1acda303087398169a43`  
		Last Modified: Mon, 31 Jul 2023 22:44:31 GMT  
		Size: 472.9 KB (472912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a564a0c39f638c098e9bc86921cabd26259ed5c70a849d83facb51f8de25d7c9`  
		Last Modified: Mon, 31 Jul 2023 22:44:31 GMT  
		Size: 10.1 KB (10138 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d5d430b26da52ead6060066f20f93428a0cc16d23937e85bdacb05a0773fca3`  
		Last Modified: Thu, 03 Aug 2023 00:21:47 GMT  
		Size: 44.1 MB (44069237 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4e7eb959642804031d4371fa6c8a459b13f0115233cdf5a92f9bf53439e0bd0a`  
		Last Modified: Thu, 03 Aug 2023 00:21:44 GMT  
		Size: 1.5 MB (1519682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a1be8dc1234d5666c0fad2c1d5fb5a43f211cafe6d1d81399062ccdf48dc0b`  
		Last Modified: Thu, 03 Aug 2023 00:21:45 GMT  
		Size: 17.7 MB (17666940 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3f679ff32a59ef24edb6405d9099fd21fbc18a6b59ac5f294f1eaf0ffcb5893`  
		Last Modified: Thu, 03 Aug 2023 00:21:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1c64a4e0dba94edf5933efd3a466eeaddab6a26495c4e071934f126f4b34375`  
		Last Modified: Thu, 03 Aug 2023 00:21:44 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:185797c659520cb10dba3d181957eb03b535b52bfdaf9b192a0fd25fb5417e72`  
		Last Modified: Thu, 03 Aug 2023 00:21:45 GMT  
		Size: 624.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1299b87e77360a5def9609d52c8bfcd8e53691baa1437c31e7e86aec9edcf73`  
		Last Modified: Thu, 03 Aug 2023 00:21:45 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:9280a5eb6944cc68dcde17803ed4bd68959de77b90a3dc3dc8c46941b0e594fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **754.8 KB (754848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8efaab8e239ab87340e0192949da577fd09913b0958c5cd0dad10b2a3891f65`

```dockerfile
```

-	Layers:
	-	`sha256:f99c21d2bfbc5ed879ba963576ff52231d501faa8789f261c842c714306d0242`  
		Last Modified: Thu, 03 Aug 2023 00:21:43 GMT  
		Size: 696.0 KB (695975 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f48f1807b618203954928eb0354d7a45e242f0e4726b5910c8cf1a0f9c0b2248`  
		Last Modified: Thu, 03 Aug 2023 00:21:43 GMT  
		Size: 58.9 KB (58873 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:51f2d1119bbad4779e5af9a9ad32e313c1bdc083fb2a2e1921bb1ef61e8b1ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64304436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b10e878399da7f5e62010061061237bbc71c812bde63176964ada80f49f752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 01 Aug 2023 00:34:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 00:34:19 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 01 Aug 2023 00:34:19 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 01 Aug 2023 00:34:19 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 01 Aug 2023 00:34:19 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 01 Aug 2023 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Aug 2023 00:34:19 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 01 Aug 2023 00:34:19 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d93c596e061d4f9ac700e44c2f92be627c02dbe8b9b358806c9c80515b2b401d`  
		Last Modified: Mon, 31 Jul 2023 22:17:10 GMT  
		Size: 428.1 KB (428051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9225ea301cff44a848bf80e89efffd36bc9101bf44728a398d4a5542d2314290`  
		Last Modified: Mon, 31 Jul 2023 22:17:10 GMT  
		Size: 10.1 KB (10133 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95ea0599cd0389673226bcb23a9cb05603a6df6b710939755f349d8c5dc4d010`  
		Last Modified: Thu, 03 Aug 2023 07:49:44 GMT  
		Size: 41.5 MB (41489075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a3cbf532823e7c297bdd153bd75951fcce724fc3ba20da7ad70c3528f7f9b43`  
		Last Modified: Thu, 03 Aug 2023 07:49:42 GMT  
		Size: 1.5 MB (1495026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0643ff9b3f00d278ce7b9d6d0bf58b089e7a1436d46173531c8b0acc527f4180`  
		Last Modified: Thu, 03 Aug 2023 07:49:43 GMT  
		Size: 17.7 MB (17666903 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:124815bda6ac610e1796954adba1b95fea1947cc72f937bf1812dba9297cc416`  
		Last Modified: Thu, 03 Aug 2023 07:49:42 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c35e3c3ea68ed732be8e00271aef99645adbf4e267d290760fd33186a89286d`  
		Last Modified: Thu, 03 Aug 2023 07:49:43 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:830f6f3f1754158cd209e4f7f3c4f247ff55ed7d532c07ce90af7871f2498d38`  
		Last Modified: Thu, 03 Aug 2023 07:49:43 GMT  
		Size: 619.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90083f6005f840e1a1c9ad926397cac63ee1f3ee92cfd2cb7f338476d1a753e3`  
		Last Modified: Thu, 03 Aug 2023 07:49:44 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:f750eba307a9211422f2df9c8c1b53578a490f26ddd803853512ff187e274f6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **754.7 KB (754733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0bed9577da5db9559665ab054df9f3aca34d5c4bf4969588ef61a5faefcb6e`

```dockerfile
```

-	Layers:
	-	`sha256:fd913cef8e4695751ec73f152af998b26baa18f385668b1bd169524b6abf145f`  
		Last Modified: Thu, 03 Aug 2023 07:49:42 GMT  
		Size: 695.9 KB (695922 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bfd93775d41840c8bca31e15117c607477f7fb0a94944d52c90b3da5861748a4`  
		Last Modified: Thu, 03 Aug 2023 07:49:42 GMT  
		Size: 58.8 KB (58811 bytes)  
		MIME: application/vnd.in-toto+json
