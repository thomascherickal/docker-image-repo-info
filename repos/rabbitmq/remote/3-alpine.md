## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:23ec95b20e371821e791220da01aef9f7064a1b2a2171f1bd4d02ab03cbd3d95
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
$ docker pull rabbitmq@sha256:0e6c28e7d79cc337b0fde7a16587d382ec2022bfe64a3e7a54d10c1643d8d392
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (71041071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e37986d5bed177671d00edc2d0b8545dacf705624d83204a8bf740258b59bf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23749d8ebabbc57f2cc5e562e0cc02d2b7a4375595e64054958140160d700790`  
		Last Modified: Fri, 06 Oct 2023 01:07:22 GMT  
		Size: 40.1 MB (40075658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:daa48703636c395f750e1e6e5daf44c45db50ba4e2a138c802e581356b44b706`  
		Last Modified: Fri, 06 Oct 2023 01:07:20 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89f49954322d35a425dc895fc1ec4523233d2f917db6470abb5f47073081d0b9`  
		Last Modified: Fri, 06 Oct 2023 01:07:21 GMT  
		Size: 7.5 MB (7545713 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e4c204f7b873b79a78a6a943a8ed46acfb5440bdfd8a0a539831fe0d703934e`  
		Last Modified: Fri, 06 Oct 2023 01:07:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b507e5e0ff006bfb2a78bb0da7b001d0872787d88b647346ca511307a0a0fe4`  
		Last Modified: Fri, 06 Oct 2023 01:07:22 GMT  
		Size: 2.3 MB (2297429 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc19add11fb9d40777b6ba169f3d30ec6cae65bb84f88ddebaa80374d2233f8d`  
		Last Modified: Fri, 06 Oct 2023 01:07:23 GMT  
		Size: 17.7 MB (17717782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:752b91f7475158d7881b29f5b59d54f15a23a20c697f00a5818217934549a5ff`  
		Last Modified: Fri, 06 Oct 2023 01:07:22 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ee28840cf9d57f8aa737480fb573328e039cc71bb21f6c0aeebe00a85ea3481`  
		Last Modified: Fri, 06 Oct 2023 01:07:23 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67f08ed9a1a3f3d1b30e337d783ba962a975561792c9546c07f80678e692ca1e`  
		Last Modified: Fri, 06 Oct 2023 01:07:23 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59c4d351e8a1c9029858c2a8c9a2fc8c9be7645ae6b6f408d27dfd88f72e4709`  
		Last Modified: Fri, 06 Oct 2023 01:07:24 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:d4e4e2997b2f0f54802cdf36e4b1085a16724f66d433de06544bde06b9d4c905
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5536120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135dd09e3764242109ed0f97456c91923a30b913f91aff953f10798156eab2ff`

```dockerfile
```

-	Layers:
	-	`sha256:ee004fd6e3189bfe6fda070ec0d4ff69fa42782c715d073965a92498f3879300`  
		Last Modified: Fri, 06 Oct 2023 01:07:20 GMT  
		Size: 791.2 KB (791154 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cbb3e27f9b3ea2017d7d2a51612a50d9d3662d5ae518ccab92c7731016e4b47a`  
		Last Modified: Fri, 06 Oct 2023 01:07:20 GMT  
		Size: 2.3 MB (2338323 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0204271eba4e79ec6d19f04998b70e079ee2b6bb419286682e5ac05dff7001cb`  
		Last Modified: Fri, 06 Oct 2023 01:07:20 GMT  
		Size: 2.3 MB (2337377 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:26f8bcfad0ee399527d4dcfa337e7887d90d71265ec53bc835cab20f5690e09f`  
		Last Modified: Fri, 06 Oct 2023 01:07:20 GMT  
		Size: 69.3 KB (69266 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:6478d609695fcf8798ecaf0a6581cc7dbecaab098fceb617537cc8e143548110
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61042731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0032781d41a37a62de4a6309291b496ccc296ce0d06e4f47107b63b2b4728b88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a3be95759a045709ab38906f7cf6f6e6bf3c68df81e46b393e362cc33ad0db`  
		Last Modified: Fri, 29 Sep 2023 03:17:28 GMT  
		Size: 32.4 MB (32389317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc8f2c66a22c3b9ebbb50e974c41ddb7a016794bba130b2aca1e9e89b67206c`  
		Last Modified: Fri, 06 Oct 2023 01:48:52 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8010ee9455ad640f04a250c4eef24e3f975f689e8b43998f81e406f032e218`  
		Last Modified: Fri, 06 Oct 2023 01:48:53 GMT  
		Size: 6.4 MB (6375332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3e9093b844eee3450d02a4da96768722eac913a433a7d81b460a61f9caa604`  
		Last Modified: Fri, 06 Oct 2023 01:48:52 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b7f348a49c5f9c87473bb6c42cfe22be37143425b162d52ad08e5a0a2e585e`  
		Last Modified: Fri, 06 Oct 2023 01:48:52 GMT  
		Size: 1.4 MB (1412513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd88cead7c601ae9dc2ff716428f91a9e975611c8604be184f3ea092c5c300f9`  
		Last Modified: Fri, 06 Oct 2023 01:48:52 GMT  
		Size: 17.7 MB (17717744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4decd4db3f5149b825cd72ab60bd3cee10d0350692ee9a018a670d0461c50a6`  
		Last Modified: Fri, 06 Oct 2023 01:48:50 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f6047e6716914622a4e1793084f35d596ef5de8930475efd1609c918dfeeb3`  
		Last Modified: Fri, 06 Oct 2023 01:48:50 GMT  
		Size: 109.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e3b7f00d08ad39c29c1cdd7e67a54bc0eae4307a793cf86f6b2ed9938df2c8`  
		Last Modified: Fri, 06 Oct 2023 01:48:50 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6d56c42a22dd89fa1e38f1d8e4408955fb81d22f1258c28c2da685b468be8b`  
		Last Modified: Fri, 06 Oct 2023 01:48:50 GMT  
		Size: 829.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:63336e02bf9af78c33d7329a37352458832735d2401868d299eec1a095a2c718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60268411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bbe6fe02a66763de6061dc8bba29a6823e968aed34dd324b5f35069550e818`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92b54b25b49d8347ed6149acb265176b78663285f2d55be185289c2301e98bc3`  
		Last Modified: Fri, 29 Sep 2023 04:53:01 GMT  
		Size: 32.3 MB (32267798 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1124142db962f69f82a15294023dc6586fc0b6f0fa61c1ce2f6554330d32b0f4`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50826557c475b6cdb76eed9e5e9ef559ae8d57a531cc4f3295938b0ff66cc533`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 6.1 MB (6080035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6590481c1b44e58bd6a8cbf419602fe53268e5f06e6c91d4312c9fc3685d9feb`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 387.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ea40aacf0fb20ce0f8b80d1ec878e3c819edc7777b1e25977586e7c54dee27`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 1.3 MB (1300458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:497afd567e1e767508d6c97e17b00cf09e7cd91b8efb922531c32f6886260192`  
		Last Modified: Fri, 06 Oct 2023 03:21:32 GMT  
		Size: 17.7 MB (17717689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c4751ab5c777d010dd7fb660ca2976fbf9a1d284dc055661b68f16fc067c76a`  
		Last Modified: Fri, 06 Oct 2023 03:21:31 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8f78e82bf6ebd62ae9440f38702974b8e27838eba67aa03af48bbb4fbae81be`  
		Last Modified: Fri, 06 Oct 2023 03:21:32 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6463a2602674eea004cdd3af18b1b3e0b550a817ff7dcdcb692d7d7f3bcf591a`  
		Last Modified: Fri, 06 Oct 2023 03:21:32 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34c4bef54ccbef9312c093dc9785c87414ecec372e53741671d5fc421d8cb985`  
		Last Modified: Fri, 06 Oct 2023 03:21:32 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:7028ff8fd800111e01b39fdff869a11b1747432374e83e8c712cd8be1bed5032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5357456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:349e2c3c738a0ff034f5ad522f7dd00f7ab665eb9080a98cd6951c1e685ec5d9`

```dockerfile
```

-	Layers:
	-	`sha256:29c82b7b33ebb2c5649e474b1b77e7a59ba468b3aa84710638613a4423aad33d`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 787.2 KB (787174 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ac3ab866c68c33ecb86110dedd4f124b8b31f39b6182a9be68b9eaa425892e16`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 2.3 MB (2250958 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f5eb5396347bb9b67d908107a4fbe29d6114284297536b76d4792269d071657a`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 2.3 MB (2250012 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b55caccf4258a8726a46ca02ab1ac4439e7ce480b8f4ed982a6fe3c7f5122a7d`  
		Last Modified: Fri, 06 Oct 2023 03:21:30 GMT  
		Size: 69.3 KB (69312 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:fe345432ab5d5994b320e01844f7e17ddf9626e9d198d6aa3ef92a78f7810918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68432579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c41f1a459d82562fd998d7f556078122b00a701e9db1177922216494fc9a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc88776f25bc7a218134623254b6c2d572d6f6e753134e433a7a2fe68c9dea7`  
		Last Modified: Fri, 29 Sep 2023 05:02:25 GMT  
		Size: 37.9 MB (37873917 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d0d901bfce5a8fcf27f23165edf88b84a546308780b59411e51ed05022ec439`  
		Last Modified: Fri, 06 Oct 2023 03:09:59 GMT  
		Size: 398.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89cd876d1307663cd0a4a66c7cd4748f95b6f8ae9fc15be12b091b66321b01d8`  
		Last Modified: Fri, 06 Oct 2023 03:10:00 GMT  
		Size: 7.1 MB (7137752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1a4739fb5ffc382efa327031cc1b7f967039ab02d5ae1532c205b33ba68801f`  
		Last Modified: Fri, 06 Oct 2023 03:09:59 GMT  
		Size: 388.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:062b016056057e47074f9694fd2c2db298c205d7cd6cfddb6824284c4704abb6`  
		Last Modified: Fri, 06 Oct 2023 03:10:00 GMT  
		Size: 2.4 MB (2368785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:926849ba94ed632aa90dbdccacfd1d693318f3ea937f808dcaa8ed41a0a8182f`  
		Last Modified: Fri, 06 Oct 2023 03:10:02 GMT  
		Size: 17.7 MB (17717765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6cd0c5ab86a8f0ff085f2b074e072c708317a4b2a1fa122770c3d259270fcab`  
		Last Modified: Fri, 06 Oct 2023 03:10:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5c4df52137c07d7f39a601e1955dca97fd016755c54d739df0d8690a1a50bd7`  
		Last Modified: Fri, 06 Oct 2023 03:10:01 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aeaafaabc69786b92a359189e818beebb6a360814c3e999bf3db230c17d879ec`  
		Last Modified: Fri, 06 Oct 2023 03:10:01 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8092c0fc72be27afed2a70aa5c8c02e161c4621a9f020f3779a23c9874bd3b`  
		Last Modified: Fri, 06 Oct 2023 03:10:01 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:c00e137f6525078741710c5d974f37ba92dbf186ebaa2d40cda393509d3fa5e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5577135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a154bf981adda79055af7e25c77c664937c1dab90f233b5908e262be724367`

```dockerfile
```

-	Layers:
	-	`sha256:bb118c740d1e7a7334b479b970e3f83b663ed5b99992ccd57985811c81550658`  
		Last Modified: Fri, 06 Oct 2023 03:10:00 GMT  
		Size: 791.2 KB (791167 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:dabe55afa496202f067474e5b826fe3334eace20d10360dc1a3ca8f40ee48b49`  
		Last Modified: Fri, 06 Oct 2023 03:10:00 GMT  
		Size: 2.4 MB (2358902 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:153e15da5d55455dca234809fa3c19b50dff42ee62153635b91d28f6e05f6448`  
		Last Modified: Fri, 06 Oct 2023 03:09:59 GMT  
		Size: 2.4 MB (2357956 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c175790f72f95df7b767fb78ff6c25d2e575ee824e50eddca7b4351e28a949e4`  
		Last Modified: Fri, 06 Oct 2023 03:09:59 GMT  
		Size: 69.1 KB (69110 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:df6ba4d659206661f72d720f88b8be7e1d7d60458e7f618aeab98feaf0ef26e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62418432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b49293b360dc942a895c9cea9efec7c7ee3a8e79f485bc972f16e6f2132b1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd40bad1975f6f3ec6ac5d8ffb1f47c7ffc0efb83d84b0c72d0b05a66ae05f7c`  
		Last Modified: Fri, 06 Oct 2023 01:07:17 GMT  
		Size: 32.6 MB (32623535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a132056f079eddf9120516df83031b40a9e8df1df923a580720df7d78b4f3bc1`  
		Last Modified: Fri, 06 Oct 2023 01:07:14 GMT  
		Size: 388.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b306063e977ab534dfa842abcbb48dfb1de9c450cba8724bd32d186fb1e8ac18`  
		Last Modified: Fri, 06 Oct 2023 01:07:15 GMT  
		Size: 7.4 MB (7437036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7ffe6ee2e97bd83ef9bfb73052ef7047bca1032b594e67dd0625d170384caef`  
		Last Modified: Fri, 06 Oct 2023 01:07:14 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c99855826b752d60a87ab9f7aa237887872a99048dc4d71286f68e7267f4bdc`  
		Last Modified: Fri, 06 Oct 2023 01:07:15 GMT  
		Size: 1.4 MB (1401888 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48a7265edaaf7856720eb841ad5e98e8c3c115425b9cd6b9ddf1f80550cc7df5`  
		Last Modified: Fri, 06 Oct 2023 01:07:17 GMT  
		Size: 17.7 MB (17717692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63a62150e8d7eeeac4a95694162b8b697112c16eefee28885793b9e9594074ce`  
		Last Modified: Fri, 06 Oct 2023 01:07:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e9cf4ab27ff7f3bda3c4031185cf5d92429c40b2cf9d0b9d65a9d86963f8592`  
		Last Modified: Fri, 06 Oct 2023 01:07:17 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b222e41248689af23835ad500f5f1ea782339dc92796676f0d5f15f3e9770cad`  
		Last Modified: Fri, 06 Oct 2023 01:07:17 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbff2bdf4faa5e7f3cc3a9d7a5d42607c90f3129384a2ab5f4360afbd4baf0b4`  
		Last Modified: Fri, 06 Oct 2023 01:07:18 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:7e387611bf9bc081105fb061a4512ab437b1ae0debff533bdaa4f85badae70c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 KB (69000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dc25e8f8e7bd2fcc0580bb8fccdf472ae1c723ba6046adc3a67d61c6a5c07ff`

```dockerfile
```

-	Layers:
	-	`sha256:a2bc64baa09caad614ddb443619a8cefd185dcaff2bb43bf3e79940c9ab40842`  
		Last Modified: Fri, 06 Oct 2023 01:07:14 GMT  
		Size: 69.0 KB (69000 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:c5a2d5f77410eec9e5b87fdd75eba32d8316a6b1be8b8232445ad7747b162155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63346116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ced11c3a119aefe56f4f2283fb143629eb152dfa784555ee84aaa6ac8c6ef8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45ea48fb8e2adea535eac2d1ac17f729c5f4092d101c43ebeaaf612f0c0e9120`  
		Last Modified: Fri, 29 Sep 2023 07:11:56 GMT  
		Size: 32.8 MB (32805323 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766dc9f4c739405f9a410dacf5098521b1b8b5bea710de307e9ff1304faa0a9e`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 398.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15922f80bef06bb8169e1468ebdae2d549efdffdbf3e07941ce07a2ed5e8740e`  
		Last Modified: Fri, 06 Oct 2023 04:19:10 GMT  
		Size: 8.0 MB (7951791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c883708fffb9e9035bd6d114f0d9393306fb85e8a918842374e43109eedf6279`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f867e6069a3917799e1c0994a80120541ffc03b2fcd70db94659589fdc05ebae`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 1.5 MB (1522264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3dcc64599ea5065f97b8876559f0b6e359e18b247f136f9a7a239adfa0bf0ccc`  
		Last Modified: Fri, 06 Oct 2023 04:19:12 GMT  
		Size: 17.7 MB (17717687 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:35b01a2738bfd9b4b66e387f05fbba579fcbabbf671a4b0b44822d69243839a1`  
		Last Modified: Fri, 06 Oct 2023 04:19:10 GMT  
		Size: 192.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab71f9025f12bfd6683781069b35342813665864c326ded955397a707a8d0286`  
		Last Modified: Fri, 06 Oct 2023 04:19:10 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f86ee85ed2b43cec5cf5aaa0983b4c9cd0775b506f84f949d80035789d12af7c`  
		Last Modified: Fri, 06 Oct 2023 04:19:11 GMT  
		Size: 624.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bffc78690dc4f3c9f85ec99da390942ea10b4de450711f51932ec9412fca9da`  
		Last Modified: Fri, 06 Oct 2023 04:19:11 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:1c7fa452455a78df3c573a558b3276be09280d8597a7e9aff07898d813b6ea3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5527318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c22c89dd31d043b991706a0edee7ed6679e4f327ac6334863bcd2d5ab396415`

```dockerfile
```

-	Layers:
	-	`sha256:47fba86d59a4071a78ee9c0c10d29df55d6aaf07d4fb7c4714a1dbfa054abec6`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 785.3 KB (785254 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3ad6a39c5944c37cf1945cb01e18d42e6babd2e74a4c247b3553796992362eb3`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 2.3 MB (2336925 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:27d46558771277456cf044531d7cde67636d5327ee625cf9e0dcecd9b0af2d6f`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 2.3 MB (2335979 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:60eddc783b51ed56ad2560152d72be874edda97c5901eef39738d4ce038a57ec`  
		Last Modified: Fri, 06 Oct 2023 04:19:09 GMT  
		Size: 69.2 KB (69160 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:37a7bf6fdc3d614f0a644721f01c8619ffe2338c4bc99f9147fb37453953fcb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61336616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d74a9b4cc41858982be77f2f256a568bce6f9c6b17790e3ea5b712e503c2f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Tue, 03 Oct 2023 23:45:42 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.6","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.3","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_VERSION=3.12.6
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 03 Oct 2023 23:45:42 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:45:42 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.6","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.6?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN su-exec rabbitmq rabbitmq-plugins enable --offline rabbitmq_prometheus # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
RUN ln -sf /opt/rabbitmq/plugins /plugins # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 03 Oct 2023 23:45:42 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 03 Oct 2023 23:45:42 GMT
ENV LANG=C.UTF-8 LANGUAGE=C.UTF-8 LC_ALL=C.UTF-8
# Tue, 03 Oct 2023 23:45:42 GMT
COPY 10-defaults.conf 20-management_agent.disable_metrics_collector.conf /etc/rabbitmq/conf.d/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:45:42 GMT
EXPOSE map[15691/tcp:{} 15692/tcp:{} 25672/tcp:{} 4369/tcp:{} 5671/tcp:{} 5672/tcp:{}]
# Tue, 03 Oct 2023 23:45:42 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f86917adcb065022f143f482b32276bda784cf8021acbfe99aac4e672db7fabc`  
		Last Modified: Fri, 29 Sep 2023 07:13:16 GMT  
		Size: 32.5 MB (32478704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1c02c9cbf01be90d834c4ac899a095e0afcd7a6fe58b21de2035e6de0f6cee0`  
		Last Modified: Tue, 10 Oct 2023 07:54:15 GMT  
		Size: 398.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cacad9fa9866a32242495ce072adaff7b02a2cb49b4695a079b1a031e297f259`  
		Last Modified: Tue, 10 Oct 2023 07:54:16 GMT  
		Size: 6.4 MB (6427067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb27c520ceb757b5e3b4b3446098b03f33381f2f43ac75b5f39855fe4d5f0f54`  
		Last Modified: Tue, 10 Oct 2023 07:54:16 GMT  
		Size: 389.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4d81daf3542ccaa09c72d4ad58bfbad5da984f0713b22fc582a941a674d2f9a`  
		Last Modified: Tue, 10 Oct 2023 07:54:16 GMT  
		Size: 1.5 MB (1495539 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8231dde68563eed3c4f2569610fc2a47087cd6b7c8bd24c60ccc50c9e09de1ec`  
		Last Modified: Tue, 10 Oct 2023 08:12:41 GMT  
		Size: 17.7 MB (17717664 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b7b23d52a2f1241e835c78920c2b5172a9da5a089a79d5c44f22505ab5fa8f0`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61a8ce78811615b6c30a1d69001a9726cb822905f782f564bf4840d2b18c4c9a`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e716d1dd646f2070a69375845a9a28e9f388950669fc02c4d12b4ee71657efdb`  
		Last Modified: Tue, 10 Oct 2023 08:12:40 GMT  
		Size: 623.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30ec4ef42558c591ee062e43002530cf274af79e1ef18feb88ed342a23855fee`  
		Last Modified: Tue, 10 Oct 2023 08:12:40 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:3-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:2f9db5d88f6e7ccacb59237380292c80dcf52d33916846d66c46c896cbbb86ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5349696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8959e3b1f57865bb6b610e68475992f3444caa1adf9738cd0529fe9ce6adf9`

```dockerfile
```

-	Layers:
	-	`sha256:49cf2caf8f9c52c5a42118f851e505416bead5df35a13e24e2a33ffb073f61e0`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 785.2 KB (785208 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1a24e97bfc779da058a75773909876a8c142ca07f82bcb719f1158caee61310b`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 2.2 MB (2248167 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e106651d107c2ee4d4146316ff93edd7fa8ea1f88ecb4ea8903b91b830a174b4`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 2.2 MB (2247221 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ccbb47a0f68b2d857dbba8027acd589fe34b54e82ee25e71f77dc8895ded5ac3`  
		Last Modified: Tue, 10 Oct 2023 08:12:39 GMT  
		Size: 69.1 KB (69100 bytes)  
		MIME: application/vnd.in-toto+json
