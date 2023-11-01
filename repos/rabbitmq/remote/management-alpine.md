## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:c95f6e3e5a18e873a0c489a40acfe6aa31f3dae0de61b667e3339fec77f77f53
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
$ docker pull rabbitmq@sha256:82925ed7d3b262265342d8847d2abccc4dd62f0431b499dde81ca9c3ea762e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86160024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5409acbcc5d75c72649b0ef8c82df1f103f83949090b8d0bea214d01c81fb7f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.8
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9dc2c9b3c2de43c34e4dd62b97f541ffc136a5422c4996ea0d25bf44832211c7`  
		Last Modified: Wed, 01 Nov 2023 00:09:19 GMT  
		Size: 40.1 MB (40076558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5157da1e8ca98222e84293df9eab3e3bb02e7c6cb8a498906f99c63f1b1262aa`  
		Last Modified: Wed, 01 Nov 2023 00:09:16 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:288fac1a35533742296fca957bbfd03fa38fe47c02a4a96e32e06e39b51b19b3`  
		Last Modified: Wed, 01 Nov 2023 00:09:17 GMT  
		Size: 7.6 MB (7550197 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0313f95ed1600d55368a10306c2be61fbf190597cb59750cb535ab9b8692443c`  
		Last Modified: Wed, 01 Nov 2023 00:09:16 GMT  
		Size: 389.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a69e8b2423c07af00f2dec633450d3dc2a96d5d23dbdf4accad25bb2d844873f`  
		Last Modified: Wed, 01 Nov 2023 00:09:18 GMT  
		Size: 2.3 MB (2297409 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b1350d7409b4c129a0f655e40b44d4a8e5ba48ac63248004cfc7bcdbaf4cf26`  
		Last Modified: Wed, 01 Nov 2023 00:09:18 GMT  
		Size: 17.7 MB (17729258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:78900cd8a4d4d1fd1341713351179aaa49c1d0209b4df869e4ec6bdfa421f0ed`  
		Last Modified: Wed, 01 Nov 2023 00:09:19 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:099df3e252d91393417ae6dbc703ec0c3fa6d5dd6f5ae5d66f233063fb5da241`  
		Last Modified: Wed, 01 Nov 2023 00:09:19 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:426ba31af342aa654693949784f15422366cd739fd2316195f2891ba2a90be82`  
		Last Modified: Wed, 01 Nov 2023 00:09:20 GMT  
		Size: 618.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33353d368cf915d5d7f30057bf13d3c2875c29a0c07f68a52f87795c626b93dc`  
		Last Modified: Wed, 01 Nov 2023 00:09:20 GMT  
		Size: 831.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db8fcab1c58ec1788d9a003a36ce5972383f05a1f7ae077cb372df6d0338c023`  
		Last Modified: Wed, 01 Nov 2023 01:02:33 GMT  
		Size: 15.1 MB (15102104 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:6377e9eadc0de006e9fc1281e4ea4edeb499643292d228262f058c477fcba0d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 MB (1664652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ffafd2327edf8747bf5e5c972047fbae29fe5ce7f4e1dceffea5f5a41bec568`

```dockerfile
```

-	Layers:
	-	`sha256:50bef105b45b76e441eba8fdd2be605c3766c830d32c838533708f9dc7824e34`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 1.7 MB (1651175 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5b59b5384f7116589cde133f0fcfa744a0784d3f375b020c9e0300d91f51ae0d`  
		Last Modified: Wed, 01 Nov 2023 01:02:31 GMT  
		Size: 13.5 KB (13477 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:7bc1bd7e8843eb6cf12fa45599d959dbdf68b2f8a3ccee42ceb2666086429ce4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76695442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9afce878923a38b0a94657a5611f0804d5ab3d1b1e5e444a3b4bb226322792`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.8
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b05de52c518eafc854587c546fb6622f496b882d90b7a2ed47c08d91eb41e8`  
		Last Modified: Fri, 27 Oct 2023 17:09:49 GMT  
		Size: 32.4 MB (32388988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caaa232c0eb9e703f5d0b314525727cd6bccec33ea17d7674977eadd4cd38b56`  
		Last Modified: Fri, 27 Oct 2023 17:09:44 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa975259a2a63b60c4eb7818a4ad0540995a4ef5047104fe1b556d7b7e9c336`  
		Last Modified: Fri, 27 Oct 2023 17:09:45 GMT  
		Size: 6.4 MB (6382898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9767d780bf5584c2cad3cd9abfd5d52313fd1321c68521650ec773016a6d315`  
		Last Modified: Fri, 27 Oct 2023 17:09:44 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc30bd075c6c3a5b88f28da3f248d6a109536e6f95efd4d0dbb720bce8ef034`  
		Last Modified: Fri, 27 Oct 2023 17:09:44 GMT  
		Size: 1.4 MB (1412520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a84920928da45dd0252663ec61762062095dda3a9972d543fe166621c8e8879`  
		Last Modified: Wed, 01 Nov 2023 00:02:04 GMT  
		Size: 17.7 MB (17729169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d3b4cfe8f5ad5a6d9950b8cc368ec3c4fb267ece5d4f6ccfad88ebffee5dd4`  
		Last Modified: Wed, 01 Nov 2023 00:02:02 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13914b3b4c9636477960ff8cd24e9fe02d3f345c260185ee8f1be38d5a37a7bb`  
		Last Modified: Wed, 01 Nov 2023 00:02:02 GMT  
		Size: 109.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f31230d875dff60fe11ad156baf46f885e4182fdd2a1587f57f4a76a6740e6c`  
		Last Modified: Wed, 01 Nov 2023 00:02:02 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9a2a33a60f68e2f14785808a893b76a681cb553b535180429435d22221368a`  
		Last Modified: Wed, 01 Nov 2023 00:02:02 GMT  
		Size: 828.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631d918dbc2aa6b6bac67ee93999d8d9f41009492c6e82b959da81930a6c1414`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.6 MB (15634054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:42c9e74867b7107c5f2cba2cdf011c7144705d1d06367ce7821a809b5f77e5ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75532967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc70b95892a34a41e175dfed2547cd3ecc72f7b3c45dddef2ede09e4f8a3a8f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.8
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7f57e652bf551759f9169cf7cbc65a05f05678d004fb4ecf84bbcb2ce36eb87`  
		Last Modified: Fri, 27 Oct 2023 17:51:19 GMT  
		Size: 32.3 MB (32271017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f327defd88b9aa4fddd69dee7ffebd3b13314b7841fc6c136fa4838e309016d`  
		Last Modified: Fri, 27 Oct 2023 17:51:16 GMT  
		Size: 394.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f463091713f46b393a8ec9a3be629a5c67b73263f8d101dd87a6ec7599de0249`  
		Last Modified: Fri, 27 Oct 2023 17:51:18 GMT  
		Size: 6.1 MB (6082548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9385564d576ce6ba34e74067f4819742b82ac5ab8f4fa3f3b39834b27d0eefe2`  
		Last Modified: Fri, 27 Oct 2023 17:51:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f4080c6f809b4aadf1a7dcb3b7042f5ba8d014b7e1bf1128277f41807cb4db2`  
		Last Modified: Fri, 27 Oct 2023 17:51:18 GMT  
		Size: 1.3 MB (1300444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c9193feaf6bb1af2dbf9bf53e8422d887926351676154e5d13109c5340764c7`  
		Last Modified: Wed, 01 Nov 2023 00:19:13 GMT  
		Size: 17.7 MB (17728973 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27775173ad00109046d30995c27a6133c4eabb248c4b6b618cb0c5f54ef7c688`  
		Last Modified: Wed, 01 Nov 2023 00:19:12 GMT  
		Size: 191.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:029c0fddbc26b50fa080a5df5e0b03032eb4a9685d10a65f72daa5c817b491a4`  
		Last Modified: Wed, 01 Nov 2023 00:19:12 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:041069165a1bcc1cee7193b3f227a868216266f26fab6d3f9781c2658b8f8009`  
		Last Modified: Wed, 01 Nov 2023 00:19:12 GMT  
		Size: 616.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d5b93db94b160b74d9bf4e99b4c5349e088d98942baedfe2e0daa03aca08339`  
		Last Modified: Wed, 01 Nov 2023 00:19:13 GMT  
		Size: 825.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91bd93c81d557f57c1e6a95172ae79f9b0e291cd7b4647ac2bb8e88f21f363e8`  
		Last Modified: Wed, 01 Nov 2023 01:18:58 GMT  
		Size: 15.2 MB (15247555 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:99f20212cb8969c788173800e6aaeb24b29136c6dd585827212ff9292e386cac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 MB (1665037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9e5bfe55a8b21a9c7844f82dbd17a297b562a04d3ac9c9f132fbb121f2c70c`

```dockerfile
```

-	Layers:
	-	`sha256:914a0df38ecefe6a3294261de890ae6ef140800551b2bb355dadfd3996ad300f`  
		Last Modified: Wed, 01 Nov 2023 01:18:57 GMT  
		Size: 1.7 MB (1651466 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a0c16aebfb979a684cd9a577faa6d5c255071208a8006382b379cfc1a5f79ba8`  
		Last Modified: Wed, 01 Nov 2023 01:18:57 GMT  
		Size: 13.6 KB (13571 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4c40d46d5df5cdebf34afc87430ac45bf7ba14c83a7f0b6b19ba5019cd15e982
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83710700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb925ae45ecf51f8750cd0315291196d61767d4227f6318f353b9ee2d9c2d2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.8
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:196d3fd38f39c8756a92c06767d0da13ac0823d00198f79d9bce4fe20e2a3a6a`  
		Last Modified: Fri, 27 Oct 2023 17:52:52 GMT  
		Size: 37.9 MB (37874049 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf86d5275580d5e06411a30f007c63c83d1a18d534bebfaa25bde9157037a08a`  
		Last Modified: Fri, 27 Oct 2023 17:52:49 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99910fe121b7470d23958b20a4288b048b92ec93dc5bfadbd8e8091998e5afba`  
		Last Modified: Fri, 27 Oct 2023 17:52:50 GMT  
		Size: 7.1 MB (7147436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f1b5b553370dd9791261eb07815e1a7b5468dae1f8a95d4b73861744cbac6ea`  
		Last Modified: Fri, 27 Oct 2023 17:52:50 GMT  
		Size: 387.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89b81e0e6313a3ead53ce1edcedfe133674e1a67e490963067c485e9d6d24ff7`  
		Last Modified: Fri, 27 Oct 2023 17:52:51 GMT  
		Size: 2.4 MB (2368792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2136024e99cfd239a9760962256bfd1dcb8e900048750de163f1b748d89e8302`  
		Last Modified: Wed, 01 Nov 2023 00:15:15 GMT  
		Size: 17.7 MB (17729211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e12a008ce383bcbdd7edec32966140016a22fb7da24e8712b51a6cda262c2a47`  
		Last Modified: Wed, 01 Nov 2023 00:15:13 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c0392a14097a4d7ed650a36fc820c3077f6a8f0ea47c1497bbfbc0840e61c47`  
		Last Modified: Wed, 01 Nov 2023 00:15:13 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:344604bc6298f0d94d8c6757fe188c85b675f94f6ea404db408eac20654bc70e`  
		Last Modified: Wed, 01 Nov 2023 00:15:13 GMT  
		Size: 615.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40438117456a8dd725965588017b97f019ed4410aaa18f721d6185d76a38dae8`  
		Last Modified: Wed, 01 Nov 2023 00:15:14 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f515ba4c58d72725fbb1eeff8af48fcc35cdd4233a234c56f69f3eb84d3fc4a0`  
		Last Modified: Wed, 01 Nov 2023 20:27:28 GMT  
		Size: 15.3 MB (15256860 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:febbc0e2b0824e0a53ec1a08872cff7b0b3711a1a8c48d056b8220bf2510baba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 MB (1664782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d254b21646dd186e625f06593c9d182c6ea95835fe9b8d69d7db843c659bc969`

```dockerfile
```

-	Layers:
	-	`sha256:a19b140c67860338e72d8c5f971da7d287b976d02305acd178c47d086a780699`  
		Last Modified: Wed, 01 Nov 2023 20:27:27 GMT  
		Size: 1.7 MB (1651271 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:dfe92ff8f133b1b6827a05e931b0b5bd28b88b2128ffc97b4bc8ed7272f8b933`  
		Last Modified: Wed, 01 Nov 2023 20:27:26 GMT  
		Size: 13.5 KB (13511 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:f5611ca66c24c134b5121543b53c757db49048c33830d8daaa3ad8bfa2c68a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78717112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c0faba96777fd04eabccd08a17410bbc82450dc7e8beacbdde895719d2d88c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.8
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.8","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.8?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7084bb4371909a4112132e957798d4b5e7b50751077d645e59cd3604215428d2`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 32.6 MB (32624623 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebc02584d5330d01f3c7b0339d95c22295337150e12f43414aac19939a818970`  
		Last Modified: Wed, 01 Nov 2023 00:08:54 GMT  
		Size: 389.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26efdf331dbe9ea75e002721b8d804e79e40472c57b073a422f626b66d803e06`  
		Last Modified: Wed, 01 Nov 2023 00:08:55 GMT  
		Size: 7.4 MB (7445765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d95f283ef0c9903e04c158f080244f27a16e718c75e46ecb2bca266f1d959cbc`  
		Last Modified: Wed, 01 Nov 2023 00:08:54 GMT  
		Size: 391.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:881f1f4cc75515fc575c3ceb089acc544fc52d98e4a8f8a55ea230ef30f95342`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 1.4 MB (1401887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccd41d86339012cc649dd94138a2d35fb741e45f0e9221c50a2256b939c52426`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 17.7 MB (17728923 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb867b3c114cf41c2f851556efb691b881687e838c3439ec1620e3c9fda0c4d6`  
		Last Modified: Wed, 01 Nov 2023 00:08:56 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ad88ac80f833d6d54b077df19944255557c71944bff93520129310b5306e5d`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e29799fc2d6f3831bf629ad3a67bdf208589d60e9c51490c5303aee3552ee66`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 617.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e90f15fca4ec148efcff160597b9826ac8803fa5519930724b93aa08e95f48b4`  
		Last Modified: Wed, 01 Nov 2023 00:08:57 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69210e79347dacbe9a51b713b7e26819b1c7e65f2e66b891dfbab0f54af92d00`  
		Last Modified: Wed, 01 Nov 2023 01:02:37 GMT  
		Size: 16.3 MB (16277631 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:9161e75bb62e32b85db22c4adc83bc8d72c4f2766b8f7ea752223bba658edfec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 KB (13230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1973ad0948a008cd43940f11669cae3ff18456333fb7225613a72fb642177a34`

```dockerfile
```

-	Layers:
	-	`sha256:e36ca4431dbfb63bf65777469a1eb4d71023606a204215c01e001de62f5ba2f7`  
		Last Modified: Wed, 01 Nov 2023 01:02:34 GMT  
		Size: 13.2 KB (13230 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:a3036d001e7e155cf4b254b3c56c3dc387490753f171333f6b88bc37907742c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79684978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382ec494dd446d195656401e3494fecae39b16e1624f283f96735d8323aecfb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.7
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.7","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c683d3bbe8f22650d7212d298915ede8a21140c201e6ca5071a45567baba24af`  
		Last Modified: Fri, 27 Oct 2023 17:36:46 GMT  
		Size: 32.8 MB (32804837 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a763a9de36c15c741c7d357e1c5c520eaff5a227df81f070bc5a0efe2bb5dc0`  
		Last Modified: Fri, 27 Oct 2023 17:36:43 GMT  
		Size: 395.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e236127e7ef69fa54b3e90d87f61f0cf35855c0d23d1462f90a88e7c49a9e3`  
		Last Modified: Fri, 27 Oct 2023 17:36:44 GMT  
		Size: 8.0 MB (7960983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2de82464687dcdcea1488224511aaab7c076f9064c4a3104da89b19bc1184d6`  
		Last Modified: Fri, 27 Oct 2023 17:36:43 GMT  
		Size: 393.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed0b96369929775d635052541ff0f4ba42e95cccb22aff4a37b9a18475109b7d`  
		Last Modified: Fri, 27 Oct 2023 17:36:45 GMT  
		Size: 1.5 MB (1522239 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9cddb8dffa81068c72b905efe9008e4da7a4ff6c9f1beb14834d9052d9791a4`  
		Last Modified: Fri, 27 Oct 2023 17:36:46 GMT  
		Size: 17.7 MB (17722826 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ee8c320b491cb56f202a2b4cc6c710fd1ca3900258a618fcc26b363762188df`  
		Last Modified: Fri, 27 Oct 2023 17:36:45 GMT  
		Size: 193.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1651c1e30426f497148f9067e0b187d9ee29de8df8d83d8e8dfe6366f14f4ec8`  
		Last Modified: Fri, 27 Oct 2023 17:36:47 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:674928aa0f525700782f6a0ea000de116dd57fdbf570d370f001e433c35c2228`  
		Last Modified: Fri, 27 Oct 2023 17:36:46 GMT  
		Size: 625.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f047d5560c6178b862de678e168f06e08a62e72ec604d9eb251ada551167a40`  
		Last Modified: Fri, 27 Oct 2023 17:36:48 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a84d2c82ac7e1efff518bac8b7606c8789a0beaac45e2d4c703c765c85c1557c`  
		Last Modified: Fri, 27 Oct 2023 18:15:05 GMT  
		Size: 16.3 MB (16325041 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:07d4247a60082979576aaa03b02fed0a9d8b52540e748977f2d6c6f6b372ecba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 MB (1663535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75616b54134d1a027a75b141920af8a00c5b326b8539642b50de9a44806149a5`

```dockerfile
```

-	Layers:
	-	`sha256:cc7d865fbe5193b6c7bec900cf3b62549a81d8c615c2d9e903d2a31999539dd8`  
		Last Modified: Fri, 27 Oct 2023 18:15:02 GMT  
		Size: 1.6 MB (1649998 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a33f1b8631d8f5322fe972418a1995c450d3154dc9e0394d6b644bc7293694f1`  
		Last Modified: Fri, 27 Oct 2023 18:15:01 GMT  
		Size: 13.5 KB (13537 bytes)  
		MIME: application/vnd.in-toto+json

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:e66804390248c47e245a1aa9958a7afea2375a95643276440c067534ed8ac9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77475277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0313cd2521a9fc6f4f6d06e6beeacf48ba0c6929c3031a5c36b9f97ff2c9d5d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Fri, 02 Jun 2023 21:59:28 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 02 Jun 2023 21:59:28 GMT
CMD ["/bin/sh"]
# Fri, 02 Jun 2023 21:59:28 GMT
ENV ERLANG_INSTALL_PATH_PREFIX=/opt/erlang
# Fri, 02 Jun 2023 21:59:28 GMT
ENV OPENSSL_INSTALL_PATH_PREFIX=/opt/openssl
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/erlang /opt/erlang # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"erlang-sbom","packages":[{"name":"erlang","versionInfo":"25.3.2.7","SPDXID":"SPDXRef-Package--erlang","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/erlang@25.3.2.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $ERLANG_INSTALL_PATH_PREFIX/erlang.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
COPY /opt/openssl /opt/openssl # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
RUN echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"openssl-sbom","packages":[{"name":"openssl","versionInfo":"3.1.4","SPDXID":"SPDXRef-Package--openssl","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/openssl@3.1.4?os_name=alpine&os_version=3.18"}],"licenseDeclared":"Apache-2.0"}]}' > $OPENSSL_INSTALL_PATH_PREFIX/openssl.spdx.json # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_DATA_DIR=/var/lib/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	ln -vsf /etc/ssl/certs /etc/ssl/private "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl"; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive $ERLANG_INSTALL_PATH_PREFIX $OPENSSL_INSTALL_PATH_PREFIX 			| tr ',' '\n' 			| sort -u 			| grep -v '^$\|lib\(crypto\|ssl\)' 			| awk 'system("test -e /usr/local/lib/" $1) == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .otp-run-deps $runDeps; 		sed -i.ORIG -e "/\.include.*fips/ s!.*!.include $OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf!" 		-e '/# fips =/s/.*/fips = fips_sect/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/openssl.cnf"; 	sed -i.ORIG -e '/^activate/s/^/#/' "$OPENSSL_INSTALL_PATH_PREFIX/etc/ssl/fipsmodule.cnf"; 	[ "$(command -v openssl)" = "$OPENSSL_INSTALL_PATH_PREFIX/bin/openssl" ]; 	openssl version; 	openssl version -d; 		erl -noshell -eval 'ok = crypto:start(), ok = io:format("~p~n~n~p~n~n", [crypto:supports(), ssl:versions()]), init:stop().'; 		addgroup -g 101 -S rabbitmq; 	adduser -u 100 -S -h "$RABBITMQ_DATA_DIR" -G rabbitmq rabbitmq; 	mkdir -p "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chown -fR rabbitmq:rabbitmq "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	chmod 1777 "$RABBITMQ_DATA_DIR" /etc/rabbitmq /etc/rabbitmq/conf.d /tmp/rabbitmq-ssl /var/log/rabbitmq; 	ln -sf "$RABBITMQ_DATA_DIR/.erlang.cookie" /root/.erlang.cookie; 		apk add --no-cache 		'su-exec>=0.2' 		bash 		procps 		tzdata # buildkit
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_VERSION=3.12.7
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 02 Jun 2023 21:59:28 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Fri, 02 Jun 2023 21:59:28 GMT
ENV PATH=/opt/rabbitmq/sbin:/opt/erlang/bin:/opt/openssl/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 21:59:28 GMT
RUN set -eux; 	mkdir -p /usr/local/src; 		apk add --no-cache --virtual .build-deps 		gnupg 		xz 	; 		RABBITMQ_SOURCE_URL="https://github.com/rabbitmq/rabbitmq-server/releases/download/v$RABBITMQ_VERSION/rabbitmq-server-generic-unix-latest-toolchain-$RABBITMQ_VERSION.tar.xz"; 	RABBITMQ_PATH="/usr/local/src/rabbitmq-$RABBITMQ_VERSION"; 		wget --output-document "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_SOURCE_URL.asc"; 	wget --output-document "$RABBITMQ_PATH.tar.xz" "$RABBITMQ_SOURCE_URL"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$RABBITMQ_PGP_KEY_ID"; 	gpg --batch --verify "$RABBITMQ_PATH.tar.xz.asc" "$RABBITMQ_PATH.tar.xz"; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar --extract --file "$RABBITMQ_PATH.tar.xz" --directory "$RABBITMQ_HOME" --strip-components 1; 	rm -rf "$RABBITMQ_PATH"*; 	grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -i 's/^SYS_PREFIX=.*$/SYS_PREFIX=/' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	chown -R rabbitmq:rabbitmq "$RABBITMQ_HOME"; 		apk del --no-network .build-deps; 		[ ! -e "$RABBITMQ_DATA_DIR/.erlang.cookie" ]; 	su-exec rabbitmq rabbitmqctl help; 	su-exec rabbitmq rabbitmqctl list_ciphers; 	su-exec rabbitmq rabbitmq-plugins list; 	rm "$RABBITMQ_DATA_DIR/.erlang.cookie";		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"rabbitmq-sbom","packages":[{"name":"rabbitmq","versionInfo":"3.12.7","SPDXID":"SPDXRef-Package--rabbitmq","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/rabbitmq@3.12.7?os_name=alpine&os_version=3.18"}],"licenseDeclared":"MPL-2.0 AND Apache-2.0"}]}' > $RABBITMQ_HOME/rabbitmq.spdx.json; # buildkit
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
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d77b2163ba1a757bf93da3911dbd17becdda540d9226ccbf8c91e3e9401caa3`  
		Last Modified: Fri, 27 Oct 2023 19:15:42 GMT  
		Size: 32.5 MB (32478957 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b95da36a2ad80551437da3d0ef4374b2297eb20cb1ede14e47086aad0207831`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 395.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a57676d109eb9427b6a261221e9c773de3cf251045d6f0bf6049c891b87e9a4`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 6.4 MB (6432210 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923cf9c0996c6d47c2b9a291cf3edccd23f01ed3d7b38f61b48e35fa9dea1298`  
		Last Modified: Fri, 27 Oct 2023 19:15:40 GMT  
		Size: 392.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98cf8de2ab34adb2e862fbf73387b9307c0112125e5cd3ccc377d129238927fa`  
		Last Modified: Fri, 27 Oct 2023 19:15:41 GMT  
		Size: 1.5 MB (1495512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dff1587d1d6da305700e4bac332831dd7e86697a0d827b8956284bf227f91341`  
		Last Modified: Fri, 27 Oct 2023 19:15:42 GMT  
		Size: 17.7 MB (17722780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d6d07c3e2bac4cdce3d596d179f51e6364965adbd67e8cbb4d4d674a0ec40ba`  
		Last Modified: Fri, 27 Oct 2023 19:15:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e0e8a018831373072f1891ecd72816de02691570e5b3709fb01a1085cf431ed`  
		Last Modified: Fri, 27 Oct 2023 19:15:42 GMT  
		Size: 109.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d25bab58cb878466c13dd240d92e9d8219343a04d5a9a6a0ac2e4d0c3099a770`  
		Last Modified: Fri, 27 Oct 2023 19:15:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08b58c74e0fbe1b681eb098d4f603de77e04987bccbc2cfd0b3fc15ca776ccf4`  
		Last Modified: Fri, 27 Oct 2023 19:15:43 GMT  
		Size: 828.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fddf75f1aa44a00b65161a02f1f2e989f4972153c2c48e94a64f9fb10bcd647`  
		Last Modified: Fri, 27 Oct 2023 21:07:05 GMT  
		Size: 16.1 MB (16128183 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `rabbitmq:management-alpine` - unknown; unknown

```console
$ docker pull rabbitmq@sha256:d554f444e592b243d294af37e9efca0f53990f4f8828afaec0f6435dfb84a6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 MB (1661225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70c3c6df6e04e2a267be74e2b5fb4d86389433b0cfd3f3197999d0361483402`

```dockerfile
```

-	Layers:
	-	`sha256:9cc6299a396a037d3a04cfdda9b1e64f30f91f507907380daf85fda0e6d940d2`  
		Last Modified: Fri, 27 Oct 2023 21:07:04 GMT  
		Size: 1.6 MB (1649454 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8dbfd2390aa80880edc3c2f0e7b2580340349d61d6e5a51a732842aebae5f37d`  
		Last Modified: Fri, 27 Oct 2023 21:07:04 GMT  
		Size: 11.8 KB (11771 bytes)  
		MIME: application/vnd.in-toto+json
