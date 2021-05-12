### Hi, I'm Anodeus <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px">
[![Website](https://img.shields.io/badge/Text-Text-green?style=flat-square)](https://google.com)
## Your short description
- 🔭 I’m currently working on - ❔❔❔❔
- 🌱 I’m currently learning - ❔❔❔❔
- 👯 I’m looking to collaborate with - ❔❔❔❔
- 💬 Ask me about - ❔❔❔❔
- 🥅 2020 Goal - ❔❔❔❔
- ⚡ Fun fact - ❔❔❔❔
<!-- ❔❔❔❔ means username in below README.md -->
<!-- Also feel free to update second URL to any URL -->
[![Abhi's github stats](https://github-readme-stats.vercel.app/api?username=anodeus&count_private=true&include_all_commits=true&theme=radical)](https://google.com)
## Connect with me:
[<img align="left" alt="codeSTACKr.com" width="22px" src="https://raw.githubusercontent.com/iconic/open-iconic/master/svg/globe.svg" />][website]
[<img align="left" alt="codeSTACKr | Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" />][twitter]
[<img align="left" alt="codeSTACKr | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
<br />
<!-- Optional if you have blogs -->
## Latest blog posts:
<!-- BLOG-POST-LIST:START -->
<!-- BLOG-POST-LIST:END -->
<!-- This section you create this variables that are used above -->
[website]: https://google.com
[twitter]: https://twitter.com/
[linkedin]: https://www.linkedin.com/in/abhi-singh-as/

name: Latest blog post workflow
on:
  schedule: # Run workflow automatically
    - cron: '0 * * * *' # Runs every hour, on the hour
  workflow_dispatch: # Run workflow manually (without waiting for the cron to be called), through the Github Actions Workflow page directly
jobs:
  update-readme-with-blog:
    name: Update this repo's README with latest blog posts
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: gautamkrishnar/blog-post-workflow@master
        with:
          feed_list: "https://dev.to/feed/gautamkrishnar,https://www.gautamkrishnar.com/feed/"
