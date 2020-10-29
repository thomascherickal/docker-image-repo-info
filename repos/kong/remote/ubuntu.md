## `kong:ubuntu`

```console
$ docker pull kong@sha256:94cb54ff52ea1a0a9f4bcf5aaee6c67c4a8f7a3e256f43b51301c299c9f858b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:056ffd524e8849b89f710a671b10841e337a5734a372fa428e89826f2eaa54f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135598240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c048ac8311203db66211353c0d2ff83bd3696b6f3f3637b35a3b77859a1d1549`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 29 Oct 2020 18:21:27 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:27 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:16 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 29 Oct 2020 18:22:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:22:17 GMT
USER kong
# Thu, 29 Oct 2020 18:22:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:22:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:22:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:22:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89deb52ede76e668a6e5adf0b8f3373863c9d0dcaee49ba0928857ff72a0ae`  
		Last Modified: Thu, 29 Oct 2020 18:24:05 GMT  
		Size: 64.7 MB (64688329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe067f92ac3cc8db17ae04fd765d1765205b10aee77351f9773f33d935ed40`  
		Last Modified: Thu, 29 Oct 2020 18:23:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8d0a6bcb0291724ab6f0585fa01d1cdeca6787a95f7e94e0b3a0b7149099e473
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124401827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:badfa7c0e37cdd9a94bb927f49960d74527e25e4174d4dd3b3ab2dc45ffb24a3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 25 Sep 2020 22:48:52 GMT
ADD file:5ad8fe01e35cc6efe923d7698aaa261cdb15f4f4ae01009d04d2a1ddadc1d5b2 in / 
# Fri, 25 Sep 2020 22:48:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:48:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:49:00 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:59:30 GMT
ARG ASSET=ce
# Fri, 25 Sep 2020 23:59:31 GMT
ENV ASSET=ce
# Fri, 25 Sep 2020 23:59:32 GMT
ARG EE_PORTS
# Fri, 25 Sep 2020 23:59:33 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 25 Sep 2020 23:59:34 GMT
ARG KONG_VERSION=2.1.4
# Fri, 25 Sep 2020 23:59:35 GMT
ENV KONG_VERSION=2.1.4
# Sat, 26 Sep 2020 00:00:26 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Sat, 26 Sep 2020 00:00:29 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Sat, 26 Sep 2020 00:00:30 GMT
USER kong
# Sat, 26 Sep 2020 00:00:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:00:32 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 26 Sep 2020 00:00:33 GMT
STOPSIGNAL SIGQUIT
# Sat, 26 Sep 2020 00:00:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:511338b9646fd6cab2c278e174281c8d444bef1a2846348b1e0687ece0450d3c`  
		Last Modified: Wed, 16 Sep 2020 16:25:23 GMT  
		Size: 40.1 MB (40099025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b39b0ff65d844135c15ee00abc2dec8e0a964a0f626097ba95ee4c2fa0a19ed`  
		Last Modified: Fri, 25 Sep 2020 22:50:25 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a1f7ba18a1a2b6ece87fc83510da11658ea364ee85e16467c0ca7cfadb52d7`  
		Last Modified: Fri, 25 Sep 2020 22:50:26 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa76f7dac8b4a5afba79f1582f3546a987a066f79adb97b5dfa25b0f72989a`  
		Last Modified: Fri, 25 Sep 2020 22:50:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4bb3c080d765079ec8f882652786b891b2eb691d1d76d94cb98ba0a7a521c`  
		Last Modified: Sat, 26 Sep 2020 00:02:35 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fa7561cbea7354b8a4e1fcc7c4d04e7bb22276089e24f35fa41c2153c576f3`  
		Last Modified: Sat, 26 Sep 2020 00:02:52 GMT  
		Size: 59.2 MB (59218668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79eb6330d83ab3f09850bc73fcc101d3874e8632f6f766537b28b1ce5642e56`  
		Last Modified: Sat, 26 Sep 2020 00:02:33 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
