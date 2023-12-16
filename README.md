# Google-Collab-Script-to-Remotely-Upload-Files-to-Your-Google-Drive
This script enables parallel downloading of files from Google Drive and other direct download links. It converts Google Drive view links into download links, and uses Python's concurrent.futures for efficient multi-threaded downloads. It's designed for use in Google Colab, and mounts your Google Drive for file storage.

# Google Drive and Direct Download Links Downloader

This script enables parallel downloading of files from Google Drive and other direct download links in Google Colab. It converts Google Drive view links into download links and uses Python's `concurrent.futures` for efficient multi-threaded downloads.

## Prerequisites

- Google Colab environment
- Google Drive mounted on the Colab environment

## Usage

1. **Mount Google Drive**: The script mounts your Google Drive to the Colab environment for file storage.

2. **Specify Links**: Replace the `google_drive_view_links` and `other_links` variables with your own string of Google Drive view links and list of other direct download links.

    ```python
    google_drive_view_links = 'https://drive.google.com/file/d/1JIeDf-U-Ipn3qp6BOKQQT6nIhQIUnqou/view,https://drive.google.com/file/d/1WXSmhpfQgGtbv-RUXxfAXduWxmIq4nk6/view'
    other_links = ['http://example.com/file1', 'http://example.com/file2']
    ```

3. **Specify Save Location**: Replace the `output` variable with your desired save location.

    ```python
    output = '/content/drive/My Drive/gdrivefiles/'
    ```

4. **Run the Script**: Run the script in your Google Colab environment. It will download the files from the specified links in parallel to the specified location.

## Note

While this script speeds up the total download time, it also increases the load on your network connection, as multiple files are being downloaded at once.
