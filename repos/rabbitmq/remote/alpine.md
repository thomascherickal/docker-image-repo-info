## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:28580a859510121cf05d8865bf6a5d6c0b205e096ee55d85bfb7de7cf631a384
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 12
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `rabbitmq:alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:59516c96814bd1b09fcfd28cc93e67b91c3de8caa4e7f1c149e6b54eba3ee868
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74702860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a22e3292b5a97f22d7a12326618c7fcd689a1b288eee542d25ae095018a3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
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
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:383b5109dbe17afa2f045f5681891393eb7bd40ddb313bb0a5c9677527963618`  
		Last Modified: Thu, 27 Jul 2023 20:49:38 GMT  
		Size: 430.0 KB (430006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d49b812180ccb2e878d771097fa4e865a1418bc1e34dec6d5c33cc50a8d6d368`  
		Last Modified: Thu, 27 Jul 2023 20:49:38 GMT  
		Size: 10.1 KB (10142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:872b2aac00b8f1f722fc0fcdb7cafe55865c174d140ccc35c4d84e07799e36da`  
		Last Modified: Thu, 27 Jul 2023 21:00:39 GMT  
		Size: 50.9 MB (50899932 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd4a269fe80407246a71586f876c1c4897420b586af60c15c93d664df155e708`  
		Last Modified: Thu, 27 Jul 2023 21:00:37 GMT  
		Size: 2.3 MB (2296108 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aef228a18c0a78f1412f96a306a78c35463776369c48ed94b4ac3ea9337e5fe`  
		Last Modified: Thu, 27 Jul 2023 21:00:38 GMT  
		Size: 17.7 MB (17667047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7400e98bdc600df6d15d51f2064d54f027b96fedf17a8eda7eac2728bf60bdd5`  
		Last Modified: Thu, 27 Jul 2023 21:00:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46f99d07f2aa16029cf782cc3628bea196f325531bb75e7a2fdfbf228456074`  
		Last Modified: Thu, 27 Jul 2023 21:00:38 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1f5c2438bd971f994ad63c0ad25c8292d2c3f578a3d72ef488a160f3fe00711`  
		Last Modified: Thu, 27 Jul 2023 21:00:38 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:28d8414ca23d5f9ad0e0a8ee0d5154d43fb64d3a62fbf76e3f3cc67162293372`  
		Last Modified: Thu, 27 Jul 2023 21:00:39 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:8b95a4297f8602b5aef408dce262f8e6b8f61b776df84c66f200e83c7b60201c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **757.3 KB (757283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8c189c8b1fcb24c96b8aa778be6b16b8c1781574b2ea870855354c41fba09f7`

```dockerfile
```

-	Layers:
	-	`sha256:198ef7ffa540a00d700070f269cf7a59ba2e1f7cc6dcc040045f2e974506235f`  
		Last Modified: Thu, 27 Jul 2023 21:00:36 GMT  
		Size: 700.9 KB (700913 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d01cc398817a95f8ad8bba049edd83887c07ded946ae34c1a64cde11de00e01`  
		Last Modified: Thu, 27 Jul 2023 21:00:36 GMT  
		Size: 56.4 KB (56370 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; arm variant v6

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

### `rabbitmq:alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:46281b6127da12600d05dc0ec28e3810326926963e30ca678f8b6e9f8c069892
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63067235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6aea1a06ff914eddff008058efeee918722cacea3f3ec1f61cd56a2427809`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
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
	-	`sha256:0622a3815e56bd327f74abee88811dae42056f2bc231eb330df81e59ac08ae87`  
		Last Modified: Mon, 31 Jul 2023 22:35:32 GMT  
		Size: 40.8 MB (40801718 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6769a1a2956800502d144982f613687bb622edee1c2c1f34deb7694f66a5efb2`  
		Last Modified: Mon, 31 Jul 2023 22:35:30 GMT  
		Size: 1.3 MB (1298634 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:192e7765d9830b4c793f4ab4c55f6d78d5b21536643e42b3cd36d6aa67db822e`  
		Last Modified: Mon, 31 Jul 2023 22:35:31 GMT  
		Size: 17.7 MB (17666883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a67841aa483179e5158cd334b0f242b3eab8fd6907ec7a734f44e8721110e194`  
		Last Modified: Mon, 31 Jul 2023 22:35:30 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f9798c954b316996fb2ddac84449a1188daacce71e7783ca928bc4a6fcd181f`  
		Last Modified: Mon, 31 Jul 2023 22:35:31 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f121866ec48840e1db8ba8b7433e6e033fe07e228fe5e38edebac4e2a331f09e`  
		Last Modified: Mon, 31 Jul 2023 22:35:32 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2eb3daacbbc6f6269ab522b1fe1d418296a38facc01907e459d43ae4a3b1cd8`  
		Last Modified: Mon, 31 Jul 2023 22:35:32 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:e0dcfc74d65d0f208c6926a9447fa14662ab116fd55492b535ea98fa1e372c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **754.1 KB (754060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cacb8df1774a5501ec907d1a2ed9de2766588ca33e5937b7a5eb1970eccc8831`

```dockerfile
```

-	Layers:
	-	`sha256:1a5e1528767b761e37e6fb5898be794dc579bff3ded03f47e77081ac10a2a8a0`  
		Last Modified: Mon, 31 Jul 2023 22:35:29 GMT  
		Size: 697.5 KB (697451 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13c64cf9c354d7055b51b09ff39e7468acceda0cb716972ef44819eb553a8c49`  
		Last Modified: Mon, 31 Jul 2023 22:35:29 GMT  
		Size: 56.6 KB (56609 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:73378d39f04b964a211d260d3b03aae43fee7025310cb6ff32fa165226020fa9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71764091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa86f1e7e25153a96bc5a69168f0dff3e4a34daf8e80dd9e3248febba2f1d79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
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
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:558d039804e9d95930e03e5abb347a45a0d8119b16d72a5741d4dba674fec71e`  
		Last Modified: Mon, 31 Jul 2023 18:39:41 GMT  
		Size: 408.9 KB (408875 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4c4f95267685b63ababa8bf04dda04e7ccf3da0fa3d4e9aedb7149c8906b5d`  
		Last Modified: Mon, 31 Jul 2023 18:39:41 GMT  
		Size: 10.1 KB (10141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:462007742cc242a4fba75affb4b6b2bd85e4b117765781462281f108c192971a`  
		Last Modified: Mon, 31 Jul 2023 19:35:36 GMT  
		Size: 48.0 MB (47978790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea9480d3c144031817b0a942512733411c284c1fe198f51d30c531bd6691c16e`  
		Last Modified: Mon, 31 Jul 2023 19:35:34 GMT  
		Size: 2.4 MB (2368256 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f37aa36f8307d9f3ec7e2b59d170bf27c3a7901f5e480be25d687299d279b3c5`  
		Last Modified: Mon, 31 Jul 2023 19:35:35 GMT  
		Size: 17.7 MB (17667036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a44509be359f06456e7a3229e98ab6c6a03c44df400861f9fa0f368882a8235`  
		Last Modified: Mon, 31 Jul 2023 19:35:34 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ef88c631e03e3478a1e6e280e8dae315db0209164576f0cddf2aa46130ee7fa`  
		Last Modified: Mon, 31 Jul 2023 19:35:35 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a179412a57434eaefdc64bd35d24f570eb1853e843b353733c12f16a8c50122`  
		Last Modified: Mon, 31 Jul 2023 19:35:35 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1686fe9344e27ff99c1f92f804c884f7f4f5e4671f826b61b88a6693c56aa6ef`  
		Last Modified: Mon, 31 Jul 2023 19:35:36 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:30e4b4bf2ebca9cc9bceddb51d9623a9f2f1217ebb0105be446784f8c8d7bbd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **757.3 KB (757307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e730b0e3428d6311b77c2c55134d5a546e4359d782a8cea6d1bcc5de130a0a2`

```dockerfile
```

-	Layers:
	-	`sha256:e124d09963a5e319a8551aad9bb28086fd48ba364acf68d9fe0f913835633167`  
		Last Modified: Mon, 31 Jul 2023 19:35:33 GMT  
		Size: 700.9 KB (700928 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fc81b6703406bfa028e080fb81bc950b2848a47f7baf86cfb0b1ad03660399de`  
		Last Modified: Mon, 31 Jul 2023 19:35:33 GMT  
		Size: 56.4 KB (56379 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:714a882a33b7aa74794e1e3894264b0ef9921a363e532d946f08c88644120958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65946238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7a350d8c5f23089a84686e9d55646d9140b696026193cf2119fed42d5130e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
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
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f27759d81bd27392c3f1f738c525acbc8518bd641746bf33360314ee30f327`  
		Last Modified: Thu, 29 Jun 2023 22:46:32 GMT  
		Size: 444.9 KB (444892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb47200c56702b8a62ea5b4b50ae6e40e6e58e3a1a48aea66fd6365f8c222d9`  
		Last Modified: Thu, 29 Jun 2023 22:46:31 GMT  
		Size: 10.2 KB (10168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b95ae51cafc9b9d15085a48cd9118d1430e755409f0da8c960af25f2b19701`  
		Last Modified: Tue, 18 Jul 2023 19:49:06 GMT  
		Size: 43.2 MB (43188056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8abed873900b0a65b17614e68352b7047a3c84bfaeef8c87c6cfa60772d95f`  
		Last Modified: Tue, 18 Jul 2023 19:49:01 GMT  
		Size: 1.4 MB (1400160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044d82153e885b47fdf3d870d1e0175fc43c16c902befc53c4d27705a73a7e1d`  
		Last Modified: Tue, 18 Jul 2023 19:49:00 GMT  
		Size: 17.7 MB (17667231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486929caae415055f849bb6a0c1f6573d330c8c4377d44d05526060ed7da0a65`  
		Last Modified: Tue, 18 Jul 2023 19:48:58 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7be4c3393c8d0295d508cd2e8aafefa7cb1d3ee7114584768e79e129441ab`  
		Last Modified: Tue, 18 Jul 2023 19:48:58 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865950e2c4f78dbdadbf9710a6cc569edfd12da07e1bc1ad4d4c98a5eefc128a`  
		Last Modified: Tue, 18 Jul 2023 19:48:58 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023447bfaf90434bba55797d1b1128a99293c5fe4ef645f45c62fc84d22b25b`  
		Last Modified: Tue, 18 Jul 2023 19:48:58 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:5802e167287c91631fa70f7df558432bd6180ba5306315c64ff337a181ecec6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67086061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58abba5d863330df1631e330a6d6fddddca6496faceda213ebe9f7fa7525670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
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
	-	`sha256:49da224592310c93e0a56180d4daa11db13d8818e3e520326f3ef6267fb68cf9`  
		Last Modified: Mon, 31 Jul 2023 22:58:49 GMT  
		Size: 44.1 MB (44069902 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37bd55117ebbe42fca08536c562304ab219a8f07a91888a0efb59dcc4f637246`  
		Last Modified: Mon, 31 Jul 2023 22:58:47 GMT  
		Size: 1.5 MB (1519662 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c4a5443ff42eae9376d86cc35f707e2df8b1682b24ec1aa81889f72af70f018`  
		Last Modified: Mon, 31 Jul 2023 22:58:48 GMT  
		Size: 17.7 MB (17666915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:717d0ff5d9161e5ba88c98f5f7a229b4d6faa507727b621fce03cb5e1a28de27`  
		Last Modified: Mon, 31 Jul 2023 22:58:46 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29d344692d8a4714b221f60f32f040b1ae4994149529d9b749200c71332b27e9`  
		Last Modified: Mon, 31 Jul 2023 22:58:48 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72527ba4b1f19282195fdb5ca46af511a8fcb6bdd647a3cb867cdd4e695a5789`  
		Last Modified: Mon, 31 Jul 2023 22:58:48 GMT  
		Size: 622.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3bb5d4507a2f670c69687db8c04ce515aaf9f6db04020fe98a4dd01a8432e8a`  
		Last Modified: Mon, 31 Jul 2023 22:58:49 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:436a0b3201f1eb22f5cdd48331b009e72ea7f7f89f68aaf30c87a0c3a699feae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **752.4 KB (752408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4b073cc013073d2024ad5fafe799a0f2ebeb78432e682cd50457ae648de640a`

```dockerfile
```

-	Layers:
	-	`sha256:559737561a560baece8a0873bce7dddfadd24f426a195a0e72b705f25b69ec8e`  
		Last Modified: Mon, 31 Jul 2023 22:58:46 GMT  
		Size: 696.0 KB (695975 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9790fe368c4be3237b21723e3003076a2324c0d2f9d00ea0426d83a3a16eb5d4`  
		Last Modified: Mon, 31 Jul 2023 22:58:46 GMT  
		Size: 56.4 KB (56433 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:0f3753f5e7b0963a356c8f64d090cc337864797909e5cd3e50916fbed0f48dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64302252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3046506351be186f4d14d1406276304c59c62a104b67df999e833a41ebb9251`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
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
	-	`sha256:e657238bae9fc39ae38f1201598d8e348df234b6fa4f8b716429ff7ceb28e1cf`  
		Last Modified: Mon, 31 Jul 2023 22:17:13 GMT  
		Size: 41.5 MB (41486892 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e70453ac7355c10e5fd699b798189d099d45e96a33809632b75bbb54c0e1389d`  
		Last Modified: Mon, 31 Jul 2023 22:17:11 GMT  
		Size: 1.5 MB (1495018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55411a8da741e391d1a5b90aea7774e28323916b391705b92dea434400bec7f1`  
		Last Modified: Mon, 31 Jul 2023 22:17:12 GMT  
		Size: 17.7 MB (17666914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be99905707fa2a501bccfa3f9961d79a145a3a7b1fd9c50285be940650b1793c`  
		Last Modified: Mon, 31 Jul 2023 22:17:11 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:099c3210927747a5e3a53bc80df71a560d244e95b47c021fd7969dd5b3bf21f0`  
		Last Modified: Mon, 31 Jul 2023 22:17:12 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87943b3c048b715e9756a159bafa5f10faaede28f42349f9bea19295bf21214a`  
		Last Modified: Mon, 31 Jul 2023 22:17:12 GMT  
		Size: 616.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:647075f9175d30a30465e80d68f5b016757496bd46bb71aef381b065bfc0c800`  
		Last Modified: Mon, 31 Jul 2023 22:17:13 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:437f1ebee14933546b6d8547c352f773cf95071a383817416d7a7a9fb34590ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **752.3 KB (752292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab5adeb90fdb46983b2e6ea8707f0427ccf4d14406b978836d7175ae5353d31`

```dockerfile
```

-	Layers:
	-	`sha256:6482c6023a4a1f90844e6611df5de105f911c0675a64c67431858c6b6a89d263`  
		Last Modified: Mon, 31 Jul 2023 22:17:10 GMT  
		Size: 695.9 KB (695922 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5307545ea19ad47aa4cc483d94bd931cec3551c421c008c3e55a2624aab1bae4`  
		Last Modified: Mon, 31 Jul 2023 22:17:10 GMT  
		Size: 56.4 KB (56370 bytes)  
		MIME: application/vnd.in-toto+json
