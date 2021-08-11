## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f1449507aa52825898a8dacdb9470b9c2dccd5ea02382258c5c732e30318cf69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:8ce5d7edf34bee59a1392c707dc387d9a6b89d6054bfe96147e768e8b71a7510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852839218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea3f3f05aefea607e65fe88361f8f047733023ab6d05ca77899c33b57dbe3d12`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 12:44:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Aug 2021 12:44:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Aug 2021 12:44:58 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Aug 2021 12:45:01 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Aug 2021 12:46:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:03:48 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Aug 2021 13:05:01 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Aug 2021 13:05:04 GMT
ENV GOLANG_VERSION=1.16.7
# Wed, 11 Aug 2021 13:08:09 GMT
RUN $url = 'https://dl.google.com/go/go1.16.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56b3a9024268f226f679c3a8ffb21f4214a75f84050b2c395b362ae2cc8e53e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 13:08:13 GMT
WORKDIR C:\gopath
# Wed, 11 Aug 2021 21:09:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 21:09:33 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 11 Aug 2021 21:09:36 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 11 Aug 2021 21:09:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 11 Aug 2021 21:10:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 11 Aug 2021 21:10:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1014a0987936e3fa4cd5e9d82f8e82b260d69af19d422f406e4ca0ca868a2c`  
		Last Modified: Wed, 11 Aug 2021 13:29:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e04f285ca5202ce380345855cc1ef257dca5d10c911e569374401b838c36c4`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e030fd545aef8a7a910823c29f1d20459a9cadda6fb139615fc2889d11f9947`  
		Last Modified: Wed, 11 Aug 2021 13:29:32 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e552f09bafcd7011149f53ca4fb6af5814124b3433a4fe57e214782457664`  
		Last Modified: Wed, 11 Aug 2021 13:29:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed64d631b20fa6a2ca7e09eca20fd2e38188e2c5bc403a2eb944f6287397a17`  
		Last Modified: Wed, 11 Aug 2021 13:29:38 GMT  
		Size: 25.4 MB (25449457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f305eae5b6818e3197738445312b2df80302891cbc00f133a0cd4b7ed7046af`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421f7dec205350b61882c53b043a854bd0ab162395ee7016c15d2ff781492b3b`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 321.8 KB (321814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1959338b6b9981d256f2bfb4620c4ed5381b9b0a82b5f9be48d15ca97b9bf02`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b5e2784251d81abc926c9e399929ffe51c2b7a7d34023289da3c6fb4db65ae`  
		Last Modified: Wed, 11 Aug 2021 13:34:44 GMT  
		Size: 139.3 MB (139343081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1889787fe27cffd35a0cffa025a0b7e3c4fd42bd8186d190ac5ead0c6a796`  
		Last Modified: Wed, 11 Aug 2021 13:34:12 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a863a4bc7c6df8d27abe97f0b66f522a010f72b60312ea572ad4284a1d0c6c76`  
		Last Modified: Wed, 11 Aug 2021 21:14:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7983b2c5fc6b18e4b194c9a1cb93d2df4dfa17c2f9da92385ddc2192e4c8d`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3843f7bdb66522a1e0cc0738346c6ac5998803a7ee2ba0ee30591681f3d63c1`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989d649b754c49dddb422bc9f8804f96b4dd683a21047bab1a08e7eb810afa8f`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded6c055915a40954dd327da14ce0d4769121b25df2189dd522750518e2006f`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.7 MB (1708260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a99c4c74f9cc39d201e0b502b35b01475a8782f9abc9b2f7c42b90761f0da7`  
		Last Modified: Wed, 11 Aug 2021 21:14:42 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
