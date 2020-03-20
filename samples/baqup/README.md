# Local Quip Backup

Simple command-line script that copy a source directory to a specific directory in your Private folder, based on what data can be exported via the API.

## Running

```
./main.py --access_token="..." --src_root_folder_id="your source folder ID of Quip" --dest_root_folder_id="your destination folder ID of Quip"
```

You can obtain a personal access token via [quip.com/api/personal-token](https://quip.com/api/personal-token). If you wish to target an alternate Quip server, you can use the `--quip_api_base_url` flag.

## Backup to local folder

Please refer to [original repo](https://github.com/quip/quip-api/tree/master/samples/baqup).

Note that the following items are not currently backed up:

* Attachments to conversations
* Images in documents
* Contacts

You may run into rate limiting issues depending on the size of your account.

Resuming of interrupted backups is currently not supported.
