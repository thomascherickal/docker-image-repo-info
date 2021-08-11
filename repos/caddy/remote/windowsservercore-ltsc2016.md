## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:427a83aa263265d9a7898be8febb2edd4ef982d3de16149fe407d8e850d36f62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:ec7ef8cd2121d5f23f42c0251291677ecfd0c29840e51aa4c9fef254d1c1560d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283643015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ad8b04c922f6dda8fd4d42f65100f074b0c4db63ee1b3cbe606ac30abd80d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 21:05:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 11 Aug 2021 21:05:39 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 11 Aug 2021 21:07:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 11 Aug 2021 21:07:17 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 11 Aug 2021 21:07:19 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 11 Aug 2021 21:07:22 GMT
VOLUME [c:/config]
# Wed, 11 Aug 2021 21:07:24 GMT
VOLUME [c:/data]
# Wed, 11 Aug 2021 21:07:27 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 11 Aug 2021 21:07:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 11 Aug 2021 21:07:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 11 Aug 2021 21:07:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 11 Aug 2021 21:07:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 11 Aug 2021 21:07:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 11 Aug 2021 21:07:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 11 Aug 2021 21:07:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 11 Aug 2021 21:07:50 GMT
EXPOSE 80
# Wed, 11 Aug 2021 21:07:52 GMT
EXPOSE 443
# Wed, 11 Aug 2021 21:07:55 GMT
EXPOSE 2019
# Wed, 11 Aug 2021 21:09:06 GMT
RUN caddy version
# Wed, 11 Aug 2021 21:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b905a67f0a6b890effd48b106ac411e8d5f9bed02519c07893ce8267bcca1a`  
		Last Modified: Wed, 11 Aug 2021 21:14:12 GMT  
		Size: 352.7 KB (352717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6f6a9467f932967cf987e57c147f02a5db262a7f278857dda56a798e2e2464`  
		Last Modified: Wed, 11 Aug 2021 21:14:11 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53117b1284a36cc442512d2c5c77e1b621d46719c74e714db1e17bf85d75f6ad`  
		Last Modified: Wed, 11 Aug 2021 21:14:26 GMT  
		Size: 12.0 MB (12028003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795d9a6fe1f04d258cc72503b7bac2fd15afc31937edef8fc64b8be6b7544c9`  
		Last Modified: Wed, 11 Aug 2021 21:14:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae36572141921b48f387d56bc8b2151d37d29c6160dd1872593ccea24f6f7638`  
		Last Modified: Wed, 11 Aug 2021 21:14:11 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df882531a6711193135e2d4cacc1c72d11a2605be8cb0de9ab4cc31b8783f96`  
		Last Modified: Wed, 11 Aug 2021 21:14:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d758f29ff944296e6feaf842ab1d9e4cb11072666f07d4f17839b24dd89d9f`  
		Last Modified: Wed, 11 Aug 2021 21:14:09 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2269932a33e3e7b04c9267abde55673283169d25c40dd8cb34ee9238c22d7def`  
		Last Modified: Wed, 11 Aug 2021 21:14:09 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee4fe2e1025ff0fa13b2cda56f9c275f79011a908b8affeca16fa043d4b51e1`  
		Last Modified: Wed, 11 Aug 2021 21:14:09 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1677ff9a3185a77087b884fd63239b62e996a1fb9934d5c52a5a0ed0c2b9ec`  
		Last Modified: Wed, 11 Aug 2021 21:14:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e11e1d3787ef4addcf01f1c1d28c5bfb1df9671ed5d781f47c3ea291f8cedc`  
		Last Modified: Wed, 11 Aug 2021 21:14:06 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381e93e3aa9975f6e9fb0fd48d5da5676ceb0d46aa4e34f7468090f0a40f2f1f`  
		Last Modified: Wed, 11 Aug 2021 21:14:06 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686da7ab4d6b6bb476396cb448be785c2bc2def08aca52ba14f437d89553cfdc`  
		Last Modified: Wed, 11 Aug 2021 21:14:06 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512abb2c5a0f2fb6489a76860a9e8ae1d951e8306b0f4d27b3533470880ee19`  
		Last Modified: Wed, 11 Aug 2021 21:14:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672bfac681704b47216df2673d5c020b179dba72b646daa877a73b51655e199d`  
		Last Modified: Wed, 11 Aug 2021 21:14:06 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42fe3600429a2ba86980c402f95f9177ce2fbb0f3fcf342ec93caa9f3922814`  
		Last Modified: Wed, 11 Aug 2021 21:14:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1afa5e67d425706efec4f865657eae9fe68c4e283aa7ee4f23560365618da`  
		Last Modified: Wed, 11 Aug 2021 21:14:03 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac377f2b8a4b123fed52b221b5b72f2c2c065a44053f372855750c4e3471d974`  
		Last Modified: Wed, 11 Aug 2021 21:14:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f6f9319eb85bf71607751e1d005c408ed7123146f7e2294585fc0767ab8f8e`  
		Last Modified: Wed, 11 Aug 2021 21:14:04 GMT  
		Size: 270.8 KB (270764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cceefa485008e41ca85674d97229e9692866d78af51ef2a9b601f798e30f905`  
		Last Modified: Wed, 11 Aug 2021 21:14:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
