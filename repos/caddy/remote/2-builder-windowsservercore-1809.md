## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8c945eeb5d1d62d1b05b7f0ec48c00bf6e000b0cf9c3473664ebcee6988c8326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull caddy@sha256:04a79bb884e5e5d84860a496bb2297ecb60a97d62bceda8f9d31389b86701260
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2614309897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c4d2a0575b4575e7784df3b628eaf3f076af0143d49a5712bb9a8944493899`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 13:14:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Feb 2021 13:14:03 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Feb 2021 13:14:04 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Feb 2021 13:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 10 Feb 2021 13:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:25:54 GMT
ENV GOLANG_VERSION=1.15.8
# Wed, 10 Feb 2021 13:27:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'ef05b7141d3c217fb076f0e27249e144296234df96ead8751c0b76784079df97'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:27:50 GMT
WORKDIR C:\gopath
# Wed, 10 Feb 2021 19:47:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 19:47:16 GMT
ENV XCADDY_VERSION=v0.1.7
# Wed, 10 Feb 2021 19:52:39 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 10 Feb 2021 19:52:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 Feb 2021 19:53:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d4e21865693dfb6d4aa2a9d23a7e20ca3a30e03b8f626900ff764d8e9eda1f9ca4c98b0466c6f3676ff1b170974c5cb0f984d04999b4c46becc76a8da50f792d')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 Feb 2021 19:53:03 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b02a688b62e8e70705b5d1eeaae912e44e9fb6dd72cfefc104982d61c555f`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbc05d8cabd13ca38228cb52a2a4c1144c7a230b2c59e2e11b26f1f144f5dd`  
		Last Modified: Wed, 10 Feb 2021 13:40:39 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43183d44ab364a973f5b73ff7a25c64275f549270530373ee2db74a34404e1b`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f513f88f9dc5ce71832909da5e955a3a3d296b702102944db6ca5c498214b6d`  
		Last Modified: Wed, 10 Feb 2021 13:40:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139b8f328890188c74ac1ae76bc6aa32280a2598b71a4ed5d4821f2c5b5e625`  
		Last Modified: Wed, 10 Feb 2021 13:40:48 GMT  
		Size: 34.5 MB (34502138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87101ed6b28acc441dcda26e57ab2abeb02d98e08ad3efbec5597860a60977a`  
		Last Modified: Wed, 10 Feb 2021 13:40:35 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133b426ccf53b1f8e53b86fe63ca8d274a5cd4f33a63ffde34f773a31275525d`  
		Last Modified: Wed, 10 Feb 2021 13:40:36 GMT  
		Size: 321.1 KB (321091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c6b9b5f97caa3a4514c225d23eee3c9637020d8783b74ae29146479e0d46da`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14c3f9a47099dd247ef891ed5a51ec1bc60c166fdb78441658e6325513a73e`  
		Last Modified: Wed, 10 Feb 2021 13:43:38 GMT  
		Size: 138.5 MB (138494761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f053b8b58f33b809c3c367f6dbc8d44683a1ad5308dffcf9722f78885abd452a`  
		Last Modified: Wed, 10 Feb 2021 13:43:09 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef70049702aacf5a1db6677de1cbe8f09047fb18552144d7460229f4ff1669`  
		Last Modified: Wed, 10 Feb 2021 19:56:10 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624050d881979f8ae4b04532d5b9c1c68a2140ec8fb9cb20f6730c65bce4486b`  
		Last Modified: Wed, 10 Feb 2021 19:56:08 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc95294ead6f2d7872163ad8f6fdb143db8272458bd64ac8fa58ddc7608b5a7`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2135c5e359e3a69209dce27b5d588f47198143b0e58431d5c3734c43e5293d9`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d4057944ea00380c302d38712b1cfd1ecbf6e3ff8f818824cc825639272a15`  
		Last Modified: Wed, 10 Feb 2021 19:57:31 GMT  
		Size: 1.7 MB (1707381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42268ed1b86fde2a5a4aa1241c611eb877e22675794a91d76fbc3e23ca3454de`  
		Last Modified: Wed, 10 Feb 2021 19:57:29 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
