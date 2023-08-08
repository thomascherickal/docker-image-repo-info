## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:4d6c584f3dea0deae7c598957efe9ee568d12b57dd350931b2579b7e351faf22
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

### `rabbitmq:management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:88d0b1dcbd0cb7474f368e0cec138b9c8a45b4195a2ae4c2dc58c51b6a9c0555
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.8 MB (89779104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c81f4a0a0c0873223f86c1c3476549aa5dc31f4f89a58ddf57ab6aa7a2209`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
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
	-	`sha256:472f2532bef70564c69a0a7715b35c3cfe6ae8dfd294ae1bedb0992c7206f622`  
		Last Modified: Thu, 03 Aug 2023 01:51:18 GMT  
		Size: 15.1 MB (15073947 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:eb6d7db2f60819600850794b3d439c071b198c110719923d0e950b9d6a3c27ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0324eb9af3c04433e90d78119c969d29bf7b3ee3daf4c756eba276bc723dc758`

```dockerfile
```

-	Layers:
	-	`sha256:fae22cad72d0cf0c79b80db68993f093241b369667f58abaf3ec07dc74282df4`  
		Last Modified: Thu, 03 Aug 2023 01:51:17 GMT  
		Size: 1.4 MB (1440205 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e0749e7df5ad8ff899202dc37056904a85d24f9b99871783fb5de44adb51f0af`  
		Last Modified: Thu, 03 Aug 2023 01:51:17 GMT  
		Size: 12.9 KB (12887 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:6e928601319c2e38e26704ff013c550e5d80c6cfa491d80edecc44fb3c2aefae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.6 MB (79615918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30dbda73c3173f85d55d1390dfb22e8103eb90d12b6e87c5220bfc8fe8298e51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:b714e2a9538b807f63bbe8d11163842658fdb11ad099efd0f7c1c715c8447616`  
		Last Modified: Mon, 31 Jul 2023 22:51:23 GMT  
		Size: 15.6 MB (15607116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c7b6df04c02abe78f8374d1a217d991612348a06c836de1af4d099f4d25c9e13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78285478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dfc0a205fc0db35dc41c945b790618227f820624d19861dee34c3ccd597530`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:3a1446da9716e9b9ebc836f1463b7f996fe186d9a3bae0a0122a56785c96430f`  
		Last Modified: Thu, 03 Aug 2023 00:55:40 GMT  
		Size: 15.2 MB (15217151 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:a285edfc93fc1019ac7f94e452e79dabbd278e387965df82cb23f9822dca9294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5c3d733a87f4fae5624bf257a7a367c13925813c244e4c92bc3daef93fa8e9`

```dockerfile
```

-	Layers:
	-	`sha256:669e736ce88cdc1d452aa3fcf0f616a0f76a85b4593aebee04a5df6683b19dd3`  
		Last Modified: Thu, 03 Aug 2023 00:55:39 GMT  
		Size: 1.4 MB (1440423 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:74a10bedcb6012eef7ad831d1701875a528c22b7dd080219bf540f5edd0e5378`  
		Last Modified: Thu, 03 Aug 2023 00:55:39 GMT  
		Size: 13.0 KB (12981 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:052cc2c777a56d45df504538b3c76e35113fdfb4ef46c481c5342f725bd09720
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86990422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0819e5f8c4721e8845b4d16363073d25e3d17ace95b80face404189eddf3cdba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:0f8bee0999c4199fe6f21c5c80ec4c6d62a7ca382bdc7b30ff6b6b11136933ff`  
		Last Modified: Tue, 08 Aug 2023 00:17:27 GMT  
		Size: 15.2 MB (15223677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:46d7119fa4610aa79dae42e3218a0341022d0f33068e8370b2d093d7fef97043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8279888314b137aec0ea6f33442669891367ec13f1a65aee656e36c89a4cd38b`

```dockerfile
```

-	Layers:
	-	`sha256:e2439c6ea62565d106e00c9b870554b8505d8d09d19fc591afe61c5a27f5adbc`  
		Last Modified: Tue, 08 Aug 2023 00:17:27 GMT  
		Size: 1.4 MB (1440328 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13787427a8a21602f4e9788ecc6807721c2d427c00c7d1bd8c5e795be2216f1e`  
		Last Modified: Tue, 08 Aug 2023 00:17:25 GMT  
		Size: 12.9 KB (12945 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:ed9690790afb91723460a8dcdc19dad7fadb98d0970a45e1c62b6af1354fb614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82191140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cceec0c12dd63471a7ff9c9388ea0eea924da2f880208fbffbcccf9bad0fa2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:bab36a150c6a0ab4da9754a5ac77f10d4e4b82f60b091e1e06ae8f878842c7ad`  
		Last Modified: Thu, 03 Aug 2023 00:52:00 GMT  
		Size: 16.2 MB (16242959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:15a3c9ec01419eb84f4ecff544c50153df051d2639fc7ccbb76515faf76ddf8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 KB (12630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3fa106c9acb5538358842a22a1bcbaf26ad7de72dd090c94beb296b9d48085`

```dockerfile
```

-	Layers:
	-	`sha256:21ba0a139c32edce8cc322b926a9f40867f1b03904ce449d0b03011b7be6a84a`  
		Last Modified: Thu, 03 Aug 2023 00:51:58 GMT  
		Size: 12.6 KB (12630 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:4c4cb036577571ebeded27d106b5db1da72791c71e526c5b0738e200a2adde85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83381191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a90bebcdf50ace85d6055fef5c5288b56e41ea7497fd5b7371a65cd8b862c24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:2bad935fd7cba84e2513e0be60439568c4248d5966f01b3370f2cac1835147ca`  
		Last Modified: Tue, 08 Aug 2023 02:52:44 GMT  
		Size: 16.3 MB (16293984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:b9ae3f29cca011511d5be6a12e24538a2cd8481fc68d21e1c287d33f3dd6133c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1451125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:330c8475a2be96feb2e9c9ca0554d345260b5f0e20e19210449a90ed2e50ecda`

```dockerfile
```

-	Layers:
	-	`sha256:be2b4cd55bc0ef79ce2de3675d11fa08e1cadcb7574e2902d2a8bd56b4901afe`  
		Last Modified: Tue, 08 Aug 2023 02:52:43 GMT  
		Size: 1.4 MB (1438153 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68488540afaab00389857da9efbac3520742502aadf293161c44afca61fd6d75`  
		Last Modified: Tue, 08 Aug 2023 02:52:42 GMT  
		Size: 13.0 KB (12972 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:11c0bac9b683fa873f26c3dcd19232dd572b02761a653225b66df83f61af8a58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80406079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8786172ca91961e5dd27d5173571e59fd4e37df9785f6215bd87b163bf05f7ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.2
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Fri, 02 Jun 2023 21:59:28 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["rabbitmq-server"]
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
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
	-	`sha256:33352909cc07b666c994370c4d33382b634e45ca32d0dcfb0f9916d40966c166`  
		Last Modified: Tue, 08 Aug 2023 06:06:34 GMT  
		Size: 16.1 MB (16100984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:d160902c57cfe27c3b7731544a23c0ce4249986dbe949c1dd6c481ed0402a517
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1451134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f970aa8765a736c58bc241943b4c93018757a72dd0f1e61e2f40d64a0015b1c3`

```dockerfile
```

-	Layers:
	-	`sha256:408ef07254e94b9fa935251eb349708ce822d38f6745d3e29a22b2341fcb985b`  
		Last Modified: Tue, 08 Aug 2023 06:06:32 GMT  
		Size: 1.4 MB (1438206 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b657c07185a0808a87cbb348d9e42af8767932b801535f0c988a588cf054fb6d`  
		Last Modified: Tue, 08 Aug 2023 06:06:32 GMT  
		Size: 12.9 KB (12928 bytes)  
		MIME: application/vnd.in-toto+json
