- 👋 Hi, I’m @srkpositive
- 👀 I’m interested in Python/Automation/Data Structure Algorithm/Data Science/ML/AI
- 🌱 I’m currently learning Python/Data Science
- 💞️ I’m looking to collaborate on Data Science Project
- 📫 How to reach me? E-mail - srkpositive@gmail.com

<img 
   src="https://github-readme-stats.vercel.app/api?username=srkpositive&show_icons=true&theme=tokyonight" 
/>

name: Update README

on:
  schedule:
    - cron: '*/30 * * * *'
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: Update this repo's README with recent activity

    steps:
      - uses: actions/checkout@v2
      - uses: srkpositive/github-activity-readme@master
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
