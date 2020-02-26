## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:702f5ed9a4eec35af10690c6264158871705309e78a0bed978a29330aafa1b49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3506; amd64
	-	windows version 10.0.17763.1040; amd64

### `golang:1-windowsservercore` - windows version 10.0.14393.3506; amd64

```console
$ docker pull golang@sha256:70ee2e2309c511b95a695bf5abae98406dd72ed89c939e6e33a094049f0a8982
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5905555290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8b972741e20cc99b5edb55931c3665ec1b9a9a495c13e6015c6946afcedbbb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 14 Feb 2020 21:42:00 GMT
RUN Install update ltsc2016-amd64
# Thu, 20 Feb 2020 01:48:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 09:14:29 GMT
ENV GIT_VERSION=2.23.0
# Thu, 20 Feb 2020 09:14:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 20 Feb 2020 09:14:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 20 Feb 2020 09:14:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 20 Feb 2020 09:16:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 20 Feb 2020 09:16:17 GMT
ENV GOPATH=C:\gopath
# Thu, 20 Feb 2020 09:17:39 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Feb 2020 00:24:17 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 00:31:39 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'cc2f1e8d19744fe0b2e979bf9a4f9d224e416f4f54cb6cf3aa8b5e9c0865de37'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Feb 2020 00:31:41 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:846a2223e9e7a88a2a07d706553f144d380483d72fb9f0697c4fcd71773a8693`  
		Size: 1.7 GB (1657079102 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:72c4471958f7f0f07260f0f430bcffb0bc07811088c24cffba1439d250ea1ae3`  
		Last Modified: Thu, 20 Feb 2020 03:04:52 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560a5edc3b65548cd8f0a5736740259c10731b69be646647541d454f4a46d74d`  
		Last Modified: Thu, 20 Feb 2020 10:16:28 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d778cb1587245dbb3aa1eadff960d2ca6808181a7f76399e1461b4488dd0d110`  
		Last Modified: Thu, 20 Feb 2020 10:16:27 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc71d139522c2d69f799715a806ce8ce02bd536d9fb33c3c1cff0d512c06ebe`  
		Last Modified: Thu, 20 Feb 2020 10:16:25 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3aec6ae82f728acb67ab3203c9f84faf93c0ff671c1d1341837da6f6127ec3`  
		Last Modified: Thu, 20 Feb 2020 10:16:25 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6734e518b8f70059c148a428fbd47fe51d143e43477597a7b34afb502090a6cd`  
		Last Modified: Thu, 20 Feb 2020 10:16:57 GMT  
		Size: 30.5 MB (30460160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52c1cb26338697dbffd8fd282e956aa88db7f630a7b5c1c90f750eee04c24e4`  
		Last Modified: Thu, 20 Feb 2020 10:16:22 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58993efc965e34067a71381b74e269f61cff043dfd64a430cddfcd494cd3f21`  
		Last Modified: Thu, 20 Feb 2020 10:16:24 GMT  
		Size: 5.3 MB (5316014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7346524e3170cae52e12ecf555dfa52b9ccd9595caebb7bd8ad48d9573ea9e9`  
		Last Modified: Wed, 26 Feb 2020 00:45:02 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f79df10c0d625a69d6eab9a3e306a15502d190b55ea12b3b74aad531144875c`  
		Last Modified: Wed, 26 Feb 2020 00:46:44 GMT  
		Size: 142.7 MB (142704440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcad0e327f58fe14b1d910c5f02f0b0195f9b99ea4d1bc3b5702f65bfbbd9c31`  
		Last Modified: Wed, 26 Feb 2020 00:45:01 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-windowsservercore` - windows version 10.0.17763.1040; amd64

```console
$ docker pull golang@sha256:783c9f02622941eeafbbd695d354deb406eeedb800a16794407966c24d220201
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2393659233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe21e2f9b814b5f9db1378b2bf56ec6e2a5e9af2c51c3d7bbb8c2458ea406d5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 17 Feb 2020 06:57:13 GMT
RUN Install update 1809-amd64
# Thu, 20 Feb 2020 01:13:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 09:24:51 GMT
ENV GIT_VERSION=2.23.0
# Thu, 20 Feb 2020 09:24:52 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 20 Feb 2020 09:24:53 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 20 Feb 2020 09:24:54 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 20 Feb 2020 09:26:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 20 Feb 2020 09:26:04 GMT
ENV GOPATH=C:\gopath
# Thu, 20 Feb 2020 09:26:30 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Feb 2020 00:31:56 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 00:37:54 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'cc2f1e8d19744fe0b2e979bf9a4f9d224e416f4f54cb6cf3aa8b5e9c0865de37'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Feb 2020 00:37:55 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5405b7580792436b60c664b5fa766ea57f5a60c1d9a8c522cf53e99e4813355`  
		Size: 695.8 MB (695818606 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2061e035d6ba931d9f00238104b970d3410f4ef0d9603b4f074c7052858e01e3`  
		Last Modified: Thu, 20 Feb 2020 03:03:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110dad01ccee3d09fea60ea0d52694e30fd66dde9aba2b80aecf974b583e715e`  
		Last Modified: Thu, 20 Feb 2020 10:18:49 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08227349fdb2e96c42cfe1dd8b9fc4d8a4a85e9a303fe293727eb01701bbcacf`  
		Last Modified: Thu, 20 Feb 2020 10:18:47 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fee65f96c94d8080d815d503bbc149109dd1f67641301deb251ab9473035e6`  
		Last Modified: Thu, 20 Feb 2020 10:18:47 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca5f0dbb9e1f23daefbfb48689ca6dbf034e885572be47a1ddab25dbd2daf2b`  
		Last Modified: Thu, 20 Feb 2020 10:18:47 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3010ef660c0462ec39174065b9aab710d1d830c63d271b91f0fa7ba9e7db38`  
		Last Modified: Thu, 20 Feb 2020 10:18:59 GMT  
		Size: 29.6 MB (29649597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1950846c735f1005e0ddd4a3bf964daa3d2b82a96afbbe1a9db1b1cfe95ad623`  
		Last Modified: Thu, 20 Feb 2020 10:18:44 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4aa2e260f5863265a5a10dd0bc9437eff66a067199e59f228354fa33138657`  
		Last Modified: Thu, 20 Feb 2020 10:18:44 GMT  
		Size: 294.9 KB (294889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12b2cdac232e26aed4b1374d7e9437c44ceada6080e6f4aa12e01967102c13`  
		Last Modified: Wed, 26 Feb 2020 00:47:29 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab772824c5623e72e87291a7ff11fd664713feb46c412710177e74607c1f5d`  
		Last Modified: Wed, 26 Feb 2020 00:49:06 GMT  
		Size: 133.2 MB (133201112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb32b723fc0235debf87ddc0af1ad3ec9670f574b1fe405b1322e14473f53eb`  
		Last Modified: Wed, 26 Feb 2020 00:47:28 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
