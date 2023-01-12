## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:67ec69b56b6b8116446abfcdc0d627d9c1b244af1c371bb0f458ec5cb8291201
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats-streaming@sha256:0a8c8b643ff6a71471326145bd9f7a1af422d2adbde413dff8650bc81dd00637
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1716415719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0be0a35b5114e448caf1f8f9f0e8c40919e8ad373194ff5251d25fcb56e9f4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Thu, 12 Jan 2023 05:03:28 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 12 Jan 2023 05:03:29 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Thu, 12 Jan 2023 05:03:30 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Thu, 12 Jan 2023 05:03:54 GMT
RUN Set-PSDebug -Trace 2
# Thu, 12 Jan 2023 05:05:12 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 12 Jan 2023 05:05:13 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 05:05:14 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 12 Jan 2023 05:05:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf2d2471dfe8f217d8b7421e6b7ee60bdfec03b3308a673bd53e9127a22b15c`  
		Last Modified: Thu, 12 Jan 2023 05:06:01 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5859c02649f53330c0dede90845303aac7f9917de23f5c7685aabfd4a088adc5`  
		Last Modified: Thu, 12 Jan 2023 05:06:01 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956628c482aa0f8d5c3e1f0fee10ad27b89fd455b95dd979425dd342586c2269`  
		Last Modified: Thu, 12 Jan 2023 05:06:01 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c0f699fa5a16ff6512897ac0a8b28938cba0c09184ccb240b330c9676d8d2b`  
		Last Modified: Thu, 12 Jan 2023 05:06:00 GMT  
		Size: 360.8 KB (360817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea7a6ef728665002b922f36d8652ce103676c7913d6df30e8dd6fbc6aaa9252`  
		Last Modified: Thu, 12 Jan 2023 05:06:01 GMT  
		Size: 8.1 MB (8099685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f147bf9f8ef2640383c0a3f63f73c7bf70e70c797cf91e129aa386734ee6efe4`  
		Last Modified: Thu, 12 Jan 2023 05:05:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ddabdf0771d2d08d1976602aba697599dcd78abbae868c0f4ea24fa6fe3bf1`  
		Last Modified: Thu, 12 Jan 2023 05:05:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc8bd34377a11fd7ff482bb8e2cd23271eee373157371e959fab3c6a0883903`  
		Last Modified: Thu, 12 Jan 2023 05:05:59 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
