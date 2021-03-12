## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dfa33ff752c331d4b76bfe3817fd42ef3ef0bc24d9167cdfdd39f137054ea298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:5203e8707456e06dfc8d03ba99cdfe84d4b3dc00be512770827ef5e692ec18e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487805125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f93dd36e27e04e9ac5d0bc9da46fbeebc4541b2a242f90a7bc7003d2bc636fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 21:27:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Mar 2021 21:27:32 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Mar 2021 21:28:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Mar 2021 21:28:06 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Mar 2021 21:28:07 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Mar 2021 21:28:08 GMT
VOLUME [c:/config]
# Wed, 10 Mar 2021 21:28:09 GMT
VOLUME [c:/data]
# Wed, 10 Mar 2021 21:28:11 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 10 Mar 2021 21:28:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Mar 2021 21:28:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Mar 2021 21:28:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Mar 2021 21:28:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Mar 2021 21:28:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Mar 2021 21:28:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Mar 2021 21:28:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Mar 2021 21:28:19 GMT
EXPOSE 80
# Wed, 10 Mar 2021 21:28:20 GMT
EXPOSE 443
# Wed, 10 Mar 2021 21:28:21 GMT
EXPOSE 2019
# Wed, 10 Mar 2021 21:28:41 GMT
RUN caddy version
# Wed, 10 Mar 2021 21:28:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a02199a38f7dde446e1c919797037b896dc0d954cc313cd49d1fd7ef7b309a`  
		Last Modified: Wed, 10 Mar 2021 21:43:28 GMT  
		Size: 9.5 MB (9466151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928fadc2fce7089b23d0e2d915e1cf2211aec3ffdc88b5eb66c67f18f7fb2c6e`  
		Last Modified: Wed, 10 Mar 2021 21:43:26 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7bb988dcbf796f3839a524b32be07309d29f50ec4273ded91973b631e0ad00`  
		Last Modified: Wed, 10 Mar 2021 21:43:45 GMT  
		Size: 16.5 MB (16453921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621047471067d3c16923f7c3b79f8615ddbcc2f9a879832c456f67fe3cd1544`  
		Last Modified: Wed, 10 Mar 2021 21:43:25 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f148a6aba7a2d10970470390d5229567735df01114acfbdad1c661bdc8dc22`  
		Last Modified: Wed, 10 Mar 2021 21:43:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc608f5d46fef14425bc80c9c7062532f20bec43d7073a8e17e8278f9c60cc7a`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda8fe89940ce8986995aee365da1f58c22d0d3b8a050600e429ef1cdd8c5fc`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403d8611297f60270051c62d4bb7d7dff6aeeb33dc0c5cecd06ae94080fd1802`  
		Last Modified: Wed, 10 Mar 2021 21:43:23 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df9d9f268b91b0f5bd3e27ba3e1cd03694b62c48ad901fa7fc47ebd2956db`  
		Last Modified: Wed, 10 Mar 2021 21:43:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eabd07d0fd9430b675ce97b3bd926812eb4e9f4c4cf0872d68b91be65dd9d9`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec389e155c01fcd9625c110db8b62baac443eb2bee04a5f631e7cecc534c0818`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8fad2b33541d43c28d6113e51b250763c7ec33d8503df271481f615a1f99bc`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf0c1f7ba714c558dd8ed7e0336f84c91c25a35766d2efa592b1f39b1e448d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93772cd9ce84491fa183154e0972b941a4379f628a54f9213bf36c4311dbbb`  
		Last Modified: Wed, 10 Mar 2021 21:43:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fa064b906d0bd7b584ea5f181fbca29305d9ad824eaed29bf341c1abbcea3`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b753cdd37ef6dce0fbecce933fdf1957f9d72cf512be44c11d32181611a433`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0205b004a4016df290e2fd8b362003adad13b56a6fbc17c35209de56b2bac034`  
		Last Modified: Wed, 10 Mar 2021 21:43:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f63eec622fd92f0ce90d6e06bd12c2687cbdf86aae3cdbbb8d3fdc92ef028`  
		Last Modified: Wed, 10 Mar 2021 21:43:19 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446a62c8913c6a60f39e8053d6ad0d6dfaf69ec7d8cf3fcc2665386e362238d6`  
		Last Modified: Wed, 10 Mar 2021 21:43:18 GMT  
		Size: 325.1 KB (325114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc4417c46cd53b142f42f58ded86ccf383c9f9b6e5f97d8a8183abbd1bd7aa`  
		Last Modified: Wed, 10 Mar 2021 21:43:17 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
