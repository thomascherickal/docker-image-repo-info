## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:436036f28881769832f0957acbef68a0340c8ef82c139fa3df86bb8c164d2f18
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
$ docker pull rabbitmq@sha256:3a6a83582fc23717558f7cc53b2002a916ff53abe45ec4aa2253dafe834c4a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74723790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc4d2203b48161c4437b2e1c700502caad90d8809b8cc78d9479b3ff0b9d329`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 08 Aug 2023 16:59:29 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 08 Aug 2023 16:59:29 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 08 Aug 2023 16:59:29 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0a34b3b70846851711b57de25146c70825bff8059524e525da2c3a1699bf272`  
		Last Modified: Wed, 09 Aug 2023 01:35:34 GMT  
		Size: 430.3 KB (430255 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91d336130f18d1481ecce79d7b907e56f2c92f19369afb226b09cb921e19c926`  
		Last Modified: Wed, 09 Aug 2023 01:35:34 GMT  
		Size: 10.1 KB (10144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c34b7b67f8d2bc13f7ed584d5af25d4d808a074a179baa4042d2ac8040feda8d`  
		Last Modified: Wed, 09 Aug 2023 01:35:36 GMT  
		Size: 50.9 MB (50916907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d762e6ffc176a6f0e5ab15cde735b919ac9de184cdde60a5ea652e52beacd1d`  
		Last Modified: Wed, 09 Aug 2023 01:35:34 GMT  
		Size: 2.3 MB (2296088 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a24b1b2468d7e09267f5ad5891c45cc8fc7eeb536c3524e8ac7485d63015890`  
		Last Modified: Wed, 09 Aug 2023 01:35:36 GMT  
		Size: 17.7 MB (17667033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b9356b2f6ad4b5aaf785aa62f23826dc211152f4b863c5c044682b2eaa27fc9e`  
		Last Modified: Wed, 09 Aug 2023 01:35:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ee44198571e946e4564ba02a011433da0d9859ff350ebe59d9225284265f21c`  
		Last Modified: Wed, 09 Aug 2023 01:35:36 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3adf699bb496c07e05274fead3dd4a77ae94d6d482c245fcf588f04da1a96541`  
		Last Modified: Wed, 09 Aug 2023 01:35:36 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:347cd6a8cfca2b42580f31ef0a0e0ab237cc5f151d77b5828d5f7b3d462d7b25`  
		Last Modified: Wed, 09 Aug 2023 01:35:36 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:c96e1743f2355ee7fa6e64f27041a113b49bdad5dfb121373cbbe8b5dfdfbad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **760.5 KB (760542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cdabbb7c0693955357b48d51c828fcdade3b654a48a4241b5d21a4ed81ee83`

```dockerfile
```

-	Layers:
	-	`sha256:7ec347343018fcf43ea41aae3e2824d6ca776bdd4352def378dd2622ee949605`  
		Last Modified: Wed, 09 Aug 2023 01:35:34 GMT  
		Size: 701.5 KB (701508 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5d3c81ae0363fc76654a760c467741362c81c87cd974fc1b0dfc0284c4d7d94e`  
		Last Modified: Wed, 09 Aug 2023 01:35:34 GMT  
		Size: 59.0 KB (59034 bytes)  
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
$ docker pull rabbitmq@sha256:dbc6a645ee6516d33e028d090d0844ce08befbf68481588f2c9bebc9ee675c53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63073577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afca2ab78b7c3b68baf5dd3986d330a2eb91ff0a89bff0cc5c5113fdf78c4408`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 08 Aug 2023 16:59:29 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 08 Aug 2023 16:59:29 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 08 Aug 2023 16:59:29 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:170a7d6afd79205115eb6352e8cdc69b32b83c16b38117d824a45a709cfb7c88`  
		Last Modified: Wed, 09 Aug 2023 01:12:53 GMT  
		Size: 390.0 KB (389991 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eed440a1b3d9ccc752805ebd2f70b123778714929fba871514c035a75a88883e`  
		Last Modified: Wed, 09 Aug 2023 01:12:52 GMT  
		Size: 10.1 KB (10141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c18bc4bdbf70f86c361da5414bdeec5a836df0457df5abdd53a11a47e7398729`  
		Last Modified: Wed, 09 Aug 2023 03:10:08 GMT  
		Size: 40.8 MB (40806738 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4d36c591a33dca0bff9fde8ee9d459ee300a86dbc4cf00e24b08f87582a39f8`  
		Last Modified: Wed, 09 Aug 2023 03:10:04 GMT  
		Size: 1.3 MB (1298577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e10fc27b41f1d15aafc7e12135a4e09b13d7a990a9f546d10b0495ef504d4e26`  
		Last Modified: Wed, 09 Aug 2023 03:10:05 GMT  
		Size: 17.7 MB (17666907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c5a22d001f004a3cc383e416ddc19d8eeeb70f3f76d011b198c07ab1952b36`  
		Last Modified: Wed, 09 Aug 2023 03:10:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50ccfcbe2934a118c57b1eaf5de8b9ef5d942e2cd66d69a7180826bea45e36a7`  
		Last Modified: Wed, 09 Aug 2023 03:10:05 GMT  
		Size: 106.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:008f017c42dfda00bc3f97e955c217ad59a667114d5665cc968a29ef0c06634e`  
		Last Modified: Wed, 09 Aug 2023 03:10:05 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:deec9b2bc252d481a7c7da7ebbcc726f52b6f68696b50f3fbd80c21aeb1b2a38`  
		Last Modified: Wed, 09 Aug 2023 03:10:07 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:e4489f644efcd0a8c62a12f720bddf28dd07e481ef7cc64e8d5af238c60d9d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **756.5 KB (756473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d98518d0db45fa35cd62203032e5ba0704c5165ec21d4442b7030ae1379b74`

```dockerfile
```

-	Layers:
	-	`sha256:e4a0d073189922c7269b70bdcd4e952e49b1f23cba7cd98ac96c5f152fd6a31c`  
		Last Modified: Wed, 09 Aug 2023 03:10:04 GMT  
		Size: 697.4 KB (697431 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fe93c4ad397175c87e51eb412995cdf914ce6e9dc80cec94f08e8fb82dbfaa04`  
		Last Modified: Wed, 09 Aug 2023 03:10:04 GMT  
		Size: 59.0 KB (59042 bytes)  
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
$ docker pull rabbitmq@sha256:585eb6288a4a6d9ab64449b813b6689e6acb2a1e4810962e8d6be12d0fd60968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65955464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2c86164f76fc6e3adf0fc58a12176e8eb8ab65568f741d6ed527b8af83639b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_VERSION=3.12.2
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 08 Aug 2023 16:59:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 16:59:29 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 08 Aug 2023 16:59:29 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 08 Aug 2023 16:59:29 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 08 Aug 2023 16:59:29 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 08 Aug 2023 16:59:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 16:59:29 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 08 Aug 2023 16:59:29 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e10eefffd51b7e0bff1ff7b3f35e3e6cb34a07f403d2c79b3f80eb76380b4e8`  
		Last Modified: Wed, 09 Aug 2023 01:36:58 GMT  
		Size: 445.2 KB (445177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011fe6e6864f4d686d95ba3256bb2981197b857cb93e2ebd59fa05124431c35b`  
		Last Modified: Wed, 09 Aug 2023 01:36:58 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a80641f4f1c64871b6b4feec7bb9c0ce16a00affcf474c7adf8960cd1ba1cc24`  
		Last Modified: Wed, 09 Aug 2023 01:37:01 GMT  
		Size: 43.2 MB (43196127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767ef00c328484138a476891b85be2415c14a42efd0d9b1fc45b2d97796891c5`  
		Last Modified: Wed, 09 Aug 2023 01:36:59 GMT  
		Size: 1.4 MB (1400209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:580dffb32625ad14327291d58457d3281ddabaedf31c1b855326634ed395fd6b`  
		Last Modified: Wed, 09 Aug 2023 01:37:01 GMT  
		Size: 17.7 MB (17666917 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:022e868f340ac2d0cc4e6eb25c5df32ad4c559f43b64b399a81cd38757a32ecd`  
		Last Modified: Wed, 09 Aug 2023 01:36:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:580314be15504534241db68c6e321692708f93901775ecedd5d204f96c1edf2a`  
		Last Modified: Wed, 09 Aug 2023 01:37:01 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b82b8e2d490722c1812bb83455ef24706117b56eb8fdf543eebab8466ddcea51`  
		Last Modified: Wed, 09 Aug 2023 01:37:00 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c7914283782e13a70c3cb85968212220448ea7a0e95647dfe0d546e3faf6c29`  
		Last Modified: Wed, 09 Aug 2023 01:37:01 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:94e0944e55a56652db689a8c5a1d151931257295ebc9855577aa1ad709211580
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 KB (58764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d27dd50942799d9e704e6c81d2fe54f65ea26cc20ff54c535ada5d06ccd05bf2`

```dockerfile
```

-	Layers:
	-	`sha256:5ff33c0102e1a0cf9f7e4ef60d871e0d1b95480c15c36dfa25a9e69dc4308ec4`  
		Last Modified: Wed, 09 Aug 2023 01:36:58 GMT  
		Size: 58.8 KB (58764 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:5728052a28d4cd20bfceccd748f6d905f993d9b27e18d4ea8e7b1c8e28f73156
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67087207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bff059f81ffa8363b2a71bd711930f9cfc7cfa13e71a6f6a55434a8445e67e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 01 Aug 2023 00:34:19 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
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
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbd1f3cac2030a6026dfac943f2ef1128b3e71bf1cd303a7c51c168fdd0743b8`  
		Last Modified: Tue, 08 Aug 2023 01:59:18 GMT  
		Size: 472.9 KB (472913 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbe42809c3b8a42e8b786ec41cf2a4917f8acab788667e0b0a287e64b2e4c815`  
		Last Modified: Tue, 08 Aug 2023 01:59:18 GMT  
		Size: 10.1 KB (10141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7310b5ca55033bca90b29b4eeeac315171f7affce74ce5b6454a45ce91e4b963`  
		Last Modified: Tue, 08 Aug 2023 02:09:15 GMT  
		Size: 44.1 MB (44069555 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ce57d84652b5c4ab8bc25f2800690dbdbdc359654b9ff46b231db793d439f64`  
		Last Modified: Tue, 08 Aug 2023 02:09:12 GMT  
		Size: 1.5 MB (1519685 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9cc39856e69026666eca23ee3ebe1a91b8e05d3640f11965dc6d01847ad95e35`  
		Last Modified: Tue, 08 Aug 2023 02:09:13 GMT  
		Size: 17.7 MB (17666900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ade89b64839aa5b2bc6bf8b238b8ab9a7500db37b479788da258db83c77bad0a`  
		Last Modified: Tue, 08 Aug 2023 02:09:12 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6833111613fbcc68f0da9efa76c0da41c6914069a6a418db94b6b3525e33b13d`  
		Last Modified: Tue, 08 Aug 2023 02:09:13 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73c32afe97cc486632c47e0d481ebafb499f40da33dc48416c933129776da7ec`  
		Last Modified: Tue, 08 Aug 2023 02:09:14 GMT  
		Size: 629.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc074c32db223ea6369c22476d6e2ce7d5815607ddbcc60b4779b044c016ed91`  
		Last Modified: Tue, 08 Aug 2023 02:09:15 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:372f0f64b32959bf157464b9d06696612d0d5fc35842d0099cd44f16cb95520b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **754.6 KB (754621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4ccdb6bbcbdbe05d31dddd95e88799f1b9e4ca585389d0650ce6bd81668b11`

```dockerfile
```

-	Layers:
	-	`sha256:0cd041fe8d703b308263211a343bd6c779b2ada4578b4c4777bbc690777831a9`  
		Last Modified: Tue, 08 Aug 2023 02:09:11 GMT  
		Size: 696.0 KB (695977 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:54d6f4c9e623b595e843c29b483694d81656a6a835f8105e40529b7a1a77b44f`  
		Last Modified: Tue, 08 Aug 2023 02:09:11 GMT  
		Size: 58.6 KB (58644 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:bf85c3949b1df7f93bd0659706cdcc98ffabadf967b9aad46e9d919c5ca32f6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64305095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5074e2f39a399133665feda5167a4daa1a7edac3d055faee481b96ab4da9f2df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 01 Aug 2023 00:34:19 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
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
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2979bafb03100523bf0dc5df470035e1f5eb05b30e515e5faab7ae33194f18d0`  
		Last Modified: Tue, 08 Aug 2023 05:36:11 GMT  
		Size: 428.0 KB (428049 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd115be0b29328708a268fe1876f9a421983ae0801548e0a5635d43687599ff`  
		Last Modified: Tue, 08 Aug 2023 05:36:11 GMT  
		Size: 10.1 KB (10132 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72b6999023524ae0430cbe64380815503438784e93d9fa625fb7f06dc82923b2`  
		Last Modified: Tue, 08 Aug 2023 05:40:12 GMT  
		Size: 41.5 MB (41489111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:925538e532103297be48c19de4c7e85d408faf60b319cd08520f3168e668282a`  
		Last Modified: Tue, 08 Aug 2023 05:40:11 GMT  
		Size: 1.5 MB (1494995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70200aa72540929e9c5611888b56ad2df8d6117c07598523004afabb0339afaa`  
		Last Modified: Tue, 08 Aug 2023 05:40:14 GMT  
		Size: 17.7 MB (17666858 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81520a3cde0c3bd06a4b6c762ae735781359e27c5298650f0d00671b177e54e0`  
		Last Modified: Tue, 08 Aug 2023 05:40:11 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:551b5ea15e8f52bf65af976b316d41b68980c0741854084a147bfb61f02a54b8`  
		Last Modified: Tue, 08 Aug 2023 05:40:12 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:daea90846a9e8485f9be110f10eac08e2f78ec97877b84698c0e455f928bddf2`  
		Last Modified: Tue, 08 Aug 2023 05:40:12 GMT  
		Size: 621.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:905a509068a52f5bced568d659ba737cf4a23faad5d92b6a5581b752c100d972`  
		Last Modified: Tue, 08 Aug 2023 05:40:12 GMT  
		Size: 832.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:49878ef6caaf5574f1526cc3ffbcffa9b267e2a090acca5aa29ceb2345cf4bcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **754.5 KB (754499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c3dfb32c6462931f2531a42a43f86020d0a536c69463cbe6d01a5caa034241`

```dockerfile
```

-	Layers:
	-	`sha256:cf9bf595425758676345274450684c6fdb0ce6cd116f31635fabea2907781200`  
		Last Modified: Tue, 08 Aug 2023 05:40:11 GMT  
		Size: 695.9 KB (695910 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5b9559ec8f3b9e4000a4ece61fab24912e53d1da584dd9201847007ddc0c673b`  
		Last Modified: Tue, 08 Aug 2023 05:40:10 GMT  
		Size: 58.6 KB (58589 bytes)  
		MIME: application/vnd.in-toto+json
