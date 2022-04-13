## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:7d7cae74feaab83bc05e3f3443218f45bf0eead274ab8c1946ae9a53c2d0f04d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:d8be778bdbef898f5d1bd5293b42cf1dd554d9a8fee542ace03ce7333f469dfd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723819171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a79e6460f3b94b3f4cab31ce7395b20fb9d019f054d5a5dc3c6d8bdd9d0399`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 17:25:36 GMT
ENV NATS_STREAMING_SERVER=0.24.3
# Wed, 13 Apr 2022 17:25:37 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.3/nats-streaming-server-v0.24.3-windows-amd64.zip
# Wed, 13 Apr 2022 17:25:38 GMT
ENV NATS_STREAMING_SERVER_SHASUM=7473bfa7efd734ca6984907bc9586260031cca926883b468b4752557ecefaff0
# Wed, 13 Apr 2022 17:26:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Apr 2022 17:28:05 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Apr 2022 17:28:06 GMT
EXPOSE 4222 8222
# Wed, 13 Apr 2022 17:28:07 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Apr 2022 17:28:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf145cf85a60aab39cbd435958ed35769e55fa7b0e37a2782b88fc2f0d2bbea`  
		Last Modified: Wed, 13 Apr 2022 17:28:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995d3bec8ec657b3364548e2855de1ffa0eb00b35a676b57d3ac17201926b4bb`  
		Last Modified: Wed, 13 Apr 2022 17:28:56 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59150e3be512c902815677dd7fef86c1ec6219f48a8a0414f1d4c6836d8ee466`  
		Last Modified: Wed, 13 Apr 2022 17:28:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509d760670afd3f80efca1c924b1deb75789630800e02e2178e6fbffd358eed6`  
		Last Modified: Wed, 13 Apr 2022 17:28:53 GMT  
		Size: 359.5 KB (359463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709896503a15033ce6faf7dc0ca5c5ae3cf6393398d1d99f280e88d7b724f093`  
		Last Modified: Wed, 13 Apr 2022 17:28:55 GMT  
		Size: 7.5 MB (7528082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159616a832b4f189bbd4a3bc13d3916e4f019d039d4cd3deb3e88b0f6994f626`  
		Last Modified: Wed, 13 Apr 2022 17:28:53 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98590e7ace3cde620ca97857cbaec37df892fd893caa962a70b726c4a2e41d26`  
		Last Modified: Wed, 13 Apr 2022 17:28:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91a3599b60c18624c2ab76790e3c889c25d1c6c76d1b7efcfa813789ca7345`  
		Last Modified: Wed, 13 Apr 2022 17:28:53 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
