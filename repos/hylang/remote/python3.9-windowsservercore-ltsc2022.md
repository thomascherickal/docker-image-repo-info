## `hylang:python3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:ae6773d8d8ecce9209c0f170a4d3cdd063c181b78de89e965fa145ff17bfd66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `hylang:python3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull hylang@sha256:792fa48595d2e3d4f49104c02a0941d9d629f67215c30f304dec520a807daeeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2242614249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dffdc4cede340d6c4c6fb41fce591c7c4a46b74827f9f783a28bed8ab723a01`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 01:38:21 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 16 Nov 2021 18:16:23 GMT
ENV PYTHON_VERSION=3.9.9
# Tue, 16 Nov 2021 18:16:24 GMT
ENV PYTHON_RELEASE=3.9.9
# Tue, 16 Nov 2021 18:17:43 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 16 Nov 2021 18:17:45 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 16 Nov 2021 18:17:46 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Tue, 16 Nov 2021 18:17:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Tue, 16 Nov 2021 18:17:48 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Tue, 16 Nov 2021 18:18:37 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 16 Nov 2021 18:18:38 GMT
CMD ["python"]
# Fri, 03 Dec 2021 23:17:26 GMT
ENV HY_VERSION=1.0a3
# Fri, 03 Dec 2021 23:18:09 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Fri, 03 Dec 2021 23:18:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf213104327874c948c49178d2338f922bb9443acdcbffa4029d62be119c81e1`  
		Last Modified: Wed, 10 Nov 2021 02:07:38 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab30350a41a6a0d7f7b4bf1af2027c9c8065cb1b38c2d0fbe7a849c7922ef79c`  
		Last Modified: Tue, 16 Nov 2021 18:27:25 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04464805fc465781fd4fee8e691dbd7bae5aa9ebf8f2923653bbd563bbaedb2`  
		Last Modified: Tue, 16 Nov 2021 18:27:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c94c913a25e7cd7520f30c30ae468e5627fcd48f08943d1a53a2e89ad948cc`  
		Last Modified: Tue, 16 Nov 2021 18:27:32 GMT  
		Size: 49.9 MB (49876437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a1454356acfb48095bb6591a8dae67bdba21bcc28456ccddac4ce695acf03c`  
		Last Modified: Tue, 16 Nov 2021 18:27:25 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13caa3bd31281eb06082f61e3beceece23b5e66665fc4b4d2e066df51a336e9a`  
		Last Modified: Tue, 16 Nov 2021 18:27:22 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add5ee8c73c829364189a678f2622a44ad006e690ef86e6c495a0a6c66c4a131`  
		Last Modified: Tue, 16 Nov 2021 18:27:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4863573aacb7cdce8870db537e618d0f3074e797762fa3e62f6150ba5dd210f`  
		Last Modified: Tue, 16 Nov 2021 18:27:23 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee59705e9024973703964d3bcc87faa472748832b129d556667f558169a67128`  
		Last Modified: Tue, 16 Nov 2021 18:27:25 GMT  
		Size: 6.5 MB (6544920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c64efa5ef000a0417d9baeb4c87f188b919eed4a73a2c7c8d1784272cd5dfb`  
		Last Modified: Tue, 16 Nov 2021 18:27:23 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdf45f95a38be338c4da779df0fd4def77977ccd6718aefcb81de27d264ae99`  
		Last Modified: Fri, 03 Dec 2021 23:19:02 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd268a9150b85641db351e9f6a0d88a59188e3d36b563bafca76c6b7e30d00b9`  
		Last Modified: Fri, 03 Dec 2021 23:19:03 GMT  
		Size: 1.6 MB (1571164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4adbbfa898f6d25086c79ee580b585ebf494d0378307ee8ad371107de82d732`  
		Last Modified: Fri, 03 Dec 2021 23:19:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
