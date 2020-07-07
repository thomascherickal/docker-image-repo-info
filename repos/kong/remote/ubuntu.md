## `kong:ubuntu`

```console
$ docker pull kong@sha256:b50d572071c3e487d7c827bb6c1f74bd0a575d55afb7b9b76b6dd5d0a5027a6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6e7fc280432b51237a21c97dd07c51109d33ee3bbfbd1853d6311118ee05503d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94258837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b976ee092dd39308988372a5f626dc0e1cbac717718540d7ec5de2e140ce543`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 17 Jun 2020 01:21:26 GMT
ADD file:52af30f80ba214985a59cb0ef7073c64f8514d58396c0de48f8d7056dec2a58a in / 
# Wed, 17 Jun 2020 01:21:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:21:29 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:41:23 GMT
ARG ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
ENV ASSET=ce
# Wed, 17 Jun 2020 03:41:23 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 17 Jun 2020 03:41:23 GMT
ARG KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:23 GMT
ENV KONG_VERSION=2.0.4
# Wed, 17 Jun 2020 03:41:56 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Wed, 17 Jun 2020 03:41:57 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Wed, 17 Jun 2020 03:41:57 GMT
USER kong
# Wed, 17 Jun 2020 03:41:58 GMT
RUN kong version
# Wed, 17 Jun 2020 03:41:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 17 Jun 2020 03:41:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 17 Jun 2020 03:41:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 17 Jun 2020 03:41:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b5e173e44934e01d8d2674bc8b1da00f761c4fe796e0fb2bee1bd1129d2e4ae1`  
		Last Modified: Fri, 15 May 2020 13:20:22 GMT  
		Size: 44.3 MB (44320272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29047100b0407dff554ea80b8005380d62b13a66d7fe2e2adb07b9c091b9f2c0`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15743a713c2a4033877dab08fb3989280f8c856234227158a4011811c7991372`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc9e2987763aa991b7dfd742be04c7b3bb04448982ffe88e58d55c93b76d4`  
		Last Modified: Wed, 17 Jun 2020 01:22:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4343b29744d103aba382b3e0d1bb877f9ecd481767e889ab6c86d1875c6bad99`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77d810dd3c12a2c32a82bc3979848e8ffe74d88da00a775d5973e2e2303d18`  
		Last Modified: Wed, 17 Jun 2020 03:44:24 GMT  
		Size: 49.9 MB (49936157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c17c931a333f8e16904735f731b63e0b725c77ac98f4cb169e71a903211d53`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02e74085ded36213dfb17ff4f178ddef933eaed8d1cdda2638546c6946a638`  
		Last Modified: Wed, 17 Jun 2020 03:44:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f45baefb4365cf59fbfb8784a87835c07c003e6cd4d43061a622f595a87f9896
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87956868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaad0ea2000f7e8419a14d4050bd515e37846a9be657ce80e8743675ef6ed4c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 06 Jul 2020 23:11:53 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Mon, 06 Jul 2020 23:13:11 GMT
ARG KONG_VERSION=2.0.4
# Mon, 06 Jul 2020 23:13:11 GMT
ENV KONG_VERSION=2.0.4
# Mon, 06 Jul 2020 23:13:49 GMT
RUN set -ex;     if [ "$ASSET" = "local" ] ; then exit 0 ;     elif [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb &&         apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong
# Mon, 06 Jul 2020 23:13:52 GMT
COPY file:7cd3b30326ffeaddc1253699208f97fb54711d4ae930aeeeff1e19ebf51cb561 in /docker-entrypoint.sh 
# Mon, 06 Jul 2020 23:13:52 GMT
USER kong
# Mon, 06 Jul 2020 23:13:54 GMT
RUN kong version
# Mon, 06 Jul 2020 23:13:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Jul 2020 23:13:55 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 06 Jul 2020 23:13:56 GMT
STOPSIGNAL SIGQUIT
# Mon, 06 Jul 2020 23:13:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e9d9ca3d496619cb7d9dd321c5e1b12f499e234a4bfff523ed3169665df8b`  
		Last Modified: Mon, 06 Jul 2020 23:15:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7167cc4fdbdcd6b1e42eefef9a0e843677603d721543bdd71fbb5fccfe0c784b`  
		Last Modified: Mon, 06 Jul 2020 23:15:45 GMT  
		Size: 47.9 MB (47919051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145f31f4d6fa8e388dcda72f41d13b4140883938ea81778a74cdc775a44e8c4e`  
		Last Modified: Mon, 06 Jul 2020 23:15:30 GMT  
		Size: 632.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627990a3dfb0b5ae178e48a22a9b7c41e7c01d057779a3d83dfc2f96e91d4b5c`  
		Last Modified: Mon, 06 Jul 2020 23:15:29 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
