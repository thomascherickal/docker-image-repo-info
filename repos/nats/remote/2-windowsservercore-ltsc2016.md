## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:e0113341e4407f3e09685758839e17a425ac36640e0b8ef2c1b72f61ef0f50ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
