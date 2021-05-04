## `hylang:python3.8-windowsservercore-1809`

```console
$ docker pull hylang@sha256:500f050d3ac905457f2f694df299da7d7890daea3202c24892e004691bde0ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `hylang:python3.8-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull hylang@sha256:416ae3d6f4c42f8662ab9630c4812053036ed054fdfbd2f0bb4e3a35f5f995bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2530943404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c70875c7c165769ae73d62f7e0bf6cad07ed9e611fedd89dc1f82494f14a7a4c`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 12:14:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 04 May 2021 17:28:53 GMT
ENV PYTHON_VERSION=3.8.10
# Tue, 04 May 2021 17:28:54 GMT
ENV PYTHON_RELEASE=3.8.10
# Tue, 04 May 2021 17:30:25 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:30:26 GMT
ENV PYTHON_PIP_VERSION=21.1.1
# Tue, 04 May 2021 17:30:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1954f15b3f102ace496a34a013ea76b061535bd2/public/get-pip.py
# Tue, 04 May 2021 17:30:28 GMT
ENV PYTHON_GET_PIP_SHA256=f499d76e0149a673fb8246d88e116db589afbd291739bd84f2cd9a7bca7b6993
# Tue, 04 May 2021 17:31:16 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:31:17 GMT
CMD ["python"]
# Tue, 04 May 2021 17:59:40 GMT
ENV HY_VERSION=1.0a1
# Tue, 04 May 2021 18:00:13 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 04 May 2021 18:00:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc61c4265bfe314fb772d57da4c3023d46cacdbdab9bb6fd5c475f11696dbab`  
		Last Modified: Wed, 14 Apr 2021 16:38:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707dcd915af7dc58b2f45213e86cb211ae0a5a5b12ef0f3ed1093d35642df4ee`  
		Last Modified: Tue, 04 May 2021 17:39:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d395a6dc36655dbf291659f560789ca32dffd4c7e919a13e9a8b99a059f57c`  
		Last Modified: Tue, 04 May 2021 17:39:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b204d0d3ca4da13a65c1461cd0d163146bc4e609cde9423b811492a4cc3a1d`  
		Last Modified: Tue, 04 May 2021 17:39:44 GMT  
		Size: 53.8 MB (53779644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d218a0d099ac27e6c8a6103d4481269430856a8b61ed7259c96f4223662246`  
		Last Modified: Tue, 04 May 2021 17:39:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bed842e43b68833e662a4001c318edcb3040006487ef3a292448d100a4ed828`  
		Last Modified: Tue, 04 May 2021 17:39:33 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def9d0ea705f36ec2f7baa4ec8f176a9ae67b033c84327d90939b8289750693e`  
		Last Modified: Tue, 04 May 2021 17:39:33 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179cbced54ebf5b53547cc1dd0228103fce3971ec8ae6b761c37d131567284d`  
		Last Modified: Tue, 04 May 2021 17:39:36 GMT  
		Size: 6.2 MB (6180054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14fa968ba256fa61d6a9c9704e4fab0cc95cb3fcad5ecdb97f9f4a44d198af8`  
		Last Modified: Tue, 04 May 2021 17:39:34 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8d4259e2b084cb27b595ba055897a7c21ce0c8a2708f208c558a98686c9fd7`  
		Last Modified: Tue, 04 May 2021 18:06:03 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d137ac8ba32c3abe6d62f1ae3da30288fea6f4921a8743cf4b72d2c4610e8a3`  
		Last Modified: Tue, 04 May 2021 18:06:05 GMT  
		Size: 1.2 MB (1215783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2d619605649d316bec10ff86341e9c79ae4693bb89b2c792b0c1cfbb96d168`  
		Last Modified: Tue, 04 May 2021 18:06:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
