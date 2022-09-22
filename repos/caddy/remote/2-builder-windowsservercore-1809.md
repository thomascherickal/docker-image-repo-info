## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9c5d756ef5065110fe986b28f92f1fb4054117a7ec29af6ba748bbe5a9844471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:23c7efb529472abe36c3a41b435f8065744545203b52960a92eb147d7000ed5f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888529673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5a96673f8b73805e57100801d8974f6f027e2391028ae75f53eeba868339df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Sep 2022 12:55:35 GMT
ENV GOLANG_VERSION=1.19.1
# Wed, 14 Sep 2022 12:58:58 GMT
RUN $url = 'https://dl.google.com/go/go1.19.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b33584c1d93b0e9c783de876b7aa99d3018bdeccd396aeb6d516a74e9d88d55f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:59:00 GMT
WORKDIR C:\go
# Wed, 14 Sep 2022 18:00:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 18:00:59 GMT
ENV XCADDY_VERSION=v0.3.1
# Thu, 22 Sep 2022 19:18:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:18:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 22 Sep 2022 19:19:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 22 Sep 2022 19:19:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8814f02c21aff38f5fa9adfffb3c684366a8399428ce5182908d6d99aabfb5f9`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee9723248ef725c331a4228b989a1c074baa23bd2f02066e81ab13109e5cbf3`  
		Last Modified: Wed, 14 Sep 2022 13:25:07 GMT  
		Size: 157.5 MB (157547676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47be49b3a74f40722cc506752c0803f0f9cedb16fef286fda14b840d31427384`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.6 KB (1570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d248e708c50b3ff0f8f6a8c999580dac396e3fb9a73762de23ec138b30fbcb`  
		Last Modified: Wed, 14 Sep 2022 18:05:25 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6efbf87d10bd599184ffd62280896a1479bd9b52b29ce36b30ff97af80d31b`  
		Last Modified: Wed, 14 Sep 2022 18:05:23 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180b1c411897e6d42c7a69e23ebc5a276a0c824804e9d70d0c05c91147209cd5`  
		Last Modified: Thu, 22 Sep 2022 19:21:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cb8805fa05101ce6420d45ed4ce2a75a43ab77c0319581ec579df9af383f70`  
		Last Modified: Thu, 22 Sep 2022 19:21:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5092d2e8bd34adf1f20374cb62f252ffacc3158c15af03725dd5df51c9c4e8e`  
		Last Modified: Thu, 22 Sep 2022 19:21:42 GMT  
		Size: 1.6 MB (1637391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb16b30bb4d353fd35dfc31b99be9aa1c7f6d7e84b5cd4f1c4ad814cfee8f726`  
		Last Modified: Thu, 22 Sep 2022 19:21:42 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
