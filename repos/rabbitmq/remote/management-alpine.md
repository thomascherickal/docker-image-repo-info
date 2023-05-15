## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:16d7da8ea63c31484f754b7d6781654420b7b54cd45e9360e06af67bdacd0526
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
$ docker pull rabbitmq@sha256:a5661e3b79c3a476ea1e72b96eb1a5b5032d4b09fd87fb7dcf4cba32f55b9072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88121083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dee980bdab517ecd6dc8c657cbcc6715f267f825f074b2598a2e21240e578ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee385a09527de31532e14f03ca9bf37a477ed3eed276075e56a753d075ae71e`  
		Last Modified: Thu, 11 May 2023 21:17:12 GMT  
		Size: 427.0 KB (427048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab56bd8d7d2eb982e43d440efde2d21f9e5351724fa7009fcc88f95398f7dd1`  
		Last Modified: Thu, 11 May 2023 21:17:12 GMT  
		Size: 10.1 KB (10141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c069ac05d1391b5391ca0e2ca95628fd0f030ab7dc37545faccc0d86dba206`  
		Last Modified: Thu, 11 May 2023 21:17:16 GMT  
		Size: 44.0 MB (43974361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f4bd6dbc0f81e1130d75d9067d258c634784acb031126729ccbf25a279db6`  
		Last Modified: Thu, 11 May 2023 21:17:12 GMT  
		Size: 2.3 MB (2296181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54daf963c22dfdbc96332cefadf471c7d19411ba305b2026d972671716bfbd8b`  
		Last Modified: Mon, 15 May 2023 21:29:31 GMT  
		Size: 23.0 MB (22969742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b8aa7054e8ae31ee0b7e7369b2ae996381224b4ae84cc71e0aa1e419f2e4b`  
		Last Modified: Mon, 15 May 2023 21:29:30 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265e7f0d035232b2a8d8f9711a9838f6c8d343d1738c5832318e3aad5cdf98d3`  
		Last Modified: Mon, 15 May 2023 21:29:30 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d8297a792d69525b1501b494fd3f4917799a7260bcc4fc130755c804fde7e`  
		Last Modified: Mon, 15 May 2023 21:29:29 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037e246423c7809b55e5af88ab33e51822b54239bf3a6ec7f5488c3081092bdc`  
		Last Modified: Mon, 15 May 2023 21:29:29 GMT  
		Size: 827.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e868ee61678f3207c65e69f43a7ca04a4a5eae41acdf69093423e2c153d26ba`  
		Last Modified: Mon, 15 May 2023 21:29:46 GMT  
		Size: 15.0 MB (15044354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:05c14e180efe7b4238f6661cfc7b0d0668945efbe4dd96192acc4779ee712e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84897064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a848a02933a2f25ab55f127399217e5068b57ff0f33b7e35fb69668c7f8641d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
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
	-	`sha256:7e20fa2849bfcda2e22726be52627a45ccc5a67c6a60c0a8c02cd8ee4bbbb1c1`  
		Last Modified: Mon, 15 May 2023 22:00:41 GMT  
		Size: 23.0 MB (22969372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993c028453a80f70e109bfc79d07d50efbfb851754b06e8c000d0d054cff0db1`  
		Last Modified: Mon, 15 May 2023 22:00:38 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54aa47cda2fced809f3bd1cf8f64552b4d65b2e22d83edb4814f5ba49603743`  
		Last Modified: Mon, 15 May 2023 22:00:38 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb3508e395c809785cc8a9d3dd3eb7559846e35ef302854ba9ffc7ab235cd3`  
		Last Modified: Mon, 15 May 2023 22:00:38 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa8c36259ddd9e1a91c43029ff8915a451fa36e38b7fcd7d2e85dbb2f70081`  
		Last Modified: Mon, 15 May 2023 22:00:39 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d819e3310af6ac0dd7a6bd3e7ab0bf629f7c88a20a3c499b3ca09d07cb0c78a9`  
		Last Modified: Mon, 15 May 2023 22:00:57 GMT  
		Size: 15.6 MB (15577895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:eb9281cff22414b22a5d01a414ef82c3bf1f73f6fb589c86ed3c1ff323126f54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83497150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ff8a51db2c9b936b5167da09e7b3e6bf5bb2d1f3f38499e1cfcc18337500b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
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
	-	`sha256:4047743bcd61c1fb545ec5864570de2ac3406b3d95bc50d4f8fa11248736136d`  
		Last Modified: Mon, 15 May 2023 22:30:53 GMT  
		Size: 23.0 MB (22969242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b416f3a09a59652efe5820671a6e5e393d1ba586af0f3271a9540643ba0b1583`  
		Last Modified: Mon, 15 May 2023 22:30:51 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda287fa2a94080ab740179284724edbbd23ce685a1a32e86103851ef1b7ad17`  
		Last Modified: Mon, 15 May 2023 22:30:51 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dc6729868b2bea979cbdf238548b34d08b056643ab20477943c3004b471244`  
		Last Modified: Mon, 15 May 2023 22:30:51 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8200151fc6daec1505bc3320847b6b348f0a2485d9ebe4245e236468bb26ed7e`  
		Last Modified: Mon, 15 May 2023 22:30:51 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637cb65489d79d2e307f8bcd073d290db9ed8a9ac5c4cb980164d1c8e8c22b9`  
		Last Modified: Mon, 15 May 2023 22:31:13 GMT  
		Size: 15.2 MB (15184537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:efc95b5f8f17f2470408019450cf01f7ed6f37e234783f4c41e05f28bb1db710
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92130031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca08ac999cb0e127be4ed91bf6ee5daf2dc6f03eccb8341dc55edba4722cbb0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
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
	-	`sha256:f6f9e06c48a28d923442bdee15ecde1baa68a2e28bddeadce7e08a15ad5a0d53`  
		Last Modified: Mon, 15 May 2023 22:06:41 GMT  
		Size: 23.0 MB (22969712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c66e3fb3727836a97a5fbcb105dbbd1788bad78e31ef9757832b663652d7ac`  
		Last Modified: Mon, 15 May 2023 22:06:40 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbca246a5b9102697854dd9a4d6413f6f285abdfb2e36dfa1bc4372ba33586f`  
		Last Modified: Mon, 15 May 2023 22:06:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6570baa24f8fb9c722535514c873b817193342a4154d1c9b4eda5f1a02622e`  
		Last Modified: Mon, 15 May 2023 22:06:40 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be6b434533798b51585ace28a624ddd421f453e7d674f9ed6084730690cc37`  
		Last Modified: Mon, 15 May 2023 22:06:40 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75b2c531421cf9ee7f51e39c6ac3d21e7f32f328a0bd15a9bfaabe59b016582`  
		Last Modified: Mon, 15 May 2023 22:06:56 GMT  
		Size: 15.2 MB (15198053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:dd760c469709d498324eb608b9f45ccbbed0611672864a0828f1e29a4b9b8423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.4 MB (87415641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c583b7f2920434e1f788a8a3e28376dd158477a3e4b1b9764d6fb25212f4fca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:03 GMT
ADD file:cfe47ebe49c4a75094234cafa52aa13aa26abcdad49b89293585884b3a8faeae in / 
# Tue, 09 May 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
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
	-	`sha256:22ee86a7941798930dc1bfb2335eaf6ea7768aba08c8225123d8e7731adc7dda`  
		Last Modified: Mon, 15 May 2023 21:48:20 GMT  
		Size: 23.0 MB (22969259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b56abcabd11cb0856877264e5d4a589eab6a88742acca4f431103bf6cff0bde`  
		Last Modified: Mon, 15 May 2023 21:48:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2fbccf1cea79cf3301d1e098064f073d7957fd31f21acd88e77f7f03401a4e`  
		Last Modified: Mon, 15 May 2023 21:48:17 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1594e8b2f5e0ae4148d590be4817915ca4e1e124fccdd986d530bd371bec7582`  
		Last Modified: Mon, 15 May 2023 21:48:18 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f0ecddd2823683a61423bc6467a3695ecbdbc07d27c02e6b874f684254f79e`  
		Last Modified: Mon, 15 May 2023 21:48:17 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28658ab9907c7e4c3e790a398ec1a1de6931ec6576b39f912a49a5fa085e2b2`  
		Last Modified: Mon, 15 May 2023 21:48:36 GMT  
		Size: 16.2 MB (16217894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:1ad39439a7dd9ee5ba211005cf3c8394ae1c846401acb241c6d6976aead39e26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.6 MB (88610813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e416186ccd1f86fda98928305ccc43622c9f52ddb1f1bda30caf4b608bbcc110`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
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
	-	`sha256:f40609fff92a3b5c52d274a155c70de51a018b466a1b44444f97d43602b6e1c0`  
		Last Modified: Mon, 15 May 2023 21:30:53 GMT  
		Size: 23.0 MB (22969250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7ac5eb39368470470582c6a39adae13b4c419c17f65c0f63b7e401653d20b2`  
		Last Modified: Mon, 15 May 2023 21:30:50 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602c09c88162e1ee48c5a42984306ac1ec57f81e1a5001cf3a41c3fbfb9cf841`  
		Last Modified: Mon, 15 May 2023 21:30:50 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f2d6d2f1af761e4abee43d9d12740ad2654fb85f0417d2c14112950833d79f`  
		Last Modified: Mon, 15 May 2023 21:30:50 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a938c82882b506e8c4c67e8e6534dddfba8dd5049557e9a5d6a418994ec76e`  
		Last Modified: Mon, 15 May 2023 21:30:50 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fcbed7315b191384e27342eaeae603528e81ca3045c37d237eed899d987731`  
		Last Modified: Mon, 15 May 2023 21:31:12 GMT  
		Size: 16.3 MB (16267937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:e6ddca53b632456b88ce6ed6f16053b9bc17b1c009813ee0acdb4d81f992bb07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80015288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff92bd011ac9b70319aeeaccaf24ac4e39c1b46017064a36b26af08db8df1eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e '/\.include.*fips/s/.*/.include \/usr\/local\/etc\/ssl\/fipsmodule.cnf/' 	    -e '/# fips =/s/.*/fips = fips_sect/' /usr/local/etc/ssl/openssl.cnf; 	sed -i.ORIG -e '/^activate/s/^/#/' /usr/local/etc/ssl/fipsmodule.cnf; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_VERSION=3.11.16
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Sat, 13 May 2023 17:05:18 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 May 2023 17:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Sat, 13 May 2023 17:05:18 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENV HOME=/var/lib/rabbitmq
# Sat, 13 May 2023 17:05:18 GMT
VOLUME [/var/lib/rabbitmq]
# Sat, 13 May 2023 17:05:18 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Sat, 13 May 2023 17:05:18 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 13 May 2023 17:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Sat, 13 May 2023 17:05:18 GMT
CMD ["rabbitmq-server"]
# Sat, 13 May 2023 17:05:18 GMT
RUN set eux; 	rabbitmq-plugins enable --offline rabbitmq_management; 	rm -f /etc/rabbitmq/conf.d/20-management_agent.disable_metrics_collector.conf; 	cp /plugins/rabbitmq_management-*/priv/www/cli/rabbitmqadmin /usr/local/bin/rabbitmqadmin; 	[ -s /usr/local/bin/rabbitmqadmin ]; 	chmod +x /usr/local/bin/rabbitmqadmin; 	apk add --no-cache python3; 	rabbitmqadmin --version # buildkit
# Sat, 13 May 2023 17:05:18 GMT
EXPOSE map[15671/tcp:{} 15672/tcp:{}]
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ff7227d7a9746fd56b9318759c02d91823d6766c3627a321b04ed92124a986`  
		Last Modified: Thu, 11 May 2023 21:06:22 GMT  
		Size: 425.2 KB (425186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e7ac60bde04070bb337c7594c1c44980735a2d22daf4ea5430af6459c378b0`  
		Last Modified: Thu, 11 May 2023 21:06:22 GMT  
		Size: 10.1 KB (10139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd30a8569d19617387bcc9c39ee8f0e7b0c574a1252557936cf0c6195cea792`  
		Last Modified: Thu, 11 May 2023 21:06:26 GMT  
		Size: 35.8 MB (35817881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af228fe269174efc4042191e7c5b1cfd733c15f8e44ba2f9547c571658f4080e`  
		Last Modified: Thu, 11 May 2023 21:06:22 GMT  
		Size: 1.5 MB (1494911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ecdfc7ff5bdcb3a3498b5ac62388b26108262c7d9a1fd43e94d4ab7807282`  
		Last Modified: Mon, 15 May 2023 21:59:01 GMT  
		Size: 23.0 MB (22969214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c402039aeeec8352320e9c5d9a70cb749d960b55f6aa9a108abfa521c3f9084`  
		Last Modified: Mon, 15 May 2023 21:58:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1583ba7df5489b4ae6863158790d946d44d700da4f236da5e23b762d89c1155f`  
		Last Modified: Mon, 15 May 2023 21:58:59 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4db0cb254dc61eb7f3dc226ca935e2654c971ea45af320d7950250bff7650`  
		Last Modified: Mon, 15 May 2023 21:58:59 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1917ed048fe36472fe31f1fa8dacd39fe0851d8295b238c73fe7fbd7e76c86b`  
		Last Modified: Mon, 15 May 2023 21:58:59 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33fdf4233249c1dfcd4f2a1e910c39f20082e9fbe4587e68800ffbaa9d23a12`  
		Last Modified: Mon, 15 May 2023 21:59:12 GMT  
		Size: 16.1 MB (16069879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
