## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7dade2ad7012a220264a666cb88816602136a902b5111fa2082b30911aa5208d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
