## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:59db6d0f170c6af671689ed19b09212b86839befadf95257625d83d571878de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:0de05f9de162e737bc9e342d449d08b910cf5db394e94aaf03c3827ed668c525
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fc16f9d95d271337d111d9fb9e0348f0733dd1fad3c8cbc9597d7b9ba1b93c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:12:57 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:13:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:13:52 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:13:53 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:13:53 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:13:54 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:13:54 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:13:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:13:55 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4017e5d7a7432ffced49eca070dc7fae5e805eab6df288dedec4b65f6c9aeaa2`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 2.7 MB (2685092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e8e40a7f6fe8ca5e371cd3a187c0ea43e8687ed1593900de6d2570b050a5b`  
		Last Modified: Thu, 17 Dec 2020 14:14:19 GMT  
		Size: 3.3 MB (3285726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870293c10157a8f2f2f93e5a3c71633812d3c83d407b8b2fbe7a7f52d86493dd`  
		Last Modified: Thu, 17 Dec 2020 14:14:17 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4404ebd7ec8f77adc5a6d9a63a69c1bb3088e84489edd900db81353cb47a26`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
