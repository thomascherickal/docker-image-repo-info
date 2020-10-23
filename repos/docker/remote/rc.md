## `docker:rc`

```console
$ docker pull docker@sha256:781c78fee5c3f339912b38f3c1245c686697dc52107f30637f1d1ffd21e2a335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:9e48395e522e824f372b08cd9493698aceee59f877b155d032b441ad3f36cd78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73670183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d7562490102a554243c83faa61f325fdca9dbba375b450fff57c56616ccc24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:15:43 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 03:15:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 23 Oct 2020 17:16:56 GMT
ENV DOCKER_VERSION=20.10.0-beta1
# Fri, 23 Oct 2020 17:17:04 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-beta1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-beta1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-beta1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-beta1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 23 Oct 2020 17:17:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 23 Oct 2020 17:17:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 23 Oct 2020 17:17:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 23 Oct 2020 17:17:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 23 Oct 2020 17:17:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:17:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c675703d60dc4d757acb40557350159f600ca3d49e2e8d4c2039dd6b69457`  
		Last Modified: Thu, 22 Oct 2020 03:16:47 GMT  
		Size: 2.0 MB (2039054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8c12a437cbe4e104dcea425e0ce277a2442603e14551d22a948e11026ae658`  
		Last Modified: Thu, 22 Oct 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06d45f08c7f56239d3fb96575b77c0b29e69e6ff79621cde9e8363e56667f84`  
		Last Modified: Fri, 23 Oct 2020 17:19:01 GMT  
		Size: 68.8 MB (68832435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48baaff01cbdfab0e1c2263cc7d711d5aa917c1449880a72cc28b711ab5bdc`  
		Last Modified: Fri, 23 Oct 2020 17:18:47 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194baee72433a4e99ac86886684bfbab5e7b5656ff117f35440659b6587d5177`  
		Last Modified: Fri, 23 Oct 2020 17:18:47 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd9003061ceb8bc738deb30262eb58e6fd46a84c93d5067daea433238615c02`  
		Last Modified: Fri, 23 Oct 2020 17:18:47 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v6

```console
$ docker pull docker@sha256:b50cd9618f77ebb37c77bfbc7159787900f8449bff5ebd16ef4314439e1905d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64876994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996aeccdec0200978b3055ef8f213be775fcfb814206e90b5f451dbf28002f11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v7

```console
$ docker pull docker@sha256:eb32cec8343a12b521cc18b3f20bd834c93fd78d5ad364ae5f16375d396a2d9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64565553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d565c546476b27e22955e7eba0558a217cdec7677161d7d758e8e5a484873a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:f8ecea9dc16c9f6471448a78d3e101a3f864be71bfe3b8b27cac6df83f6f0970
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67756329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709df7468e2c5fa5d12e00c74be9153146f423f1c390a02afaf540c893be7dd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:50:30 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 22 Oct 2020 02:50:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 23 Oct 2020 17:16:38 GMT
ENV DOCKER_VERSION=20.10.0-beta1
# Fri, 23 Oct 2020 17:16:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.0-beta1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.0-beta1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.0-beta1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.0-beta1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 23 Oct 2020 17:16:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 23 Oct 2020 17:16:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 23 Oct 2020 17:16:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 23 Oct 2020 17:16:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 23 Oct 2020 17:16:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:16:56 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db56a0506354d758e7aa37b41ef4fff997520e3bad443abf5a31e7e71d779f`  
		Last Modified: Thu, 22 Oct 2020 02:51:51 GMT  
		Size: 2.1 MB (2061246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb67d6aeaaac2f2df73d644bd7912b4e92743c2520751feb04af77d3c76ff5b`  
		Last Modified: Thu, 22 Oct 2020 02:51:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5aa244033afce57d79e9c6cdc610328b716bd18bafe31a76f67a3aa57e952f`  
		Last Modified: Fri, 23 Oct 2020 17:18:33 GMT  
		Size: 63.0 MB (62986663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb903437417c7228c0f714227d87fc017f81cde6d8f9bac6ccf446379943842`  
		Last Modified: Fri, 23 Oct 2020 17:18:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d0e94618c50c46717cac6b14ff0f8b1d695b5d967cb0c131783d15739128e3`  
		Last Modified: Fri, 23 Oct 2020 17:18:15 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4c68a1425f7fc3b97908e877de6f61f10cbaec70038d7015e325c993dccbf8`  
		Last Modified: Fri, 23 Oct 2020 17:18:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
