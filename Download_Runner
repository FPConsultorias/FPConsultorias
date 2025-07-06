# Create a folder under the drive root
$ mkdir actions-runner; cd actions-runner# Download the latest runner package
$ Invoke-WebRequest -Uri https://github.com/actions/runner/releases/download/v2.325.0/actions-runner-win-x64-2.325.0.zip -OutFile actions-runner-win-x64-2.325.0.zip# Optional: Validate the hash
$ if((Get-FileHash -Path actions-runner-win-x64-2.325.0.zip -Algorithm SHA256).Hash.ToUpper() -ne '8601aa56828c084b29bdfda574af1fcde0943ce275fdbafb3e6d4a8611245b1b'.ToUpper()){ throw 'Computed checksum did not match' }# Extract the installer
$ Add-Type -AssemblyName System.IO.Compression.FileSystem ; [System.IO.Compression.ZipFile]::ExtractToDirectory("$PWD/actions-runner-win-x64-2.325.0.zip", "$PWD")
