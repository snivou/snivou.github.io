# hugo-pillar-theme

This is a **[Hugo](https://gohugo.io/)** port of the **[Pillar](https://themes.3rdwavemedia.com/bootstrap-templates/all/free-bootstrap4-resume-cv-template-for-developers-pillar/)** theme, a resume/cv template for developers

1. **[Screenshot](#screenshot)**
1. **[Install](#install)**
1. **[Customize resume information](#customize-resume-information)**
1. **[Customize profile image](#customize-profile-image)**
1. **[Preview](#preview)**
1. **[Credits](#credits)**


## Screenshot
![screenshot](https://themes.3rdwavemedia.com/wp-content/uploads/2018/05/Bootstrap-Resume-CV-Template-Pillar-Pormo.jpg "Pillar screenshot")


## Install
- Create a new `Hugo` site
- Clone the theme repo to your Hugo's site `themes` folder

```
$> hugo new site my_resume
$> cd my_resume
$> mkdir themes
$> cd themes
$> git clone https://github.com/ifarfan/hugo-pillar-theme.git

```


## Customize resume information
- Copy `config.toml` to the root of your Hugo site and update the corresponding variables
- Copy `themes/hugo-pillar-theme/data/resume.yaml` to your Hugo's site `data` folder and update the file with your own resume data, ensure that YAML syntax is correct

```
$> cp themes/hugo-pillar-theme/config.toml .
$> cp themes/hugo-pillar-theme/data/resume.yaml data/

#... edit now the 2 newly copied files with your editor of choice
```


## Customize profile image
- Create folder location for your own profile image/picture
- Copy/move your picture to this folder
- Ensure your image filename is updated under `data/resume.yaml`, under `'profile'` > `'image'`

```
$> mkdir -p static/assets/images/
$> cp my_picture_full_path/image.png static/assets/images/

#... edit data/resume.yaml, search for 'profile.jpg' and update with the filename of your image
```


## Preview
- From the root of your Hugo site, run `hugo server -v` and navigate to `http://localhost:1313/` to preview your resume
- Update your data and/or content files until satisfied
- Once completed, run `hugo` one more time and upload the contents of the `public` folder to your own site

```
#... scaffold your resume
$> hugo server -v

#... browse your resume under http://localhost:1313/
#... hugo will automatically reload your file changes, repeat until satisfied

#... once everything looks good, build it:
$> hugo

#... your new site files will be under the 'public/' folder

```


## Credits
[Xiaoying Riley](http://themes.3rdwavemedia.com) for providing a lovely + clean + crisp theme

[Pavel Kanyshev](https://github.com/aerohub/hugo-orbit-theme) for theme porting inspiration
