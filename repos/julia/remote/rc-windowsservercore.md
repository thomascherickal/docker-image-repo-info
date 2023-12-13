## `julia:rc-windowsservercore`

```console
$ docker pull julia@sha256:af9e508edee6284565ed856060113e5407018e6858367f06acd03b6ebaab3227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `julia:rc-windowsservercore` - windows version 10.0.20348.2159; amd64

```console
$ docker pull julia@sha256:049e7502ea25152ce685d518674ae83ed3f6ac7de1656aab573e5b603428a790
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2071866938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ea8220dbeb90bfac014221acc11a8fa47ee1249507a7572691261c49f4fe73`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Wed, 13 Dec 2023 00:57:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:57:26 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Wed, 13 Dec 2023 00:57:26 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.10/julia-1.10.0-rc2-win64.exe
# Wed, 13 Dec 2023 00:57:27 GMT
ENV JULIA_SHA256=e65b6b0c573c4d0539f31e86870358e12970b2cb0cb9a4c43945c19c36464187
# Wed, 13 Dec 2023 00:58:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:58:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc9c0ad6232b7aa6715a195144a825760f430ee1aed8bfc3608bb43a3ba09a6`  
		Last Modified: Wed, 13 Dec 2023 00:58:27 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84143e5421fb1e8bae501bb168cd0b0e58d95f90de30a9d800069929924e9d2`  
		Last Modified: Wed, 13 Dec 2023 00:58:26 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c417bf40a1828b40d68e7fa3c17565c492cf773210234953238d9c0a9506f5e8`  
		Last Modified: Wed, 13 Dec 2023 00:58:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5158b13efb72e1eff57ac402b25e2f75d99bdd2904aebba1f6c8cebd0febcca`  
		Last Modified: Wed, 13 Dec 2023 00:58:26 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0b2ccfa6831bfa9eae8c24944aea85567d3e61c27b5c1b405b4d1def1513b`  
		Last Modified: Wed, 13 Dec 2023 00:58:50 GMT  
		Size: 182.6 MB (182586877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebd0cf82997ba74f20f2061dc3406ac90867ce42d5eedac601409634efa5c97`  
		Last Modified: Wed, 13 Dec 2023 00:58:26 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-windowsservercore` - windows version 10.0.17763.5206; amd64

```console
$ docker pull julia@sha256:49bba8520daff62f5fc89463bee84420bfcbf0e79bc8478cbe4222eb8f99ab22
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2242322676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc7f0c3a5618ae1471545bfb4c9d5bf6ed2a7046f27e38e07126c76c5bd0cf3`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Wed, 13 Dec 2023 00:59:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:59:25 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Wed, 13 Dec 2023 00:59:26 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.10/julia-1.10.0-rc2-win64.exe
# Wed, 13 Dec 2023 00:59:27 GMT
ENV JULIA_SHA256=e65b6b0c573c4d0539f31e86870358e12970b2cb0cb9a4c43945c19c36464187
# Wed, 13 Dec 2023 01:01:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 01:01:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a189d937d5f963eba5e4a5fd117b04b35e52220721dbfcb0616b30b653d6c3a3`  
		Last Modified: Wed, 13 Dec 2023 01:01:34 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02931385f99439c0007f0202942fd6acbef4ad342b13909b06f2c3a35aec29c3`  
		Last Modified: Wed, 13 Dec 2023 01:01:33 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf2413b3d80e0395ab981f5271b11ed5a88be70719bc0a87783fa179f2a7db`  
		Last Modified: Wed, 13 Dec 2023 01:01:32 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b31d69b7b78b805337f7f086f1c21d02cd878a6ebfb44bea2a8b33fcf4bfb6b`  
		Last Modified: Wed, 13 Dec 2023 01:01:32 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520dd040a86873ca76dd6fa6ad90314cb53e790cfbaadf10fea34ed6bab8b2a7`  
		Last Modified: Wed, 13 Dec 2023 01:01:57 GMT  
		Size: 182.6 MB (182607187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3d28de2f4c6f5309421f55d4488c87eda76481e0dc76bdfcf44e734ad23582`  
		Last Modified: Wed, 13 Dec 2023 01:01:33 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
