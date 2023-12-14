# Easy ETL Template
The templated version of our [Easy ETL example](https://github.com/xetdata/easy-etl).

## Usage 

Configuring the repo:
1. Click `Use this Template`, and select `Create a new repository`.
2. Fill out the repository information and click `Create Repository`.
3. Add write permissions to Actions. This enables the pipeline to check the files back into the repo. Click on the repo Settings. Select `Actions` and `General`. Scroll down to `Workflow permissions`, and select `Read and write permissions`. Click `Save`.
4. Follow the instructions at [XetData integration for GitHub](https://github.com/apps/xetdata) and install the app to your new repo
5. Edit `.github/workflows/etl-action.yml` and remove the comments from the schedule section. Set `AUTOMATION_USERNAME` to a good username and `AUTOMATION_EMAIL` to a good email address.

Making it your own:
1. Edit `src/pipeline.py` and replace the code in `extract()` with your own ETL code.
2. Make sure to save your requirements with `pip freeze > requirements.txt`
3. Commit and push your changes.

At the 21st minute of the next hour, your ETL pipeline will be run. Couldn't be easier!

