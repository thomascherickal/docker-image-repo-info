## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:5900310c3eab8a59e4e805049a068c22d327e2ca1294d303301549438fbf259a
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

### `rabbitmq:3-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:27f0593bed2dcb76fd23cd86af9b4dae9c4126212a752cd4b0bbf29412f0efcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70166448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37cf1a255719313355d23218cce83f8c8ad8a5463da9051550e00d4bf07e19a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:41:15 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 19:41:15 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 09 Jan 2023 19:41:16 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 09 Jan 2023 19:41:19 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 09 Jan 2023 19:41:19 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 09 Jan 2023 19:41:19 GMT
ENV RABBITMQ_VERSION=3.11.6
# Mon, 09 Jan 2023 19:41:19 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 09 Jan 2023 19:41:19 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 09 Jan 2023 19:41:19 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 19:41:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 09 Jan 2023 19:41:29 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 09 Jan 2023 19:41:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 09 Jan 2023 19:41:30 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 09 Jan 2023 19:41:30 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 09 Jan 2023 19:41:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 09 Jan 2023 19:41:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 09 Jan 2023 19:41:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 19:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:41:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 09 Jan 2023 19:41:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13940706f5135b061da5a8eb2ae0771b2bd616138845a4cd819a03e504daa04`  
		Last Modified: Mon, 09 Jan 2023 19:43:20 GMT  
		Size: 336.8 KB (336849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6020063b14e2abc455e9ef6411c0b7a7797cbb3d6439b9157a5a8a7f95c9f34`  
		Last Modified: Mon, 09 Jan 2023 19:43:20 GMT  
		Size: 8.9 KB (8918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd0f1839ab499436889400ad4f046585bce14f6f319cba0053d53410a014c53`  
		Last Modified: Mon, 09 Jan 2023 19:43:25 GMT  
		Size: 46.7 MB (46728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3037b514b070533292fa133ae5008f5c6c56215351679a3b555527e14cc6018c`  
		Last Modified: Mon, 09 Jan 2023 19:43:20 GMT  
		Size: 2.3 MB (2320719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307cbc98ab1ecfe5e960b557f88e9cc2e2ab12d60b42f557beb3efe95db54f3a`  
		Last Modified: Mon, 09 Jan 2023 19:43:20 GMT  
		Size: 17.4 MB (17398843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb5dee1fd14153d1a3427caaed9aee4e44a8cd1aed71480878de145c04443fd`  
		Last Modified: Mon, 09 Jan 2023 19:43:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e05d2e4ae545bf5268c9f8c73b79b4864e2e35af2f5058a3a69a16bec1b9ad0`  
		Last Modified: Mon, 09 Jan 2023 19:43:18 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eafbc9c3236ee9a2a9e0ede9f741f8969254d900ffb9a55f823372e9dadc78`  
		Last Modified: Mon, 09 Jan 2023 19:43:18 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb6593057bb92f0d8e3f553ba13dd385bf99287ad2781e3dc5d2a752935aee6`  
		Last Modified: Mon, 09 Jan 2023 19:43:18 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:0bc0d110f0d06f66fd10c014df1075b7515c7ce152ca43b89df78e3a6690b809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60402569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9ea3154da9acc547c1d3549b6db714fae4a44cfa5b8615d6ab89024593ba1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 22:43:39 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 22:43:39 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 09 Jan 2023 22:43:39 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 09 Jan 2023 22:43:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 09 Jan 2023 22:43:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 09 Jan 2023 22:43:42 GMT
ENV RABBITMQ_VERSION=3.11.6
# Mon, 09 Jan 2023 22:43:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 09 Jan 2023 22:43:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 09 Jan 2023 22:43:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 22:43:53 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 09 Jan 2023 22:43:56 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 09 Jan 2023 22:43:56 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 09 Jan 2023 22:43:56 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 09 Jan 2023 22:43:56 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 09 Jan 2023 22:43:56 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 09 Jan 2023 22:43:56 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 09 Jan 2023 22:43:56 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 22:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 22:43:56 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 09 Jan 2023 22:43:56 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00e7c223db25228dd1bb51ea7de96e01ee2d66e97c6e608b5ad8735b225d9ad`  
		Last Modified: Mon, 09 Jan 2023 22:46:42 GMT  
		Size: 318.3 KB (318349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6c1601aa6ebbb6222aa29f72093502dcee23df55a8e27488ca4aefcda5a4c`  
		Last Modified: Mon, 09 Jan 2023 22:46:42 GMT  
		Size: 8.9 KB (8894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ead8ae6ef1d017dfe8e2e282cc2fcf6252f4d96e4e2fca4afd3c5bf28ff5ed9`  
		Last Modified: Mon, 09 Jan 2023 22:46:47 GMT  
		Size: 38.1 MB (38117092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b4760df4b4d4b98c55d8745b0fa8c81d397ff05a2c3c950af42426bc6a394c`  
		Last Modified: Mon, 09 Jan 2023 22:46:42 GMT  
		Size: 1.5 MB (1450734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016594fce0cf9f04dda8d9cd7d03aa9239bdca36b3ef9b1546b7f4c74a28e84a`  
		Last Modified: Mon, 09 Jan 2023 22:46:42 GMT  
		Size: 17.4 MB (17398519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4943c3c4eb398e7b5e66a9f723445e92746f4e07a4b04696aed18b57001cdb2c`  
		Last Modified: Mon, 09 Jan 2023 22:46:40 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b903cd9f4de45edf3b4af64188550b0676eacfd44e27708ea73c9034b4fc24`  
		Last Modified: Mon, 09 Jan 2023 22:46:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2972aae067aefa2791067e542e36e7c46f9001b9c6ae66f65bbc76334b7ecc73`  
		Last Modified: Mon, 09 Jan 2023 22:46:40 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8c81f7ba5bbc16667954fb3271a60c5051afac3ac02336cfd3d99855406994`  
		Last Modified: Mon, 09 Jan 2023 22:46:40 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:39e2bb577e3a000a0076a9beb57fbe74aa4a30b00f587e3b19ba87d481ef2d67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59664476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3428a835d19cf946660196215479504b209267c75bc4106effe2cdc83cdc6fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 22:35:25 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 22:35:25 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 09 Jan 2023 22:35:26 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 09 Jan 2023 22:35:29 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 09 Jan 2023 22:35:29 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 09 Jan 2023 22:35:29 GMT
ENV RABBITMQ_VERSION=3.11.6
# Mon, 09 Jan 2023 22:35:29 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 09 Jan 2023 22:35:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 09 Jan 2023 22:35:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 22:35:37 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 09 Jan 2023 22:35:38 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 09 Jan 2023 22:35:38 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 09 Jan 2023 22:35:38 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 09 Jan 2023 22:35:38 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 09 Jan 2023 22:35:38 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 09 Jan 2023 22:35:38 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 09 Jan 2023 22:35:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 22:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 22:35:39 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 09 Jan 2023 22:35:39 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f13c9df40da94c6dc9726cb21279c8f4b4e04db6503aaa067071def7a85c9cd`  
		Last Modified: Mon, 09 Jan 2023 22:39:13 GMT  
		Size: 300.3 KB (300330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58de52fe130987f13657762bbb3c17d1a1ad96047b566787b70249623ee14598`  
		Last Modified: Mon, 09 Jan 2023 22:39:13 GMT  
		Size: 8.9 KB (8887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00457926bea1c3b0fbae3d3cb94196a516e0b7b310f2c2d1a511ef96bd30a527`  
		Last Modified: Mon, 09 Jan 2023 22:39:18 GMT  
		Size: 37.7 MB (37730587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc07d0fbcb71ef055f26a555a9c71688a045570eac1024a5f9fc96a31b57155`  
		Last Modified: Mon, 09 Jan 2023 22:39:13 GMT  
		Size: 1.4 MB (1359212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0563144ceca7ce23e2db3a26d49be1eba91830aa3e8d662dc3ff41395657d0`  
		Last Modified: Mon, 09 Jan 2023 22:39:13 GMT  
		Size: 17.4 MB (17398516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c48d149e1b1d4660eca680b113fe482c606f92cf4448479b810de1acd6f08b`  
		Last Modified: Mon, 09 Jan 2023 22:39:11 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df955bdee6bbb2ee50a08d42a96801e451efc4222bfa26313eace631bd2818c`  
		Last Modified: Mon, 09 Jan 2023 22:39:11 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b28c5501e4e41506b0b8c1b7f698e68bbbdc3933307dd4b112dec6b02cf370`  
		Last Modified: Mon, 09 Jan 2023 22:39:11 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78463b72d0dc614e4817eda506db8baddaf6ded69b5abc8256e7eefad0f970bd`  
		Last Modified: Mon, 09 Jan 2023 22:39:11 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:a62d6d83a8b4d37f83830653fbf22298f333b9ed388fe5a113e5388247dd905c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67546625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636b3b0b899ce46bc873cd51e301099149fe1857a1481fa83787a8c362403946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:04:14 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 19:04:14 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 09 Jan 2023 19:04:15 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 09 Jan 2023 19:04:17 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 09 Jan 2023 19:04:17 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 09 Jan 2023 19:04:17 GMT
ENV RABBITMQ_VERSION=3.11.6
# Mon, 09 Jan 2023 19:04:17 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 09 Jan 2023 19:04:17 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 09 Jan 2023 19:04:17 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 19:04:26 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 09 Jan 2023 19:04:27 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 09 Jan 2023 19:04:28 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 09 Jan 2023 19:04:28 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 09 Jan 2023 19:04:28 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 09 Jan 2023 19:04:28 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 09 Jan 2023 19:04:28 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 09 Jan 2023 19:04:28 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 19:04:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:04:28 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 09 Jan 2023 19:04:28 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa6fc68dc79e0c0a160b4e34a533a12be6d9c516c4f2db4079b321b6c606ac1`  
		Last Modified: Mon, 09 Jan 2023 19:06:19 GMT  
		Size: 318.9 KB (318946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a78a2e74a3f29d186eed9037d9264612b11f8775ae4003d18f10f910f0a6acb`  
		Last Modified: Mon, 09 Jan 2023 19:06:19 GMT  
		Size: 8.9 KB (8919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2295e22e51875c9bdbbccaffe07302e8fee2e5a75a8c006b412db3d069427080`  
		Last Modified: Mon, 09 Jan 2023 19:06:23 GMT  
		Size: 44.2 MB (44185365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f260f81a86fe7ef66f1dbf35429a43f9eb8a0b511731822375ae9834ea537b80`  
		Last Modified: Mon, 09 Jan 2023 19:06:19 GMT  
		Size: 2.4 MB (2373367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654d3c89be4462240c24bc4eca9aa68ce99e7cee4aacd6627a8b0c4e54433d28`  
		Last Modified: Mon, 09 Jan 2023 19:06:19 GMT  
		Size: 17.4 MB (17399045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e021b292f3ec67a30ef0f531e704098ec1bc78c6726239e8baf0edd3a4c827`  
		Last Modified: Mon, 09 Jan 2023 19:06:17 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa744b3d532747549da021bfd094fac1792875503cd4e1b80ed4261eccf78cf`  
		Last Modified: Mon, 09 Jan 2023 19:06:17 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5991943508ed009a8cb1af6bf3df69c2669183ca3952e9a1dfdc7162ca9ef4`  
		Last Modified: Mon, 09 Jan 2023 19:06:17 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae86bd93aa97070cfb4ec14fb444fba378e3526124e75b8dd54f98db226be0d`  
		Last Modified: Mon, 09 Jan 2023 19:06:17 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:a0972b2b661daa52e9f5beaa398887199ac6e382359bc4abe626e5517a88c8bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62004936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f3e27e8eaf3f5e24ca63e361c37e4071a2caaf43e7e056e7e82067c8a81ab6`
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

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:773a1828d220adb0a3107637e182a25644de77423fa9989e13970522cec9c000
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739b7e3a359dc82ad578fd66ba607bdbf1453ae016fb76c8bf370be28d4f6b4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:26:06 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 21:26:06 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Mon, 09 Jan 2023 21:26:07 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Mon, 09 Jan 2023 21:26:12 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Mon, 09 Jan 2023 21:26:12 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Mon, 09 Jan 2023 21:26:12 GMT
ENV RABBITMQ_VERSION=3.11.6
# Mon, 09 Jan 2023 21:26:12 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Mon, 09 Jan 2023 21:26:12 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Mon, 09 Jan 2023 21:26:12 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 09 Jan 2023 21:26:27 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Mon, 09 Jan 2023 21:26:29 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Mon, 09 Jan 2023 21:26:30 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Mon, 09 Jan 2023 21:26:30 GMT
ENV HOME=/var/lib/rabbitmq
# Mon, 09 Jan 2023 21:26:30 GMT
VOLUME [/var/lib/rabbitmq]
# Mon, 09 Jan 2023 21:26:30 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Mon, 09 Jan 2023 21:26:30 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Mon, 09 Jan 2023 21:26:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 09 Jan 2023 21:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:26:30 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Mon, 09 Jan 2023 21:26:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5719ee68e0eed949889c2bbc858871bfde755616cfbb0fcca3d0242dbf5115`  
		Last Modified: Mon, 09 Jan 2023 21:30:09 GMT  
		Size: 371.1 KB (371083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a59f8544f60799ba79266a8982ce6b81812aff40e0574e27b2bec3f80214dc`  
		Last Modified: Mon, 09 Jan 2023 21:30:09 GMT  
		Size: 8.9 KB (8927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974fa106ec6bb77ca4c8c726ba21171b262e77b3e0b180bd94b28bd540580c5c`  
		Last Modified: Mon, 09 Jan 2023 21:30:16 GMT  
		Size: 39.3 MB (39256986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc353a3b21dc3eeb24b87a7e6404243ab2b7be17a43ae492fa6ecf1bfa79715d`  
		Last Modified: Mon, 09 Jan 2023 21:30:10 GMT  
		Size: 1.5 MB (1549489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43eb1cb5a892cdf6f138a51f7c36b1222f9c1d2dd6cf8e47ffe88c545b2dc84`  
		Last Modified: Mon, 09 Jan 2023 21:30:10 GMT  
		Size: 17.4 MB (17398554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91a4594d9a4082a0c9562a6d5df859973c37fc33e9eb38a6d9166428a15ec40`  
		Last Modified: Mon, 09 Jan 2023 21:30:07 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e935b06cbca0417c2e0686530d61d01bf544a421114f86b88272cb8be61b2a`  
		Last Modified: Mon, 09 Jan 2023 21:30:07 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6b9dd2037d49fca2f64c660de6102e45452ebb13689aee2ff725c7be49321`  
		Last Modified: Mon, 09 Jan 2023 21:30:07 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acb9a5d54a900ba49fca9f1c0852337f56ef6ae89ad98e70d0c524aa04f903d`  
		Last Modified: Mon, 09 Jan 2023 21:30:07 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:b326ff51ea0bca681febb801d056ab09d781dad708601a26bbd83d2dd9eeed6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60474850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4db32ed2df6eaa629db282965473912edf65041406fddacc633956ac6a73639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:11:12 GMT
COPY /usr/local/bin/ /usr/local/bin/ # buildkit
# Tue, 10 Jan 2023 01:11:13 GMT
COPY /usr/local/etc/ssl/ /usr/local/etc/ssl/ # buildkit
# Tue, 10 Jan 2023 01:11:17 GMT
COPY /usr/local/lib/ /usr/local/lib/ # buildkit
# Tue, 10 Jan 2023 01:11:21 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 10 Jan 2023 01:11:21 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private /usr/local/etc/ssl; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		openssl version; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 10 Jan 2023 01:11:21 GMT
ENV RABBITMQ_VERSION=3.11.7
# Tue, 10 Jan 2023 01:11:21 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Jan 2023 01:11:21 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 10 Jan 2023 01:11:21 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 01:42:34 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie" # buildkit
# Wed, 18 Jan 2023 01:42:35 GMT
RUN set -eux; 	su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus; 	echo 'management_agent.disable_metrics_collector = true' > /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf; 	chown rabbitmq:rabbitmq /etc/rabbitmq/conf.d/management_agent.disable_metrics_collector.conf # buildkit
# Wed, 18 Jan 2023 01:42:35 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Wed, 18 Jan 2023 01:42:35 GMT
ENV HOME=/var/lib/rabbitmq
# Wed, 18 Jan 2023 01:42:35 GMT
VOLUME [/var/lib/rabbitmq]
# Wed, 18 Jan 2023 01:42:35 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Wed, 18 Jan 2023 01:42:35 GMT
COPY 10-defaults.conf /etc/rabbitmq/conf.d/ # buildkit
# Wed, 18 Jan 2023 01:42:35 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Jan 2023 01:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Jan 2023 01:42:35 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Wed, 18 Jan 2023 01:42:35 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077cf467d5332db0aac817beae64623418a238e1cb8c60a9ce2f7db3eb2eeab`  
		Last Modified: Tue, 10 Jan 2023 01:17:01 GMT  
		Size: 336.4 KB (336363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294ec75ea5bee541b830dcd136aff24b40314bb7e5fd2e1ca52ecbc50930cca`  
		Last Modified: Tue, 10 Jan 2023 01:17:01 GMT  
		Size: 8.9 KB (8919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a594c19483a044b5b380e85dfdec52fd16f201d96994401603c88646e4653a0d`  
		Last Modified: Tue, 10 Jan 2023 01:17:05 GMT  
		Size: 38.1 MB (38067911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b10521501d1511b2a87f59842e4ee972a7d6d369fc40a0e3065e3cad6eb1cb2`  
		Last Modified: Tue, 10 Jan 2023 01:17:01 GMT  
		Size: 1.5 MB (1481298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56537ef2ec14dd159d5046066f5a045ddd9f28fc35c8790789756031f395f76a`  
		Last Modified: Wed, 18 Jan 2023 01:46:01 GMT  
		Size: 17.4 MB (17407878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af7b2eb99926da6aaeaebe4a8bd285f28ef16e286f583cecbf47382a0233b24`  
		Last Modified: Wed, 18 Jan 2023 01:46:00 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ad5ff84a34f67aa1a5c9580d7c0381badce40368f4dd4a79d1eaf71783a355`  
		Last Modified: Wed, 18 Jan 2023 01:46:00 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c7ef13b25ba22fc2b638ff6b869f0fa25d75950acc9d9dde2593620ad3355`  
		Last Modified: Wed, 18 Jan 2023 01:46:00 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b6fb1dd87c8a92cbcb766ddd8b87367eb80e36f15a21b91f4ecf7ba50323c`  
		Last Modified: Wed, 18 Jan 2023 01:46:00 GMT  
		Size: 833.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
