

# Salom, men Shahriyor! 👋

### 👨‍💻 Front-end Dasturchi

- 🚀 Hozirda HTML, CSS va UI/UX dizaynlarini o'rganyapman.
- 🛠 Loyihalarimda Git va GitHub-dan faol foydalanaman.
- 🔭 Maqsadim: Kuchli dasturchi bo'lib yetishish va chiroyli interfeyslar yaratish.

### 🛠 Texnologiyalar va Instrumentlar:
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

### 📊 GitHub Statistikalarim:
![Shahriyor's GitHub stats](https://github-readme-stats.vercel.app/api?username=FLESH-2012&show_icons=true&theme=dark&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=FLESH-2012&layout=compact&theme=dark&hide_border=true)
![Shahriyor's Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=FLESH-2012&theme=react-dark)
![Shahriyor's Streak](https://github-readme-streak-stats.herokuapp.com/?user=FLESH-2012&theme=dark)
![snake github contribution grid snake animation](https://raw.githubusercontent.com/FLESH-2012/FLESH-2012/output/github-contribution-grid-snake.svg)
name: generate animation

on:
  # har 24 soatda avtomatik yangilanadi
  schedule:
    - cron: "0 */24 * * *" 
  
  # xohlagan paytda qo'lda ishlatish imkoniyati
  workflow_dispatch:
  
  # har safar main branchga push bo'lganda ishlaydi
  push:
    branches:
    - main

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    
    steps:
      # github contribution grid snake animation yaratish
      - name: generate github-contribution-grid-snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          
      # yaratilgan rasmni "output" degan branchga saqlash
      - name: push github-contribution-grid-snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
