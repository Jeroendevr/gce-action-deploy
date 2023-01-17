# Path
## Steps taken to create the GitHub Action as a reference for myself later or for someone else to create it. 

- [gcloud compute docs](https://cloud.google.com/compute/docs/gcloud-compute?hl=en_US)

### Google Cloud CLI
[Installation Google Cloud CLI](https://cloud.google.com/sdk/docs/install-sdk)
- Installed Python version 3.9.6, Default macOS python on Ventura
- Install the package using the HomeBrew package manager
  - `brew install --cask google-cloud-sdk`
  - As instructed during installation add gcloud to path. 
    - In my case I use the Fish sheel 
      - `source "/opt/homebrew/Caskroom/google-cloud-sdk/latest/google-cloud-sdk/path.fish.inc"`
      - `exec fish` to restart shell
      - Check if gcloud is correctly installed typing `gcloud -v` resulting in 

      ```Shell
      Google Cloud SDK 413.0.0
      bq 2.0.84
      core 2023.01.06
      gcloud-crc32c 1.0.0
      gsutil 5.17
      ```
- Back to the original docs $ `gcloud init`
  - Succefull redirect to auth_succsess after logging in
- follow shell prompt to configure region

🎉 installation complete
  

### Google Cloud Python Client lib
Available through pip see [GitHub repo](https://github.com/googleapis/python-compute)
Added to the project requirements

