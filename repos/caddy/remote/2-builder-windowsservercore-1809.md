## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fc7d6643b94f172dc0be1c2a55fe404556c0ef4308cd01485587e677fd69b58f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:3de92bc248f5c55fbbf909bdc0cfe04c78ecf4fcf03ec0ae872dd44aeb090d05
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2854787814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861ecafd471cf14be1765577c8f08fa3fed43d0cb7df37ddf85109fd9f6e4649`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:53:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:53:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:53:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:53:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:55:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:55:12 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:56:14 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:35:47 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:39:58 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:40:00 GMT
WORKDIR C:\go
# Wed, 07 Sep 2022 21:16:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 07 Sep 2022 21:16:58 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 07 Sep 2022 21:16:59 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 07 Sep 2022 21:17:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 07 Sep 2022 21:18:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 07 Sep 2022 21:18:11 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c8de3c3b75d5e4df16d5b51d2629a7ea48fef427269b895425ddf83e4648f`  
		Last Modified: Wed, 10 Aug 2022 13:25:13 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379e9d7c93c53a7225d517ef3bbf5ac5db662822c6b033ba0f86e57f553f9f1`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04c4fbebbd0c6b7ec0d088c9f85358565ade6536be3c27ec839439c70b3300`  
		Last Modified: Wed, 10 Aug 2022 13:25:10 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345f3fbeaf81942e1e576c351394bee7910b1bd200d739562499849161810b00`  
		Last Modified: Wed, 10 Aug 2022 13:25:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daa4ce5f809aaf1eb408a95c9c6bb87f8b8971efb28085fb12419172bc3769b`  
		Last Modified: Wed, 10 Aug 2022 13:25:17 GMT  
		Size: 25.4 MB (25441513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a64bd2b96a29fef52e63363ec6219a5a846d18825d515fdd5c5a45d62eaf71`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ccb61f1f7e4a0d3ecd876f61280913525a4ef70cc4b82b16a164f4fe7f982`  
		Last Modified: Wed, 10 Aug 2022 13:25:07 GMT  
		Size: 315.2 KB (315177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d265b2a28190a611bcb47ea481b8e37f6ce40342e126467ee036f9ecb6d76537`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3009d4611cc39c4c933938da548087d85eb51cc6f958a79f7369a0f3bc6af426`  
		Last Modified: Tue, 06 Sep 2022 19:53:24 GMT  
		Size: 149.7 MB (149670247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bbd410a3f499639592e2cc812b7673e828b6a661c9fe59cdaf3638b85e8211`  
		Last Modified: Tue, 06 Sep 2022 19:52:51 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11922eca83b19d39878beb1b9b1759567513788da369945dbfde6c19fa4769`  
		Last Modified: Wed, 07 Sep 2022 21:26:57 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1045ddf8cc56a13b1715db40d3a3e5c6dde66f34c9e80db4ad8034a8c084bb7`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920eb2db0fd67833662a7592b66ef1c7f0cb636f9a8c4720f93b20ffe0d81651`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21f0787ba24a8a24659e3d43a24b71d42a5529f1e0ef1d476186a103966b1b`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761abb1b36781ecde305f3a8b2797344c9d547d047f6e6ded3d154159bbd312`  
		Last Modified: Wed, 07 Sep 2022 21:26:56 GMT  
		Size: 1.6 MB (1629579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c950750c1191802ec3ccf59500d6ee997d0bdf4d152b61f49b1c9775db8c846e`  
		Last Modified: Wed, 07 Sep 2022 21:26:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
