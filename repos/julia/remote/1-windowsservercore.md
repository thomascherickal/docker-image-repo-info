## `julia:1-windowsservercore`

```console
$ docker pull julia@sha256:a4d892bc424abdd051de80b5147e3e5c454065ec01dc50ca6c870dbd7b0bbc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2451; amd64
	-	windows version 10.0.14393.4886; amd64

### `julia:1-windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull julia@sha256:de80a16c34129a428c6ab1ba00e3f279e30ad90a9a07703b8458d4f0c4f4e740
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2352687517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2b10d82f019aa8f9cc3048da76cc9a9ad6ed8c50b6da5ceb3be24302cd599be`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 20:49:57 GMT
ENV JULIA_VERSION=1.7.1
# Tue, 11 Jan 2022 20:49:58 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Tue, 11 Jan 2022 20:50:00 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Tue, 11 Jan 2022 20:51:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Tue, 11 Jan 2022 20:51:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd324b80ddf4893f12a81b483f368189b6d0e005b3c9821fafe9b5acb9988c`  
		Last Modified: Tue, 11 Jan 2022 21:04:50 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8ab45b6c5d9a5110e80693be1a73cc54f1992d97eb4471f61ba5a1a8b81c3`  
		Last Modified: Tue, 11 Jan 2022 21:04:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71628322046041667cb8e76d73a9aa44431130ff2dd2dc4810e0c7d3baadc551`  
		Last Modified: Tue, 11 Jan 2022 21:04:50 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272a9f60350bf47b3f3d2c66736c13a37cad6ecf4f689ae5d7262f659a0a7dd3`  
		Last Modified: Tue, 11 Jan 2022 21:07:29 GMT  
		Size: 145.0 MB (144979471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a837274a2f35f1f68c6d569d5a4b105a8cf085c385b5c3fc8e7f78a04b222b`  
		Last Modified: Tue, 11 Jan 2022 21:04:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.17763.2451; amd64

```console
$ docker pull julia@sha256:68c8baf1c9134e8852bd9d48b44ab6d5c5561d4ff6989ba7d1274ad8c46a9f26
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2856297101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ef8c3a4d40045c7ef6666608142ed798df201a848833f7f5f042010d7fbc397`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 05:42:07 GMT
RUN Install update 1809-amd64
# Tue, 11 Jan 2022 18:28:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 20:51:54 GMT
ENV JULIA_VERSION=1.7.1
# Tue, 11 Jan 2022 20:51:55 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Tue, 11 Jan 2022 20:51:56 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Tue, 11 Jan 2022 20:54:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Tue, 11 Jan 2022 20:54:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ca87ac6c02d88482e9b4bf7c5b3be47ddaa1940332b4730a0b1384b4efb987cf`  
		Size: 993.3 MB (993251600 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d817badb08ee5a6edbd47efdaa8f9393db0c59d351be8a78deda5364ab70de7f`  
		Last Modified: Tue, 11 Jan 2022 18:34:27 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72be21672ff1620f364878554ed9966eda3dd506adc4c51d208442e5818f41f`  
		Last Modified: Tue, 11 Jan 2022 21:07:45 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79adc424414fb796da3f2fc4bd4a6c46d3d0ac18ff963ce382dfa1df0b803d0a`  
		Last Modified: Tue, 11 Jan 2022 21:07:46 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14965c29b836d1a636ded16cbad1e9389f7aad1d8e52327171806fb7a177cf97`  
		Last Modified: Tue, 11 Jan 2022 21:07:46 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38e8c5c5ab189e5e11a27303a127b1355e79e5e7323d20a841ae3c4eb3988ab`  
		Last Modified: Tue, 11 Jan 2022 21:08:34 GMT  
		Size: 144.7 MB (144705585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbbbfd96b7440e3b543783476b45c99fd6572e528dc628cf45036f6a82dafaa`  
		Last Modified: Tue, 11 Jan 2022 21:07:46 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull julia@sha256:0997556804836388defef50dd2921c73e8ea47ed25753fa7484825b3613c77f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6422884189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a741041a48e34c5e80bfbd7ca2121678088559b40864fd77b6ffc6cf70f914cf`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 20:54:23 GMT
ENV JULIA_VERSION=1.7.1
# Tue, 11 Jan 2022 20:54:24 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.1-win64.exe
# Tue, 11 Jan 2022 20:54:25 GMT
ENV JULIA_SHA256=820f31de28d409ae8fda2ea01d39c67564fc6138d010e8b7e5d3d883d7daee23
# Tue, 11 Jan 2022 20:57:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Tue, 11 Jan 2022 20:57:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da716f014e43a5093dace985788c4b2e01f506c5bfc5a137cdc3f6aa923b4d92`  
		Last Modified: Tue, 11 Jan 2022 21:08:51 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa5e27458ca0e2e9af66fd2acbe26aa8689f8ca36762bebdb7a4beaad82408`  
		Last Modified: Tue, 11 Jan 2022 21:08:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d38b3b2c0525ec3e8ca88b4130e4e0b1b1dfa9e71e072423ca65fc49dab1b5`  
		Last Modified: Tue, 11 Jan 2022 21:08:51 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709e3f94b85c549827f0aaab1a35f5b8a176b67cf8a5827be70c480a8de8ba28`  
		Last Modified: Tue, 11 Jan 2022 21:09:36 GMT  
		Size: 144.7 MB (144674373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a124cfcc253a67f7fe68fd24db3b5dea09fa4c813dd190c65a7d5011865eaace`  
		Last Modified: Tue, 11 Jan 2022 21:08:52 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
