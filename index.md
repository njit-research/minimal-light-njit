---
layout: homepage
---

<h1 id="about-me"></h1>


<h2 style="margin: 80px 0px 10px;">About this template</h2>

This is a template for building a website on NJIT's Github Enterprise Cloud powered by Jekyll and the Minimal Light theme. To build your website using this template, fork this repository and name it, preferably,  _ucid_ or _firstname.lastname_. The url for the rendered website will be either https://sites.njit.edu/repositoryname

**You are not required to use this template to build your website. Many academic sites are built using [al-folio](https://github.com/alshedivat/al-folio), [academicpages](https://github.com/academicpages/academicpages.github.io), [academic-website](https://github.com/sbryngelson/academic-website-template) and [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes).** Choose the one that is a reflection of you or build your own.

**Note: ARCS and IST do not claim that this template meets all the WCAG compliance standards. You are required to ensure that your site meets these standards.**


## Building your website

### Confguration
* Modify the \_config.yml file with your information. 
* If you do not want the google scholar, github, linkedin, twitter on the left sidebar, feel free to comment those lines
* Currently the Highlanders logo is used as your profile picture. Copy your profile picture to assets/img and replace NJIT\_Highlanders\_logo.png with the name of the profile picture.  
* This website is build on Jekyll using the [minimal light](https://github.com/yaoyao-liu/minimal-light) theme of [Yaoyao Liu](https://yaoyaoliu.cs.illinois.edu) modified by ARCS.
  * Please keep this attribution as is by not modifying the author line in the Footnote section. 
  * Please free to change/comment the copyright line.

### Content

This site is build with pages for 

* Home (index.md) -  Current page.
* Research (research.md) - for discussing your ongoing and  past research.
* Publications (publications.md) - for providing your scholarly product; publications, talks, etc.
* People (people.md) - page dedicated to highlight your research group. The default page shows the ARCS team as of June 2026.
* Teaching (teaching.md) - for providing information on your current and past courses taught.

The following pages can be found in the \_includes directory.

* News and Events (news.md) - Adds to the news  section below. If you do not want to provide a news feed, delete the section below
* Contact Information (contact.md) - Adds you contact information below.


If you need to add more pages, create it in the top level of this repository. If you want it to appear in the navigation bar, edit the \_data/navgation.yml file to add the page you created. 

If you delete any of these default pages, edit the \_data/navgation.yml to remove the link in the navigation bar. 


### Already using github and github pages for your website

If you are already host your website on github and want to host it on NJIT's github, you have two options
1. move your repository from your personal account to NJIT's github. You will need to change the repository name from _username.github.io_ to either _ucid_ or _firstname.lastname_. 
2. continue hosting it on your personal github and add NJIT github as an additional remote
```
git remote add njit git@github.com:njit-research/ucid.git
git push njit main
```
verify or recreate the github actions to deploy your website. You will now have the same website at https://username.github.io and https://sites.njit.edu/ucid

**Note: You are not limited to ucid or firstname.lastname for repositories names. You can also use researchlabofucid for a https://sites.njit.edu/researchlabofucid**
<br />



<hr>

<p>The following can be used to make announcements. If this is not useful, delete the div block</p>
<div style="border-left: 4px solid #FF5F05; padding: 10px 16px; background-color: #fafafa; color: #333; border-radius: 0 4px 4px 0; box-shadow: 0 1px 4px rgba(0,0,0,0.07);">
<strong style="color:#c0392b;">No announcements</strong>
</div>


{% include_relative _includes/news.md %}

{% include_relative _includes/contact.md %}


