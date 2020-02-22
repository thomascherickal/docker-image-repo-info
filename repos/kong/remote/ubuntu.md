## `kong:ubuntu`

```console
$ docker pull kong@sha256:6884b1b187f62ee9c877de29ff6bfc37712b2b55951074369770664c0b918d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:29330b524e13be5cca2ab14111305d4ca9dba90e39daaaed6c4068ee5289b1b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84759132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10032c0185ac4c470fbf652a91c2789a6e2316c1a5bb2fd98c52edc7dab058f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:58:48 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:58:48 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:59:08 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:59:09 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:59:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:59:09 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:59:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:59:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bde84fdc6c62e356ce7c83a9a99b038153653abfdc0749ea975850dbc4e4db`  
		Last Modified: Sat, 22 Feb 2020 00:01:41 GMT  
		Size: 40.6 MB (40565549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53e6f859c77fafc346d3f1522a724dbbcbc031d7efbfbd3db3aca2ebd145c80`  
		Last Modified: Sat, 22 Feb 2020 00:01:32 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b004232c06b70ec67fa73a376be87950cf8b2795495641cdd04ad58b2bd14c99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79179962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e3f50b87ada1237fa10e0f0ca9e13c372a4f227842d7d603d24c0aef6fbbaa6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 21 Feb 2020 21:55:42 GMT
ADD file:61b91c95a686740a57740470b7a1fe64d2479c56c36c69ca1222d870e78d44cc in / 
# Fri, 21 Feb 2020 21:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:55:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:55:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:50:03 GMT
LABEL maintainer=Kong Core Team <team-core@konghq.com>
# Fri, 21 Feb 2020 23:50:03 GMT
ENV KONG_VERSION=2.0.1
# Fri, 21 Feb 2020 23:50:42 GMT
RUN useradd kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chmod -R g=u /usr/local/kong     && apt-get update     && apt-get install -y --no-install-recommends ca-certificates curl perl unzip     && rm -rf /var/lib/apt/lists/*     && curl -fsSLo kong.deb https://bintray.com/kong/kong-deb/download_file?file_path=kong-${KONG_VERSION}.xenial.$(dpkg --print-architecture).deb     && apt-get purge -y --auto-remove ca-certificates curl     && dpkg -i kong.deb     && rm -rf kong.deb
# Fri, 21 Feb 2020 23:50:45 GMT
COPY file:da5de9257b8a314f62615a4ecc2736080e316da14d00bd323efd2be62c23222d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 23:50:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 23:50:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 21 Feb 2020 23:50:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 21 Feb 2020 23:50:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a7bab9946de3c22ecccd832a0910adc2ffa82eea53f83c600d5ebce9e5422ad0`  
		Last Modified: Mon, 17 Feb 2020 15:45:27 GMT  
		Size: 39.9 MB (39940373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38630c4d9093f5b60806171ca7fa47a70d7ab28eeed25edfad43fb91d5f9f825`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef678cbe74d844c6a114c1158a8c8868b412b7c5ed3a4c159831975a4915db9`  
		Last Modified: Fri, 21 Feb 2020 21:56:39 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78928743b0e778df64b15ac919705702ee0a080c2586f43c4349b35180de3c36`  
		Last Modified: Fri, 21 Feb 2020 21:56:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c254c68615ac69e67f51f050f2a39cf48e4249c3513d062dc57aa5fbf166a03e`  
		Last Modified: Fri, 21 Feb 2020 23:54:32 GMT  
		Size: 39.2 MB (39237789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154dc7a5f6ff7ce51e8c36d94402558a03d22c8b7d76e27d6adb19f0d4c75ac`  
		Last Modified: Fri, 21 Feb 2020 23:54:18 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
