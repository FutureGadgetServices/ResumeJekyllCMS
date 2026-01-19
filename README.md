
# Orbit
> This theme is designed by Xiaoying Riley at [3rd Wave Media](http://themes.3rdwavemedia.com/).
> Visit [her website](http://themes.3rdwavemedia.com/) for more themes.

I have made this into a Jekyll Theme. Checkout the live demo [here](https://online-cv.webjeda.com).

<table>
  <tr>
    <th>Desktop</th>
    <th>Mobile</th>
  </tr>
  <tr>
    <td>
        <img src="https://online-cv.webjeda.com/assets/images/desktop.png?raw=true" width="600"/>
    </td>
    <td>
        <img src="https://online-cv.webjeda.com/assets/images/mobile.png?raw=true" width="250"/>
    </td>
  </tr>
</table>

## Installation

* [Fork](https://github.com/sharu725/online-cv/fork) the repository;
* Go to settings and set master branch as Github Pages source;
* Your new site should be ready at `https://<username>.github.io/online-cv/`;
* Printable version of the site can be found at `https://<username>.github.io/online-cv/print`. Use a third party link https://pdflayer.com/, https://www.web2pdfconvert.com/ etc to get the printable PDF.

Change all the details from one place: `_data/data.yml`.

### To preview/edit locally with docker

```sh
docker-compose up
```

*docker-compose.yml* file is used to create a container that is reachable under <http://localhost:4000>.
Changes *_data/data.yml* will be visible after a while.

### Local machine

* Get the repo into your machine 

```bash
git clone https://github.com/sharu725/online-cv.git
```

* Install required ruby gems

```bash
bundle install
```

* Serve the site locally

```bash
bundle exec jekyll serve
```

* Navigate to `http://localhost:4000`


## Skins

There are 6 color schemes available:

| Blue | Turquoise | Green |
|---------|---------|---------|
| <img src="https://online-cv.webjeda.com/assets/images/blue.jpg" width="300"/> | <img src="https://online-cv.webjeda.com/assets/images/turquoise.jpg" width="300"/> | <img src="https://online-cv.webjeda.com/assets/images/green.jpg" width="300"/> |

| Berry | Orange | Ceramic |
|---------|---------|---------|
| <img src="https://online-cv.webjeda.com/assets/images/berry.jpg" width="300"/> | <img src="https://online-cv.webjeda.com/assets/images/orange.jpg" width="300"/> | <img src="https://online-cv.webjeda.com/assets/images/ceramic.jpg" width="300"/> |

## Credits

Thanks to [Nelson Estevão](https://github.com/nelsonmestevao) for all the [contributions](https://github.com/sharu725/online-cv/commits?author=nelsonmestevao).

Thanks to [t-h-e(sfrost)](https://github.com/t-h-e) for all the [contributions](https://github.com/sharu725/online-cv/commits?author=t-h-e).

Check out for more themes: [**Jekyll Themes**](http://jekyll-themes.com).

---

## Future Gadget Labs Contributions

### Updating Resume Contents

All resume content is managed in a single file: `_data/data.yml`

#### Main Content Sections

Edit these sections in `data.yml` to update the main body of your resume:

| Section | Description |
|---------|-------------|
| `career-profile` | Your career summary at the top |
| `education` | Degrees, universities, and timeframes |
| `experiences` | Work history with roles, companies, and details |
| `certifications` | Professional certifications |
| `projects` | Side projects and portfolio items |
| `oss` | Open source contributions |
| `publications` | Published papers or articles |
| `recommendations` | References and testimonials |
| `skills` | Skills with proficiency percentages |

#### Updating the Right Sidebar

The `sidebar` section in `data.yml` controls the right sidebar content:

```yaml
sidebar:
  position: right          # Position: left or right
  about: True              # Show "how to use?" section
  education: True          # Show education in sidebar (False = main section)

  # Profile
  name: Your Name
  tagline: Your Title
  avatar: profile.png      # Filename of your profile picture

  # Contact Links
  email: your@email.com
  phone: 012 345 6789
  website: https://yoursite.com
  linkedin: username
  github: username
  twitter: '@username'

  # Languages
  languages:
    title: Languages
    info:
    - idiom: English
      level: Native

  # Interests
  interests:
    title: Interests
    info:
    - item: Hobby
      link:
```

#### Updating Your Profile Picture

1. Place your profile image in the `assets/images/` folder
2. Update the `avatar` field in `_data/data.yml` with your filename:

```yaml
sidebar:
  avatar: your-photo.png   # Supports .png, .jpg, .jpeg
```

Recommended size: 100x100 pixels for optimal display.

### Deployment Configuration

Update `_config.yml` to match your deployment environment:

```yaml
# Site Settings
title: My Resume
url: 'https://username.github.io'    # Your site's base URL
baseurl: '/repository-name'          # Your repository name (or '' for root)
```

#### Common Deployment Scenarios

| Deployment | `url` | `baseurl` |
|------------|-------|-----------|
| GitHub Pages (project) | `https://username.github.io` | `/repository-name` |
| GitHub Pages (user site) | `https://username.github.io` | `` (empty) |
| Custom domain | `https://yourdomain.com` | `` (empty) |
| Subdirectory on custom domain | `https://yourdomain.com` | `/resume` |

**Important:** Assets and links will break if these values don't match your actual deployment URL.

---
