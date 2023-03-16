## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:2e8a4be822107da84510e9420e45153402e0561172b7d440cc58d9e42282e59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
