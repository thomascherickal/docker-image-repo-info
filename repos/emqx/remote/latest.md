## `emqx:latest`

```console
$ docker pull emqx@sha256:cb6daea8f3ec82829550982f158cf8cab692f9f4132deae6f5fb313d13e1ed7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:f356cc67a765ca1a8f061357a4f2a642972013633aa430dabb63714d27a025ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124846626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690157a23d6d16f7a0018e067eb70e3dd47d21343f1ab306b016b698618820b8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:14:37 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:14:37 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 12:14:37 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 12:14:42 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 12:14:47 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 12:14:48 GMT
USER emqx
# Tue, 15 Nov 2022 12:14:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 12:14:48 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 12:14:48 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 12:14:48 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 12:14:48 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9361f46d474c278613330bf20b7b1264c2eec81c3e1f05e78b21aa201437a7`  
		Last Modified: Tue, 15 Nov 2022 12:15:15 GMT  
		Size: 2.6 MB (2571046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f847ee13842a669d2f625effb83a707e818d3cb509e2f4eed1ce3a7cd79db896`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45424513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0fe5c47919417828878227ee16596985e496752ae09305250f4553c19fb83d`  
		Last Modified: Tue, 15 Nov 2022 12:15:20 GMT  
		Size: 45.4 MB (45437332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb804a2f0e054f72cf8ec813e7913c1ef5fa5099d7c163aacd340aca87dd6c`  
		Last Modified: Tue, 15 Nov 2022 12:15:14 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:b96eb9baf9f59f5524f82adfbe01e9ef5c01e081bb4b7b61847de59a7ad562fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110236571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6eebb68d3555822f6610bc02400972790c4e0f2bae2ba0b827e1618e38ac76`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:13:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:13:29 GMT
ENV EMQX_VERSION=4.4.4
# Tue, 15 Nov 2022 06:13:29 GMT
ENV OTP=otp24.1.5-3
# Tue, 15 Nov 2022 06:13:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="74a65d51ab60b044874f98e1dc4022f2932c7d70e68bc13ed5fe43be177ba515"; fi;     if [ ${arch} = "arm64" ]; then sha256="6aed1583bf96b53e6355e7431204fc8b09b89ffbce580f5031a77a542c53c5e8"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Tue, 15 Nov 2022 06:13:36 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
WORKDIR /opt/emqx
# Tue, 15 Nov 2022 06:13:37 GMT
USER emqx
# Tue, 15 Nov 2022 06:13:37 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 15 Nov 2022 06:13:37 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Tue, 15 Nov 2022 06:13:37 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Tue, 15 Nov 2022 06:13:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:13:37 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad108ef5d5673e32622aa158fbc152df7e8c340c7f4e79efffecd4c5d6c2a7be`  
		Last Modified: Tue, 15 Nov 2022 06:14:09 GMT  
		Size: 2.6 MB (2560816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96042e2ccd2609d9b280266d2cc3063aab600802b597ec18244c2761f3af513`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38806727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b8a52dff2f8fc12cecf2988e77261a173d791f10a1ccedb107ace30b8fdf0`  
		Last Modified: Tue, 15 Nov 2022 06:14:11 GMT  
		Size: 38.8 MB (38807317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4504a627c078e5f88f9616bd61b3f0074e95a846d4bee00e1e4f6024bb61244`  
		Last Modified: Tue, 15 Nov 2022 06:14:08 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
