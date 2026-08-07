<div align="center">
  <img src="https://img.shields.io/badge/CORE_STATUS-ONLINE-00FF66?style=for-the-badge&logo=probot&logoColor=black&labelColor=0a0a0a" alt="Core Status" />
  <img src="https://img.shields.io/badge/NEURAL_ENGINE-ACTIVE-00E5FF?style=for-the-badge&logo=openai&logoColor=black&labelColor=0a0a0a" alt="Neural Engine" />
  <img src="https://img.shields.io/badge/AI_MODEL-GPT_4o_FINE_TUNED-7928CA?style=for-the-badge&logo=anthropic&logoColor=white&labelColor=0a0a0a" alt="AI Model" />
</div>
<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="https://github-readme-stats.vercel.app/api?username=polsoadas&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub Stats" />
      </td>
      <td align="center">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=polsoadas&layout=compact&theme=tokyonight&hide_border=true&langs_count=7" alt="Top Languages" />
      </td>
    </tr>
  </table>
</div>
name: Metrics
on:
  schedule: [{cron: "0 0 * * *"}]
  workflow_dispatch:

jobs:
  github-metrics:
    runs-on: ubuntu-latest
    steps:
      - uses: lowlighter/metrics@latest
        with:
          filename: metrics.svg
          token: ${{ SECRETS.METRICS_TOKEN }}
          user: polsoadas
          template: classic
          base: header, activity, community, repositories, metadata
          plugin_languages: yes
          plugin_languages_ignored: html, css
          plugin_languages_details: bytes-size, percentage
          plugin_languages_limit: 8
          plugin_isocalendar: yes
          plugin_isocalendar_duration: half-year
          style_header: yes

      <div align="center">
  <img src="https://github.com/polsoadas/polsoadas/blob/master/metrics.svg" width="100%" alt="Metrics Dashboard" />
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=polsoadas&theme=tokyonight&hide_border=true&background=0d1117&fire=00ff66&sideLabels=true" alt="GitHub Streak" />
</div>
