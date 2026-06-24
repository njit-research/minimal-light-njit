---
layout: homepage
---

<h1 class="visually-hidden">About My Research and Portfolio</h1>

<h2 style="margin: 40px 0px 10px;">About this template</h2>

This is a template for building a website on NJIT's Github Enterprise Cloud powered by Jekyll and the Minimal Light theme. To build your website using this template, fork this repository and name it, preferably,  _ucid_ or _firstname.lastname_. The url for the rendered website will be either https://sites.njit.edu/repositoryname

**You are not required to use this template to build your website. Many academic sites are built using [al-folio](https://github.com/alshedivat/al-folio), [academicpages](https://github.com/academicpages/academicpages.github.io), [academic-website](https://github.com/sbryngelson/academic-website-template) and [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes).** Choose the one that is a reflection of you or build your own.

**Note: ARCS and IST do not claim that this template meets all the WCAG compliance standards. You are required to ensure that your site meets these standards.**

## Building your website

### Configuration
* Modify the `_config.yml` file with your information. 
* If you do not want the google scholar, github, linkedin, twitter on the left sidebar, feel free to comment those lines.
* Currently the Highlanders logo is used as your profile picture. Copy your profile picture to assets/img and replace `NJIT_Highlanders_logo.png` with the name of the profile picture.  
* This website is built on Jekyll using the <a href="https://github.com/yaoyao-liu/minimal-light" aria-label="GitHub repository for the Minimal Light Jekyll theme">minimal light</a> theme originally created by <a href="https://yaoyaoliu.cs.illinois.edu" aria-label="Personal academic website of Yaoyao Liu">Yaoyao Liu</a> and modified by ARCS.
  * Please keep this attribution as is by not modifying the author line in the Footnote section. 
  * Please free to change/comment the copyright line.

### Content

This site is build with pages for:

* Home (`index.md`) - Current page.
* Research (`research.md`) - for discussing your ongoing and past research.
* Publications (`publications.md`) - for providing your scholarly product; publications, talks, etc.
* People (`people.md`) - page dedicated to highlight your research group. The default page shows the ARCS team as of June 2026.
* Teaching (`teaching.md`) - for providing information on your current and past courses taught.

The following pages can be found in the `_includes` directory:

* News and Events (`news.md`) - Adds to the news section below. If you do not want to provide a news feed, delete the section below.
* Contact Information (`contact.md`) - Adds your contact information below.

If you need to add more pages, create it in the top level of this repository. If you want it to appear in the navigation bar, edit the `_data/navigation.yml` file to add the page you created. 

If you delete any of these default pages, edit the `_data/navigation.yml` to remove the link in the navigation bar.

### Already using github and github pages for your website

If you are already host your website on github and want to host it on NJIT's github, you have two options:
1. Move your repository from your personal account to NJIT's github. You will need to change the repository name from _username.github.io_ to either _ucid_ or _firstname.lastname_. 
2. Continue hosting it on your personal github and add NJIT github as an additional remote:
```bash
git remote add njit git@github.com:njit-research/ucid.git
git push njit main
```

verify or recreate the github actions to deploy your website. You will now have the same website at https://username.github.io and https://sites.njit.edu/ucid

Note: You are not limited to ucid or firstname.lastname for repositories names. You can also use researchlabofucid for a https://sites.njit.edu/researchlabofucid

{% include_relative _includes/news.md %}

{% include_relative _includes/contact.md %}


