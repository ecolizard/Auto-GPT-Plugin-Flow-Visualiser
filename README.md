# Auto-GPT-Visualiser

A starting point for developing your own external plug-in for Auto-GPT

# **If you want your plugin to live within the codebase, use the example in the [plugins repo](https://github.com/Significant-Gravitas/Auto-GPT-Plugins) instead**

### Plugin Installation Steps

for Linux, depending on distro
```
sudo apt-get install zip
apk add zip
sudo pacman -S zip
sudo yum install zip
```
Mac / Linux / WSL
```
cd plugins && git clone https://github.com/ecolizard/Auto-GPT-Plugin-Flow-Visualiser.git && zip -r ./Auto-GPT-Visualiser-Plugin.zip ./Auto-GPT-Todoist-Plugin && rm -rf ./Auto-GPT-Visualiser-Plugin && cd .. && ./run.sh --install-plugin-deps

```
Windows, Powershell
```
cd plugins; git clone https://github.com/ecolizard/Auto-GPT-Plugin-Flow-Visualiser.git; Compress-Archive -Path .\Auto-GPT-Visualiser-Plugin -DestinationPath .\Auto-GPT-Visualiser-Plugin.zip; Remove-Item -Recurse -Force .\Auto-GPT-Visualiser-Plugin; cd ..
```



5. **Allowlist the plugin (optional):**
   Add the plugin's class name to the `ALLOWLISTED_PLUGINS` in the `.env` file to avoid being prompted with a warning when loading the plugin:

   ``` shell
   ALLOWLISTED_PLUGINS=AutoGPT-Visualiser-Plugin
   VISUALISER_TOKEN=Your_api_token
   ```

   If the plugin is not allow listed, you will be warned before it's loaded.
 
