## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:dc50fb7c766c9c9c11f8cd1cd05ce2c3960b2c0d7bffe9cce3b3d7e581543fe6
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

### `rabbitmq:3-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:150c113ab9ecb7dd7697bd3688728023d8746305d1325cb3830bd5be00892d9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.8 MB (89797788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a1339b045bdce8dbd7f1c99ec68dfe4b4b2b90527c3735f5a656d9ad08814f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
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
	-	`sha256:55e8d0409cc5c3b684c045109f4eb8d1c674dec84035d8b0b7beaa2edd3b3b3b`  
		Last Modified: Wed, 09 Aug 2023 02:16:58 GMT  
		Size: 15.1 MB (15073998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:4c9f2002b90b40dfab3200b2e898cc880df1f6de5574760afae6f21f7b1c70b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f945e1bb96c4ede0cb05b2257abdd2099c5b09c8779e07c0cd8c3e7bd277d24`

```dockerfile
```

-	Layers:
	-	`sha256:c09680e89986d3bd86476763269b730ddaaa4fdb725cd83b5cff2e17c747ca51`  
		Last Modified: Wed, 09 Aug 2023 02:16:57 GMT  
		Size: 1.4 MB (1440205 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:16d7a76b37a0063b226f385f618bb5f7047cc406417b1b3c896155d78fc4543d`  
		Last Modified: Wed, 09 Aug 2023 02:16:57 GMT  
		Size: 12.9 KB (12911 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-management-alpine` - linux; arm variant v6

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

### `rabbitmq:3-management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:37da1f22da6a979c78dbd22ed4bd9849a6688ac1f6c99c76975e4f6432b372e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78290844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45244d7f8a46a4c90152b23dbd70ca4b7f30f4393fca55ea568afc20b149779b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
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
	-	`sha256:1894c38afb47a6ab2e98b757542d362d7ad7377b77ce65645f6aad4a90cb9410`  
		Last Modified: Wed, 09 Aug 2023 04:14:37 GMT  
		Size: 15.2 MB (15217267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:77f733890d5418c55d6f3d129b75f0449c679e3be948d05a6b63fb87b7cc3b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be46f8a0c73bc95fce66c0c5847b6bf3905f90139521bdbecb73a760b8c8cd42`

```dockerfile
```

-	Layers:
	-	`sha256:d16cd5bdb32cd16272bed8c72a95739b8d91ea642b50b7fbc22ff1a8762724a2`  
		Last Modified: Wed, 09 Aug 2023 04:14:35 GMT  
		Size: 1.4 MB (1440392 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1f65fd9a8bec98a86e8916bbe2da812fe1b43676a9a9fec27510bc09208f5b00`  
		Last Modified: Wed, 09 Aug 2023 04:14:36 GMT  
		Size: 13.0 KB (13005 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:8a36788fe57425c12717b029d71b5ad930b1d7f01445783bc2700064b46842b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86996811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f1d2a97eb5c59c7523d1d51f91a89cc5790cbbf982426fc7bd7bdc75e700b2`
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
	-	`sha256:667f55f8875b6436bbfba6fc0cb1d76fd37b98f19217e63a4db031998ba82538`  
		Last Modified: Wed, 09 Aug 2023 10:35:58 GMT  
		Size: 409.3 KB (409331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d831351cd1ccd83812fbe61759255cbafccb9d7e3903aca96af13d5eeee0d3dc`  
		Last Modified: Wed, 09 Aug 2023 10:35:57 GMT  
		Size: 10.1 KB (10125 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7737dca9b00e34927c9805d71ccc09e8eca763cfb841ec8bdecad0c520ea240`  
		Last Modified: Wed, 09 Aug 2023 14:09:39 GMT  
		Size: 48.0 MB (47985821 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48d3862c01fb1de5dadbfae7cff1bd335880156e96bff67d22de633085ffdb90`  
		Last Modified: Wed, 09 Aug 2023 14:09:37 GMT  
		Size: 2.4 MB (2368265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4434dfe6902652b76c04e34f90bfe00ca910f1ee7d002617220f878db5d51a0b`  
		Last Modified: Wed, 09 Aug 2023 14:09:37 GMT  
		Size: 17.7 MB (17667076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f43222c1c1886d075be1bfbfa9e2e796374ca1c02fd87fdcd3c31383c251390c`  
		Last Modified: Wed, 09 Aug 2023 14:09:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:971afbbb349a7f781bbe4c70a282da69a649044520d0094a0cbe1158decf2636`  
		Last Modified: Wed, 09 Aug 2023 14:09:38 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1aadb745b5bf59e8b357e4b09603c24f9980973931f45af4ed882f7dfb4b496e`  
		Last Modified: Wed, 09 Aug 2023 14:09:38 GMT  
		Size: 619.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08602d064ec7331c6444fe3c7b9a22766b4ff0cdde8d397e03070bbc95e0d11c`  
		Last Modified: Wed, 09 Aug 2023 14:09:39 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a33c462b911d025c5540d34f64541aad335ad1636b13d49a5c52d9aeb6f847a`  
		Last Modified: Wed, 09 Aug 2023 15:29:56 GMT  
		Size: 15.2 MB (15223675 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:d440d02859bf30b99aa5c912c61d2ad2055b84446dfb7cbb8285a9d184256148
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1453273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9258423231d10976a9d904b41942d4cf08a9f99c23beb8c9ffa0da380c16c394`

```dockerfile
```

-	Layers:
	-	`sha256:2b34eab6368c56ac5c36ef517c199daa4245ad2b2e7efb7a933e22c254549b0c`  
		Last Modified: Wed, 09 Aug 2023 15:29:55 GMT  
		Size: 1.4 MB (1440328 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9884a9cd24b68bb6425d0fbc91c0db68d18ce7882ca9eadc226f402b08609216`  
		Last Modified: Wed, 09 Aug 2023 15:29:55 GMT  
		Size: 12.9 KB (12945 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:4ce0296439bc092b732df697d05f08ca58ed8968c5f3e36040f3d76e25ed5981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82198484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:023d43cfae096b33eff68202d0b79266cd8a014b5eb969ff462ed52aebaae2fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
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
	-	`sha256:5e9ed89cc72757ffb55d6a5675055b26e328f250f19a583dc7c4a070f6145049`  
		Last Modified: Wed, 09 Aug 2023 02:17:10 GMT  
		Size: 16.2 MB (16243020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:12583472342fb69d9f43895d91eadda6d4b2a4d947ba2064c0236490e3d566bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.7 KB (12654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341adb6e44633f8c965636b825d6e0282f2f394f8a36719be5d1b6d7d02c4b2f`

```dockerfile
```

-	Layers:
	-	`sha256:980484ce25d50b8bd0bd476dc3ecd69a218fd4e8ae8cd459df8b7889998bb8ed`  
		Last Modified: Wed, 09 Aug 2023 02:17:08 GMT  
		Size: 12.7 KB (12654 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:724a2e122b120ab0dd2f2e44049c886ff410374745711eb6a4eefa24e2c89fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83385496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4196ae2dbcac8dea95bab78bf72538ce367db980f10987ae52dddfd764801ce`
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
	-	`sha256:ad30f2c2ea24300733758f57c86de1345309abc331440d30489541dfbf8d4f23`  
		Last Modified: Wed, 09 Aug 2023 08:48:18 GMT  
		Size: 473.3 KB (473277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f90d3f6f00cd150a918e39ec2061008175f9d189baf332a55e51779087eeed7`  
		Last Modified: Wed, 09 Aug 2023 08:48:18 GMT  
		Size: 10.1 KB (10145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1bfa1e4b201d96a10f379dba964ef3084cc033150e2545ae9fdd76ed768ab4c`  
		Last Modified: Wed, 09 Aug 2023 14:29:26 GMT  
		Size: 44.1 MB (44073653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ccdec895322602b4abcd26bf973fbda07dd963f3d2e2bd9250a633a8927459c`  
		Last Modified: Wed, 09 Aug 2023 14:29:23 GMT  
		Size: 1.5 MB (1519688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98be2b45e76cb1cf93a891eeb58b8397762d742461426432437f689b5f3408c6`  
		Last Modified: Wed, 09 Aug 2023 14:29:25 GMT  
		Size: 17.7 MB (17666916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2903a9bd79839285ce7442d7a20c44dd06ba5a8875ceac39b5b5bea87c5f146b`  
		Last Modified: Wed, 09 Aug 2023 14:29:23 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c7e1752079bbbb6e40bfa8ce5802faef178904c4643bef85918df8c992c71d5`  
		Last Modified: Wed, 09 Aug 2023 14:29:24 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63900654739c939e16c97f7750779b0c68a53f6a61d2fe7346c219e73872f1d3`  
		Last Modified: Wed, 09 Aug 2023 14:29:25 GMT  
		Size: 622.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc0c0282fbe14c869dc32194527473d8dc1d83105d46121632ec7dc86d49489b`  
		Last Modified: Wed, 09 Aug 2023 14:29:25 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e5f1f483a97bcb766c8c10bc5cdb0d643f2e763fc16d0e4499af3784368f0de`  
		Last Modified: Wed, 09 Aug 2023 14:51:52 GMT  
		Size: 16.3 MB (16293812 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:3a66334ebc1aa3eeebcd185339d1bb2b6b9124558bb511cb5b233792d86b0589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1451126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500669b2ba8ffbaa8e0cc63d48977268e016e9699ea1b5533295b90c1ef0097`

```dockerfile
```

-	Layers:
	-	`sha256:b1494b5f411534c826ffbe322ef4a4e36e6e10e0269a7803eae51d96df10580d`  
		Last Modified: Wed, 09 Aug 2023 14:51:50 GMT  
		Size: 1.4 MB (1438153 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d1804625be316b865ad967b5af4ea0cd6dbeda882b71664f15c9e463120a956b`  
		Last Modified: Wed, 09 Aug 2023 14:51:50 GMT  
		Size: 13.0 KB (12973 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:cbad71513d47b68efb54b002fdfb9f2a2c6a1be2f95c035eaa191587c44d25ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80409571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a58ce7787974f84d64ede99c54cd7ed1a4274f30947d4d338247b8369c3882`
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
	-	`sha256:5c8bd020b2175f142a2a3f9429c4296358dd43a44cfbb01e663569dfff85d137`  
		Last Modified: Wed, 09 Aug 2023 08:59:07 GMT  
		Size: 427.9 KB (427887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af2594681521d2f9a47261aed70f074eed34684452c91f97b6340181613a7e3e`  
		Last Modified: Wed, 09 Aug 2023 08:59:07 GMT  
		Size: 10.1 KB (10148 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd1a63d9af94d59864fccb2432620087cb92b8e56f111cb6e0bc18171256903`  
		Last Modified: Wed, 09 Aug 2023 11:46:15 GMT  
		Size: 41.5 MB (41492657 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21b21249d925567afeda76c04bb02003e65914ed85bc2ad4e69ce9484df44c47`  
		Last Modified: Wed, 09 Aug 2023 11:46:13 GMT  
		Size: 1.5 MB (1495030 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85b9ca73d68cbb5f9bf3c32dfc55f20b86e64e36ca0a29c672a1c062b935614c`  
		Last Modified: Wed, 09 Aug 2023 11:46:14 GMT  
		Size: 17.7 MB (17666902 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d49c6fa2220360e940b55f27e12be31912b8d242e9171bdf9833364248305770`  
		Last Modified: Wed, 09 Aug 2023 11:46:13 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0582feec67c72574e895c82950004f4c60487866f2b661e58fba596080fd6c4`  
		Last Modified: Wed, 09 Aug 2023 11:46:14 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e12b81c3cfbe13721d5573779794ea545995a00a9bc84f243506d81ba45bccb`  
		Last Modified: Wed, 09 Aug 2023 11:46:14 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:894adbcc94f18f33d7aed2ab39cca18b856569d6c8bbcbe00929be53c6379dd6`  
		Last Modified: Wed, 09 Aug 2023 11:46:14 GMT  
		Size: 830.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a5d75735f2f41dd54a3861553e3ded54e4d42dc8d2f03a79fdad010cc0124ef`  
		Last Modified: Wed, 09 Aug 2023 11:56:25 GMT  
		Size: 16.1 MB (16101005 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:e0cc23e4226a2143c429ee0d96b62605a9138e0afed6bfa9067fb452091f648b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 MB (1451135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e90424e03bf4636246008cd8bada0c3912825c364c58cd0958c083296be0d4`

```dockerfile
```

-	Layers:
	-	`sha256:363e6a16c0ada9fa20be2a89eeea063e76ebf9253cbcfc28e88aa0cfc204e4f5`  
		Last Modified: Wed, 09 Aug 2023 11:56:24 GMT  
		Size: 1.4 MB (1438206 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6136d7f506d673cc25102f9689ea90367455748e4424ca3c1456d6b72b477644`  
		Last Modified: Wed, 09 Aug 2023 11:56:24 GMT  
		Size: 12.9 KB (12929 bytes)  
		MIME: application/vnd.in-toto+json
