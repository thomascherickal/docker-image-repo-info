## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:540bc831c83dfe88a9d469750f2d8228fd14627e1cb6433a4e6b9470190c505e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull caddy@sha256:ce36943bd1dd39de8f8d6b47eaab078dc2b47a5a3c4ce7e065d18b7cd672e911
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751106345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5fbf7d2d002a25cee5fcc7ac5259a43b287f575e9627946e2582f27295387a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 23:17:30 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Mon, 20 Apr 2020 23:35:28 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 20 Apr 2020 23:35:30 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 20 Apr 2020 23:49:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('482652dbe7600d4d324c837a00eddf58254aeff57315afa1547fc61daefcb2f8952df8f3f8ec9c44e9ec919d1bfc908aeabe68b7d780d988d68e78581202d7ca')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 20 Apr 2020 23:49:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 20 Apr 2020 23:49:36 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 20 Apr 2020 23:49:37 GMT
VOLUME [c:/config]
# Mon, 20 Apr 2020 23:49:39 GMT
VOLUME [c:/data]
# Mon, 20 Apr 2020 23:49:39 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 20 Apr 2020 23:49:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 20 Apr 2020 23:49:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 20 Apr 2020 23:49:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 20 Apr 2020 23:49:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 20 Apr 2020 23:49:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 20 Apr 2020 23:49:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 20 Apr 2020 23:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 20 Apr 2020 23:49:47 GMT
EXPOSE 80
# Mon, 20 Apr 2020 23:49:48 GMT
EXPOSE 443
# Mon, 20 Apr 2020 23:49:49 GMT
EXPOSE 2019
# Mon, 20 Apr 2020 23:50:29 GMT
RUN caddy version
# Mon, 20 Apr 2020 23:50:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72ac64d06edc38376c754491fd7ced4aa035af4e675cdc3ac928ea71101af9d`  
		Last Modified: Tue, 21 Apr 2020 00:27:58 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d9ac51d67cd523925abe19d1fefd0f5e5de96dd7f4210eebd601cd07940879`  
		Last Modified: Tue, 21 Apr 2020 00:27:59 GMT  
		Size: 5.4 MB (5407793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efd1ee2ff7bdfd99171e6f519ce15fec5cae88d015c7fe68f90bc0a06c6d931`  
		Last Modified: Tue, 21 Apr 2020 00:27:55 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6a8fefdc6e0c56bb106524f505c0946830f2f05160508c322fe12c577ff6c3`  
		Last Modified: Tue, 21 Apr 2020 00:28:00 GMT  
		Size: 17.3 MB (17345135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a9eb27291be9eca6eba7e86637f2e89299d52c9b7e6e8732d3142413a0cdd`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbda073322d4050091a4128fbee7a86f3a44a20a5e48a9a757b75f947e55389f`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25bd862ac7d8a4e4dd071336125b456299f48e50a0521b24c85d960076e0199`  
		Last Modified: Tue, 21 Apr 2020 00:27:54 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f91e729270af491f0aa53bb55300e2d82a22aad5c79d552884f60da6cd4e4`  
		Last Modified: Tue, 21 Apr 2020 00:27:53 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad733b24685a79f25a39ff32f4aa315ebfae9df99740c7432be70bad755dae2`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57efa182f8d96025abbeabbf9263c42537fda0ad5a4f59a312d5ece4cfcd508`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b347e572e899a9b99fd7aaf5f29345aaf65ce32e7a121771c8021c662a1f4f`  
		Last Modified: Tue, 21 Apr 2020 00:27:52 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9eb61d24eaffc90b7870772f420233e1520893a9ad25c44bb055f787ee2705`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8150597f5e499c8bd034ca80229afd4aa88471b8efe5443772e1e92fd066b751`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61038c548fa7ceffb45bf18cb81982dc221149295379caa793056c88590d860f`  
		Last Modified: Tue, 21 Apr 2020 00:27:49 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5e285cc3c3c7d19ff1a8aba39a5fa042cb718bae816d46b3a59358f47378ee`  
		Last Modified: Tue, 21 Apr 2020 00:27:50 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a118b6f4d69c1f8b687dd9af977ee2f24bc5941ca9b8cc69ad80e487f9fa283b`  
		Last Modified: Tue, 21 Apr 2020 00:27:49 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f711254bc6fec0693a5e59eec876b3e388671ebee36fb7ff665c7f840da97`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97944dcb26ce67036f0a5d96e3a9d8b4911945df4e4506284becb7d72aacca1`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3049d194f6bb19cb62503770c5b949a2d2806848f6dd8c2c0fa755818a8741f`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c13083a16372e822e86a1958ba180d6ad32f22d0d13ca941a74351a7d531a18`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 265.2 KB (265183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8883ec4854456b8d05c3ba46b3e7c7eec6e91ad0d596e374178fc795cda12a13`  
		Last Modified: Tue, 21 Apr 2020 00:27:47 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
