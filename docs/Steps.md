# Bike Rentals Demand Forecasting: Step-by-Step Development Log

## Installation of Libraries and Dependencies

### Create a new repo 'bike-rentals-demand-forecasting' in GitHub (with only MIT License added)

### Install Python 3.12
* `python3.12 --version`  # Python 3.12.13

### Install git
* `sudo apt update`
* `sudo apt install git`
* `git --version`  # git version 2.25.1

### Install uv => An extremely fast Python package and project manager, written in Rust
* `curl -LsSf https://astral.sh/uv/install.sh | sh`
* `uv --version`  # uv 0.11.7 (x86_64-unknown-linux-gnu)

### Use Kedro to create project folder locally with same name as that of GitHub repo
* `cd ~/Work/GitHub`
* `uvx --python 3.12 kedro new`

![Kedro new project output](./images/kedro-new-project-output.png)

### 
* Go to local project folder created by Kedro => `cd ~/Work/GitHub/bike-rentals-demand-forecasting`
* Initialize git => `git init`
* Connect to our GitHub remote repo => `git remote add origin https://github.com/ancilcleetus/bike-rentals-demand-forecasting`
* Verify the remote was added => `git remote -v`
* Add files => `git add .`
* Initial commit => `git commit -m "Initial commit: Kedro project setup for Bike Rentals Demand Forecasting"`
* Set branch to main => `git branch -m main`
* Pull remote changes and merge => `git pull origin main --allow-unrelated-histories`
* Push to main => `git push -u origin main`

```
Built antlr4-python3-runtime==4.9.3
Installed 40 packages in 63ms
[04/21/26 12:00:53] INFO     Using                                                                                             __init__.py:275
                             '/home/ancil/.cache/uv/archive-v0/vWsyMUiGvTvKLdJXGJpYv/lib/python3.12/site-packages/kedro/framew                
                             ork/project/rich_logging.yml' as logging configuration.                                                          

Project Name
============
Please enter a name for your new project.
Spaces, hyphens, and underscores are allowed.
To skip this step in future use --name
 [New Kedro Project]: Bike-Rentals-Demand-Forecasting

Project Tools
=============
These optional tools can help you apply software engineering best practices.
To skip this step in future use --tools
To find out more: https://docs.kedro.org/en/stable/create/new_project_tools/#tools-to-customise-a-new-kedro-project

Tools
1) Lint: Basic linting with Ruff
2) Test: Basic testing with pytest
3) Log: Additional, environment-specific logging options
4) Docs: A Sphinx documentation setup
5) Data Folder: A folder structure for data management
6) PySpark: Configuration for working with PySpark

Which tools would you like to include in your project? [1-6/1,3/all/none]:
 [none]: 1-5

Example Pipeline
================
Select whether you would like an example spaceflights pipeline included in your project.
To skip this step in the future use --example=y/n
To find out more: https://docs.kedro.org/en/stable/create/new_project_tools/#tools-to-customise-a-new-kedro-project

Would you like to include an example pipeline? [y/N]:
 [no]: N

Congratulations!
Your project 'Bike-Rentals-Demand-Forecasting' has been created in the directory 
/home/ancil/Work/GitHub/bike-rentals-demand-forecasting

You have selected the following project tools: ['Linting', 'Testing', 'Custom Logging', 'Documentation', 'Data Structure']
[04/21/26 12:02:51] WARNING  /home/ancil/.cache/uv/archive-v0/vWsyMUiGvTvKLdJXGJpYv/lib/python3.12/site-packages/kedro/framewo warnings.py:112
                             rk/cli/starters.py:239: UserWarning: Your project does not contain any pipelines with nodes.                     
                             Please ensure that at least one pipeline has been defined before executing 'kedro run'.                          
                               warnings.warn(                                                                                                 
                                                                                                                                              

To skip the interactive flow you can run `kedro new` with
kedro new --name=<your-project-name> --tools=<your-project-tools> --example=<yes/no>
                    INFO     Kedro is sending anonymous usage data with the sole purpose of improving the product. No personal   plugin.py:242
                             data or IP addresses are stored on our side. To opt out, set the `KEDRO_DISABLE_TELEMETRY` or                    
                             `DO_NOT_TRACK` environment variables, or create a `.telemetry` file in the current working                       
                             directory with the contents `consent: false`. To hide this message, explicitly grant or deny                     
                             consent. Read more at https://docs.kedro.org/en/stable/about/telemetry/
```
