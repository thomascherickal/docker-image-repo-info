## `varnish:fresh`

```console
$ docker pull varnish@sha256:7361a7ba9cca13fc4786d26994bc37bd59e8fe449cb772d052db250476c96212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:c333a4834a55237ccb476da1b38ef8145fdfb915878ee659ae1aec36053efb68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77067671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cec6fafe5f4bb23bb8b7044ec76de6ffc7411dd6be4685d202fd2935bb7d08a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:40:06 GMT
ENV VARNISH_VERSION=6.6.1-1~buster
# Thu, 22 Jul 2021 14:40:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 22 Jul 2021 14:40:45 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:40:46 GMT
WORKDIR /etc/varnish
# Thu, 22 Jul 2021 14:40:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 22 Jul 2021 14:40:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 22 Jul 2021 14:40:47 GMT
EXPOSE 80 8443
# Thu, 22 Jul 2021 14:40:48 GMT
CMD []
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0e487938d5f9dea43f192b931a5eb65ec30ba9e7177d5c332c70ebda5645`  
		Last Modified: Thu, 22 Jul 2021 14:41:56 GMT  
		Size: 49.9 MB (49921177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672ff1a28e3a93efb98a9898a5ff8f19112a536cb2c1003b353a4a0133e42a9`  
		Last Modified: Thu, 22 Jul 2021 14:41:46 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
