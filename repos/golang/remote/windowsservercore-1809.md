## `golang:windowsservercore-1809`

```console
$ docker pull golang@sha256:85164fbd097e37f2f9baced9e9fbe435c8c17ef89bdd9cdb744d1e990abe0466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `golang:windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull golang@sha256:631a1f9412663b15e0206d83a2a31e606f518a0cda14161af2aea3c03ebac2f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2561055990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62c1402eaa8922f53556dc4de62d175471c8d3e1a44decc303eb9dd4af1f7b8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 13:43:36 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Nov 2020 13:43:37 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Nov 2020 13:43:38 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Nov 2020 13:44:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 13:44:33 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Nov 2020 13:44:55 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 04 Dec 2020 00:15:09 GMT
ENV GOLANG_VERSION=1.15.6
# Fri, 04 Dec 2020 00:17:48 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b7b3808bb072c2bab73175009187fd5a7f20ffe0a31739937003a14c5c4d9006'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 04 Dec 2020 00:17:50 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19e00ae033e023d5973e57402eb3f05fe0908fa3f40cd0a36ae20bc72df3927`  
		Last Modified: Wed, 11 Nov 2020 14:08:35 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7f2350f21c33479862fe11c4c46ef7fc8054cb8e0acb2581b663d9e71d37f4`  
		Last Modified: Wed, 11 Nov 2020 14:08:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816110035a14bde6916267f7e5f008617773d19d8f23f77597d10b021b787c`  
		Last Modified: Wed, 11 Nov 2020 14:08:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7a389242a4449d1ca90994817f199ce0b9ec502e46035e6ea9c78c29282ce8`  
		Last Modified: Wed, 11 Nov 2020 14:08:29 GMT  
		Size: 1.1 KB (1098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993585709f02af194d96f01fb74b3158a083cac1cbf2036662bd0abab75e3bf`  
		Last Modified: Wed, 11 Nov 2020 14:08:38 GMT  
		Size: 34.3 MB (34333277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a63153155fc14ab856f02664a39a3dbf45ef8601277d161d64e9475748111`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758771af484f25fbbe9ef11107e3680d525f6bfc5a1666db73f0eb9d84be3ef1`  
		Last Modified: Wed, 11 Nov 2020 14:08:26 GMT  
		Size: 311.3 KB (311320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05164df22cc1044ebebf255e3f078aca1c5d0b01cfed997c4c52ac57268041e`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d208cb88aaef7d49293e8b5fe6cb80e9520f49d127c6991f47c4a360628ef2`  
		Last Modified: Fri, 04 Dec 2020 00:33:47 GMT  
		Size: 138.4 MB (138372930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219a39d338a89418edc5b2a3e6949d4b7c9055ce4dac36812ee963d3454525ec`  
		Last Modified: Fri, 04 Dec 2020 00:33:08 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
