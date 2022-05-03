<p align="center">
  <img width="60%" alt="Infinity" src="https://user-images.githubusercontent.com/28684401/150548363-39ebd24a-d79a-40c2-b195-abd8ae8858fe.gif" />
</p>

> 💻  I am a frontend developer. I use mostly React & other JS libraries in my work.

> 🤓  What I learned today : In hooks useCallback(fn, deps) is equivalent to useMemo(() => fn, deps).

> 📫  💬   How to reach me: 📱

<img width="20%" align="right" alt="Github" src="https://raw.githubusercontent.com/onimur/.github/master/.resources/git-header.svg" />

<details>
  <summary>Github usage stats!</summary>
  
 ![Github Stats for Maia313 repositories](https://github-readme-stats.vercel.app/api?username=Maia313&show_icons=true&count_private=true&title_color=FF69B4&icon_color=FF69B4&text_color=FF69B4&bg_color=ececec) 
  
  ![Github Stats for Maia313 most used languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Maia313&title_color=FF69B4&icon_color=FF69B4&text_color=FF69B4&bg_color=FFF&layout=compact) 


</details>

jobs:
  publish:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@master
        with:
          persist-credentials: false
          fetch-depth: 0
      - name: Create README.md
        uses: actions-js/profile-readme@master
        with:
          username: <your username>
          github_token: ${{ secrets.GITHUB_TOKEN }}
      - name: Commit & Push changes
        uses: actions-js/push@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
