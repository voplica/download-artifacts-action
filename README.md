### Download Artifacts Action

This action allows to download multiple artifacts represented by JSON array.

Parameters:
- `repository` (**Required**, *string*) - The repository owner and the repository name joined together by "/".
- `github_token` (**Required**, *string*) - GitHub token to be used for artifacts download process.
- `download_artifacts_json` (*string*) - JSON array representing attached GitHub Action artifacts of the commit to be used for the build process. All files represented in the JSON array will be downloaded and used for the build process. The JSON array must be in the format: `[{"name": "artifact name", "path": "artifact destination path relative to repository root folder", "run_id": "run id where to find the files"}]`.
- `scope_path` (*string*) - Base directory path where all artifacts will be extracted. Paths in download_artifacts_json will be relative to this directory.

###### © 2025 Voplica LLC
