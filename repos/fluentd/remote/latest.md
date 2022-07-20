## `fluentd:latest`

```console
$ docker pull fluentd@sha256:4f3e8559f74cf2e92940b0ab44e47ea01e22f4292a9f23678935c268fbcc9695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `fluentd:latest` - linux; amd64

```console
$ docker pull fluentd@sha256:0041aa53f7ec368a40a5b01b3019dc3f975d7f07c7381d0dca0f2de0c7078db6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19202602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f846a973029c4ac357617a3758c1d486a2527a927092f1b97c0fc59126eefe`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:38:02 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Jul 2022 23:38:02 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 19 Jul 2022 23:38:48 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 19 Jul 2022 23:38:49 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Jul 2022 23:38:49 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Jul 2022 23:38:49 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Jul 2022 23:38:49 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Jul 2022 23:38:49 GMT
ENV LD_PRELOAD=
# Tue, 19 Jul 2022 23:38:49 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 19 Jul 2022 23:38:49 GMT
EXPOSE 24224 5140
# Tue, 19 Jul 2022 23:38:49 GMT
USER fluent
# Tue, 19 Jul 2022 23:38:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Jul 2022 23:38:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75866a6b2770e8b31f85ea24c051a5c03d492660bcdb35e8cd785471039c07c`  
		Last Modified: Tue, 19 Jul 2022 23:39:12 GMT  
		Size: 16.4 MB (16381070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e9367632bfedf4ac4a7c9a5e1219c31d859c25618f859c28fdf7d15ad0550`  
		Last Modified: Tue, 19 Jul 2022 23:39:10 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20ed5123a37894d4bd3971dfccd5afb27c7d400bf5f9ab2dc070cf6690e0bf2`  
		Last Modified: Tue, 19 Jul 2022 23:39:10 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1766e2df13a984406f9fe6f1b6e46c8f5b370f1a384f62ead15699704ef0c2d`  
		Last Modified: Tue, 19 Jul 2022 23:39:10 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm variant v6

```console
$ docker pull fluentd@sha256:8d1bc7233876f084b3fdaf9201d9f06ceccbd66a2d7a82bc6baed0714ece6211
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18485307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5cfd1c9dd951c0b4875712b55c43357d7453f69119e2b2ee598a2f120d07ca`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:15 GMT
ADD file:19dc757ba128952e4f765f774da40913195379a34f272ac71f3b3a651adf2740 in / 
# Tue, 19 Jul 2022 22:50:16 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 00:14:12 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Wed, 20 Jul 2022 00:14:13 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Wed, 20 Jul 2022 00:16:19 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Wed, 20 Jul 2022 00:16:22 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Wed, 20 Jul 2022 00:16:22 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Wed, 20 Jul 2022 00:16:23 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Wed, 20 Jul 2022 00:16:23 GMT
ENV FLUENTD_CONF=fluent.conf
# Wed, 20 Jul 2022 00:16:24 GMT
ENV LD_PRELOAD=
# Wed, 20 Jul 2022 00:16:24 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Wed, 20 Jul 2022 00:16:24 GMT
EXPOSE 24224 5140
# Wed, 20 Jul 2022 00:16:25 GMT
USER fluent
# Wed, 20 Jul 2022 00:16:25 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Wed, 20 Jul 2022 00:16:26 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:ecfe29996dc654c28c0e2c4726e34d251c79330ce39875ae8fbb5462d2695d5a`  
		Last Modified: Tue, 19 Jul 2022 22:51:54 GMT  
		Size: 2.6 MB (2625483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83880417b8e1d93315351d4b1a05d72cec112bed25505e935120cd05965aea0e`  
		Last Modified: Wed, 20 Jul 2022 00:17:11 GMT  
		Size: 15.9 MB (15857618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b61f765100eafdfeabf46aaa6f0c3958a8eb4f61ab185af21b09a8287060b01`  
		Last Modified: Wed, 20 Jul 2022 00:17:01 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3153b2297daa54746fb1890441136b7352362f4dc6dd8193e6b16432be2099`  
		Last Modified: Wed, 20 Jul 2022 00:17:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0938d4a485e16ef7c787e2c5feb6fe3c0c812e4f2d5db7665b3c98f2f7c59859`  
		Last Modified: Wed, 20 Jul 2022 00:17:00 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; arm64 variant v8

```console
$ docker pull fluentd@sha256:9c0a4a84381fbbeb0395dde2fe0bee86b10175d37a709e26fd605d8f9067ec7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18972013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e0fbbb0f44e27ef9cc9444a08b96deccfa95b0a1ca69617abe6de2a22cdad5`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:48:23 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 07:48:24 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 07:49:14 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 07:49:15 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 07:49:17 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 07:49:18 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 07:49:18 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 07:49:19 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 07:49:20 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 07:49:21 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 07:49:22 GMT
USER fluent
# Tue, 05 Apr 2022 07:49:23 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 07:49:24 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4d143b870226d5f39fdb8712aa4a5601a1f92e4b54f9dada0506bc3bb13b45`  
		Last Modified: Tue, 05 Apr 2022 07:49:54 GMT  
		Size: 16.2 MB (16248964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683f09bd99f0a5d12da8c36d87c3f80cf54f591b19de3b614b1517ed3799a0d`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120b5acf02cc6a091e3e5c982d71e683eebcbfe34dc73d38a806c24cf01ab732`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f8e42a7770e420773b29e879e7fcf9d5a5c9f80bf8b6eaf7f78448964ebcf1`  
		Last Modified: Tue, 05 Apr 2022 07:49:51 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; 386

```console
$ docker pull fluentd@sha256:ea6570baac3902be3f0d11f7bc91717f6b35e23c490f1b27f67196c602e0fa32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18724290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5185eff52fac4e4d36c219fa50f80f199feee2507740f040c0b3c77b171e4267`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:48 GMT
ADD file:216b59d90f7e2b47e8e2db0e1ab68a5709b4ed1fc33a98d40089570dedd3b4cb in / 
# Tue, 19 Jul 2022 22:38:48 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:33:52 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 19 Jul 2022 23:33:53 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 19 Jul 2022 23:34:40 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 19 Jul 2022 23:34:41 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 19 Jul 2022 23:34:43 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 19 Jul 2022 23:34:44 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 19 Jul 2022 23:34:44 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 19 Jul 2022 23:34:45 GMT
ENV LD_PRELOAD=
# Tue, 19 Jul 2022 23:34:46 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 19 Jul 2022 23:34:47 GMT
EXPOSE 24224 5140
# Tue, 19 Jul 2022 23:34:48 GMT
USER fluent
# Tue, 19 Jul 2022 23:34:49 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 19 Jul 2022 23:34:50 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:77bace7fb30573dc3142aca393994871a56867f2e249e3e412697ed19e0735e4`  
		Last Modified: Tue, 19 Jul 2022 22:39:46 GMT  
		Size: 2.8 MB (2820956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b357e0b415e234114b15893ce1038cfdb1347def87a55def3905f39378262c`  
		Last Modified: Tue, 19 Jul 2022 23:35:24 GMT  
		Size: 15.9 MB (15901180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397a2bae804d74cd2a434298c071ebb98aa8cb7928ca9a3d19eb2273f6b7ccdf`  
		Last Modified: Tue, 19 Jul 2022 23:35:21 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62531317ae2607c2e1c7dc2f1adeefb0cc27de45a7101dfe043a872c11a4aee4`  
		Last Modified: Tue, 19 Jul 2022 23:35:21 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9047ac928347340994e4fe508ab8ecdbc4fd3219e1e9b86ee3811a92277c587`  
		Last Modified: Tue, 19 Jul 2022 23:35:22 GMT  
		Size: 460.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; ppc64le

```console
$ docker pull fluentd@sha256:871c56a4777b6a6fe8443160e93e7064b20e33a5046d8814bf3aac788526fe2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19199727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5019884c9779b7a6b641d63bc5c945a68537a12e7a8364326494b3b7fd7d87`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:46:26 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 09:46:28 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 09:47:55 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 09:48:07 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 09:48:09 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 09:48:10 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 09:48:12 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 09:48:18 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 09:48:22 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 09:48:24 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 09:48:26 GMT
USER fluent
# Tue, 05 Apr 2022 09:48:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 09:48:35 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf7bf98a0150cc3e7c08762d573d0288b1d406f1961b06d1619b2a764e41023`  
		Last Modified: Tue, 05 Apr 2022 09:49:12 GMT  
		Size: 16.4 MB (16382727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8337f772435872ab5058c0fa9edbf92ed5ab04b1c2215690bc2b23350d4b7f9`  
		Last Modified: Tue, 05 Apr 2022 09:49:09 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bbda2074a6cf0758960ecca34564ff53f5ef1fe547688c9eb9682b80491ce5`  
		Last Modified: Tue, 05 Apr 2022 09:49:09 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1b61dd9ed879ea4531474568c75fddf58b8fc30ed41a0d56f1b525b9f1bc9`  
		Last Modified: Tue, 05 Apr 2022 09:49:09 GMT  
		Size: 458.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fluentd:latest` - linux; s390x

```console
$ docker pull fluentd@sha256:fcf8dc973f484df1b04d6770c54b7097f210a9494760448791cd473fd8e018b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18833986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47b04692700f8d50356c0605419b39a0a0a3d4dd8933335802d78dc996253ea`
-	Entrypoint: `["tini","--","\/bin\/entrypoint.sh"]`
-	Default Command: `["fluentd"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL maintainer=Fluentd developers <fluentd@googlegroups.com>
# Tue, 05 Apr 2022 03:56:51 GMT
LABEL Description=Fluentd docker image Vendor=Fluent Organization Version=1.14.0
# Tue, 05 Apr 2022 03:57:28 GMT
RUN apk update  && apk add --no-cache         ca-certificates         ruby ruby-irb ruby-etc ruby-webrick         tini  && apk add --no-cache --virtual .build-deps         build-base linux-headers         ruby-dev gnupg  && echo 'gem: --no-document' >> /etc/gemrc  && gem install oj -v 3.10.18  && gem install json -v 2.4.1  && gem install async-http -v 0.54.0  && gem install ext_monitor -v 0.1.2  && gem install fluentd -v 1.14.0  && gem install bigdecimal -v 1.4.4  && gem install resolv -v 0.2.1  && apk del .build-deps  && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem /usr/lib/ruby/gems/2.*/gems/fluentd-*/test
# Tue, 05 Apr 2022 03:57:30 GMT
RUN addgroup -S fluent && adduser -S -g fluent fluent     && mkdir -p /fluentd/log     && mkdir -p /fluentd/etc /fluentd/plugins     && chown -R fluent /fluentd && chgrp -R fluent /fluentd
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:06d9a84b9b428b4e0ef5a9e3699798758dc9716908d82091239fb9f85dd30d70 in /fluentd/etc/ 
# Tue, 05 Apr 2022 03:57:30 GMT
COPY file:977670d9d298d60208db6e5110a5919bfde19ee7da9c19df693163ecd07caea6 in /bin/ 
# Tue, 05 Apr 2022 03:57:30 GMT
ENV FLUENTD_CONF=fluent.conf
# Tue, 05 Apr 2022 03:57:30 GMT
ENV LD_PRELOAD=
# Tue, 05 Apr 2022 03:57:30 GMT
ENV RUBYLIB=/usr/lib/ruby/gems/2.7.0/gems/resolv-0.2.1/lib
# Tue, 05 Apr 2022 03:57:30 GMT
EXPOSE 24224 5140
# Tue, 05 Apr 2022 03:57:31 GMT
USER fluent
# Tue, 05 Apr 2022 03:57:31 GMT
ENTRYPOINT ["tini" "--" "/bin/entrypoint.sh"]
# Tue, 05 Apr 2022 03:57:31 GMT
CMD ["fluentd"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80885e5fcbe2d38543d5e0902ede12aac0343ddb30a4b60bc4d78867956435ce`  
		Last Modified: Tue, 05 Apr 2022 03:58:02 GMT  
		Size: 16.2 MB (16226727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac37dee1aa1774c4de428bdaced201f30a775a16bb7da2c3d9a6ae31bebaed78`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da865ce216091b128ba285b8c6097d5b808474cbe95220b3d9d5e88e6a25fbd`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ad6695a5e27dd3ddaec0e5987c6384aa0eeb5374548d4e86df5137d86bd62c`  
		Last Modified: Tue, 05 Apr 2022 03:58:00 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
