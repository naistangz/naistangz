[![Anais' github stats](https://github-readme-stats.vercel.app/api?username=naistangz&show_icons=true&theme=synthwave)](https://github.com/naistangz/github-readme-stats)



<!--START_SECTION:waka-->
name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'

jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
          SHOW_OS: "True"
          SHOW_PROJECTS: "True"
          SHOW_COMMIT: "True"
          SHOW_LANGUAGE: "True"
          SHOW_TIMEZONE: "True"
          
<!--END_SECTION:waka-->
