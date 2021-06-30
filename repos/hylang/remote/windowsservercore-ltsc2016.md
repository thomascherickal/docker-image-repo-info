## `hylang:windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:462aa7a53fb0941b47c90d4e831d027f0d38f9d86b4b42cdc4a9a1829d0bf286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `hylang:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull hylang@sha256:ff455a2b8fb7247c1a39d294182cdc5c82d277b44113405068ca0ebbd50fab79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327335787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9ea1ba3aaccd640250c731f523f0199c763b645236ace02a6bae96e6601111`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 16:04:34 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 29 Jun 2021 19:17:41 GMT
ENV PYTHON_VERSION=3.9.6
# Tue, 29 Jun 2021 19:17:43 GMT
ENV PYTHON_RELEASE=3.9.6
# Tue, 29 Jun 2021 19:20:13 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 29 Jun 2021 19:20:16 GMT
ENV PYTHON_PIP_VERSION=21.1.3
# Tue, 29 Jun 2021 19:20:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/a1675ab6c2bd898ed82b1f58c486097f763c74a9/public/get-pip.py
# Tue, 29 Jun 2021 19:20:22 GMT
ENV PYTHON_GET_PIP_SHA256=6665659241292b2147b58922b9ffe11dda66b39d52d8a6f3aa310bc1d60ea6f7
# Tue, 29 Jun 2021 19:22:10 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 29 Jun 2021 19:22:13 GMT
CMD ["python"]
# Tue, 29 Jun 2021 20:36:16 GMT
ENV HY_VERSION=1.0a1
# Tue, 29 Jun 2021 20:37:53 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 29 Jun 2021 20:37:55 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfa55ab4db6f7cde43273b96f1f6819cd2c3cea34c5ad67065d7ab4210320a`  
		Last Modified: Wed, 09 Jun 2021 16:26:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e989c7ca4627f18df7e4e05fea6b5d5482b6d2a883caf1f9aeea2c343c6a9`  
		Last Modified: Tue, 29 Jun 2021 20:17:31 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091e7f5457881cf605ca41f9cde6817f31a89e98bdfdfc90ccb237a947567e61`  
		Last Modified: Tue, 29 Jun 2021 20:17:30 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473b6642b74100dc9e9a1a57e1f23cb17d24fb2e0b4bb1290e68a02a002a1ed8`  
		Last Modified: Tue, 29 Jun 2021 20:18:31 GMT  
		Size: 54.2 MB (54158935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0785fc4cccb619ca14adb6b66dae58f0297df0bbe884d7aecfe7cfb4b7562f`  
		Last Modified: Tue, 29 Jun 2021 20:17:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db242a1cb17329e70b673e7870795a477f68644c68be3fcb66cd02d56270b26`  
		Last Modified: Tue, 29 Jun 2021 20:17:28 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba87182174f4387d5e45bac07ef96a274b19c72b1e9311d1b50f9f8bd241d8`  
		Last Modified: Tue, 29 Jun 2021 20:17:28 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8405c9389c1fbcf50973af46f52363c3f5931c5d37949c0418c17f6edc84abc9`  
		Last Modified: Tue, 29 Jun 2021 20:17:35 GMT  
		Size: 6.3 MB (6267994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8026aa29f4fd8029d2725c235352fd9c0b0e4bc67cebd3967c2d5bf1de5394bf`  
		Last Modified: Tue, 29 Jun 2021 20:17:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2005a2a93470d3603ef16f6ba054e20c14f0b93cfc82ab6965b6ae6dcd8555`  
		Last Modified: Tue, 29 Jun 2021 20:39:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f7066205d6505e015a19e52e7e5caa1aa626040e887d03ff844191c4106815`  
		Last Modified: Tue, 29 Jun 2021 20:39:31 GMT  
		Size: 1.2 MB (1167400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e429ce637fa1795fd6ec3de004ff4fe9c4bd8abe12543606a91f69118f77b52`  
		Last Modified: Tue, 29 Jun 2021 20:39:30 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
