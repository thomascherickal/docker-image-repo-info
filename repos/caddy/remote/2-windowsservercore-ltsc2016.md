## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:01472e271cb930e4158b91691b2b0c8b03ae719bd9cd00cbf5244e41bde54d9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull caddy@sha256:3a07927290350c09edfce9ecbd40063370cdb8a8b7482d82baa63720aab7c349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea871a5e1ed9acbff2235680efdea101cfea3eecf457d551bd441aa814bd2ef5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:44:53 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Feb 2021 19:50:13 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:51:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Feb 2021 19:51:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Feb 2021 19:51:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Feb 2021 19:51:36 GMT
VOLUME [c:/config]
# Wed, 10 Feb 2021 19:51:37 GMT
VOLUME [c:/data]
# Wed, 10 Feb 2021 19:51:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Feb 2021 19:51:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Feb 2021 19:51:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Feb 2021 19:51:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Feb 2021 19:51:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Feb 2021 19:51:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Feb 2021 19:51:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 80
# Wed, 10 Feb 2021 19:51:44 GMT
EXPOSE 443
# Wed, 10 Feb 2021 19:51:45 GMT
EXPOSE 2019
# Wed, 10 Feb 2021 19:52:28 GMT
RUN caddy version
# Wed, 10 Feb 2021 19:52:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fca65216c0ae5ce81bad139cd0e1247b51fdbff6823b553cc77fedfe133941`  
		Last Modified: Wed, 10 Feb 2021 19:55:59 GMT  
		Size: 10.2 MB (10179684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c889da89d18131524dfee13894f0da3780e1c5ef48412eeb4057a2c3808c8d1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa3d7bbbcd517d60f49c962c84a97f8001d862abb90a0b2e0d1196735a59fe6`  
		Last Modified: Wed, 10 Feb 2021 19:57:14 GMT  
		Size: 21.9 MB (21860879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d196fd5cade052aba40376ac5d168df99f2f83ef8e80eed25f7bb415243816`  
		Last Modified: Wed, 10 Feb 2021 19:57:08 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dad702552e6c0a62f4c193101380e9066dcf379fea7302a46a11bda1a7ce0df`  
		Last Modified: Wed, 10 Feb 2021 19:57:07 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2771a088d328335018bc45075859b1c63111e7b0e3e28a6fc64cadb6a9eb4709`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4bab9d807e1e76f459eae60ab0623a316dc9f4cdeb9522be6756aba21c7903`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dde666e4472ba12a12b2fe6a95adb0185882305ad3df128138c0acddd770cd6`  
		Last Modified: Wed, 10 Feb 2021 19:57:06 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904db5bdbbd54b376d6a4dc154acc1b26b9f7ab2b7224b6d2cdd3f90c44faf33`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833b5a97d8d3f35cbe2d2ab4313357f5ca3b76e4a0521025dc4374275bf187f0`  
		Last Modified: Wed, 10 Feb 2021 19:57:05 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a358b9325eb702058fd7d5f6c0ede9782a0ff30516b0f4446bf88ad5c2c77352`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2508061b8b9c715f5741e31823f0ecdef61cfc5136e41a279d6c54f0f0719b`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4f97934d42fd6ddca14f7ee6ca360268c7d81e910e9e7c7bb91ba3ff25c02f`  
		Last Modified: Wed, 10 Feb 2021 19:57:03 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207a0472416ab29841d96b43dcba9f57a27d895f77c25737f1da72717497461`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112054257d71323af7aabc35afe84b913d05dab3be85ebe9381e146cb395e73a`  
		Last Modified: Wed, 10 Feb 2021 19:57:02 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e2075b46da5e143243cc6a93b351902308595b30a17cea08083a9fb7d5bc1f`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86f8a6e2982d2b1b36aa09c5875b421aa8e764b31b93c10d6054f72822cdf6`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac52c52010f5f3180b22f77a01ec762a8eab30264e9941f284a0df78543e854`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5713c505b7a70b79c02e8d85f0054462df5d08fe584616ea60da6ddffd44301`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 266.3 KB (266319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9093d09b769357e6cce989fed39a63250c444cd10ae20040897a770ed2c1be`  
		Last Modified: Wed, 10 Feb 2021 19:57:00 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
