## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:1c47d1b0fa1e418714b016f99aa5f3ad66676111c8191cb1a12b9fe6b6b2faab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
