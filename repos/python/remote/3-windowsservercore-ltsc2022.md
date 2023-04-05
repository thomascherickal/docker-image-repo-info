## `python:3-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:fb4aaa63f7a9a5d82bb9533ffb463eb43103858b8417b0ea4504bcf2bffed9d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `python:3-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull python@sha256:8fc6c8336b4301828fcb6e2a47955f50c82dd027c60316d2615412f115c69bfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1770803247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e906f1ab098c5e21431bbcd2c42c63c9b8b1e4fec27b53a3192311e94877e8`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 07:40:54 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 05 Apr 2023 21:36:59 GMT
ENV PYTHON_VERSION=3.11.3
# Wed, 05 Apr 2023 21:38:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 05 Apr 2023 21:38:21 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Wed, 05 Apr 2023 21:38:22 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 05 Apr 2023 21:38:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Wed, 05 Apr 2023 21:38:24 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Wed, 05 Apr 2023 21:39:13 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 05 Apr 2023 21:39:14 GMT
CMD ["python"]
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
	-	`sha256:fcd97074c3f9b465d0ad8267ca2ad1662279ea7cc6464b4b890b784732671ae6`  
		Last Modified: Thu, 16 Mar 2023 08:07:56 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4aa88eb02587ad1f330e15f961e96fc71cde774b2d09767bee0120bcbb9a90`  
		Last Modified: Wed, 05 Apr 2023 21:50:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be382e385fc6f3aaaed252cf86e2d942b8c85ade4aa85a38a065a8bd1cfe4fda`  
		Last Modified: Wed, 05 Apr 2023 21:50:50 GMT  
		Size: 50.9 MB (50920935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5defcc2ecdc470d72f19cca0819ff5302c521e2e78e97d8378f8dab764967efa`  
		Last Modified: Wed, 05 Apr 2023 21:50:43 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66da28e12a518abfdfaaa0869944a83637211c19ef504699f4c686a3e8707e4f`  
		Last Modified: Wed, 05 Apr 2023 21:50:41 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155984ddeb3d8a091de79aca6464b23b4d30775997c43a62d1fb00e8d344cc76`  
		Last Modified: Wed, 05 Apr 2023 21:50:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b5394aa72f0ed7d9cf8a2268ca0be0ee9654869b08f39e00a3449a53e692ee`  
		Last Modified: Wed, 05 Apr 2023 21:50:41 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146af1876a4d644feab6d5fdc9052ece14ed5d493f8e0df2cc0fd0b19f1cb25`  
		Last Modified: Wed, 05 Apr 2023 21:50:43 GMT  
		Size: 5.9 MB (5931021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6735a17632751e451f7d8086b9222ec3dd9b34bc27f948da5b5d09a28faa66b7`  
		Last Modified: Wed, 05 Apr 2023 21:50:41 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
