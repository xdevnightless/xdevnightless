
# Hello 👋
14 y/o Full Stack Developer
Owner of Acceleration

# Projects
Acceleration V1 

# Languages/Tools

[![My Skills](https://skillicons.dev/icons?i=js,html,css,python,scss,react,replit,vscode,github,discord,bots,gmail,instagram,java)](https://skillicons.dev)
<p href="https://github.com/xdevnightless/Acceleration" align="left">
const axios = require('axios');
const sharp = require('sharp');

// Fetch the image from the GitHub stats API
const statsImageURL = 'https://github-readme-stats-git-masterorgs-github-readme-stats-team.vercel.app/api?username=xdevnightless&include_orgs=true&show_icons=true&hide_border=true&theme=tokyonight&locale=en';

// Download the image
axios({
  url: statsImageURL,
  responseType: 'arraybuffer',
})
  .then((response) => {
    const buffer = Buffer.from(response.data, 'binary');
    
    // Use sharp to add text overlay
    sharp(buffer)
      .composite([
        {
          input: Buffer.from('<svg><text x="10" y="20" font-size="20" fill="white">776 contributions</text></svg>'),
          top: 10,
          left: 10,
        },
      ])
      .toFile('output-stats.png', (err, info) => {
        if (err) {
          console.error(err);
        } else {
          console.log('Image with overlay created:', info);
        }
      });
  })
  .catch((err) => console.error(err));





<h3 align="center">Connect with me:</h3>
<p align="center">
 <a href="mailto:shadowiscool@zombi3slayz.com
" target="blank"><img align="center" src="https://media.xordas.me/movie-river/email_icon.svg" alt="shadowiscool@zombi3slayz.com
" height="30" width="40" /></a>
<a href="https://discord.com/users/123456789012345678" target="blank">
  <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt=".xxnightless" height="30" width="40" />
</a>
<a href="https://www.youtube.com/@shadowycc" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="xordas" height="30" width="40" /></a>
</p><br>





    

















<!---
xdevnightless/xdevnightless is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
