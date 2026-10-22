<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:3b82f6&height=170&section=header&text=WordPress%20Car%20Theme&fontColor=ffffff&fontSize=44&fontAlignY=38&desc=A%20classic%20theme%20with%20car%20listings%20and%20search&descAlignY=60&descSize=16" alt="WordPress Car Theme" />

![WordPress](https://img.shields.io/badge/WordPress-theme-21759b?style=flat-square&logo=wordpress&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-theme-777bb4?style=flat-square&logo=php&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-4-7952b3?style=flat-square&logo=bootstrap&logoColor=white)
![Advanced Custom Fields](https://img.shields.io/badge/Advanced%20Custom%20Fields-integration-00a0d2?style=flat-square)

</div>

A classic PHP WordPress theme with templates for car listings, brand archives, individual cars, and a keyword/brand search page. It also includes general page, post, archive, and search templates.

## ✨ Features

- Registers a `cars` custom post type and a `brands` taxonomy.
- Provides a car search page template and car archive/single templates.
- Uses Advanced Custom Fields (ACF) values for car details and image galleries.
- Includes Bootstrap assets, a navigation walker, and theme CSS/JavaScript.
- Adds featured-image support, menus, widgets, and custom image sizes.

## 🏗️ Architecture

WordPress loads the theme's PHP templates and `functions.php`; the theme registers the vehicle content type and taxonomy, while individual templates render posts and ACF fields. There is no separate application backend or database schema in this repository.

## 🧰 Tech stack

| Area | Technology |
| --- | --- |
| CMS | WordPress (classic PHP theme) |
| Language | PHP |
| Front-end | Bootstrap, theme CSS, JavaScript, jQuery |
| Custom vehicle fields | Advanced Custom Fields plugin |

## 🚀 Getting started

1. Install WordPress on a PHP-capable web server and configure its database.
2. Install and activate the **Advanced Custom Fields** plugin for the custom vehicle fields used by the templates.
3. Copy this repository into `wp-content/themes/` (or deploy it there with Git).
4. In **Appearance → Themes**, activate the theme.
5. Create car content and brand terms; create a page using the **Car Search** template to publish the search form.

The theme's car templates expect ACF field names such as `gallery`, `colour`, and `registration`; this repository does not include field-group exports or configure those fields.

## 📁 Project structure

```text
├── functions.php          # Theme setup, assets, content registrations
├── front-page.php         # Front-page template
├── car-search.php         # Car Search page template
├── archive-cars.php       # Car archive
├── single-cars.php        # Individual car page
├── includes/              # Reusable page sections and enquiry form
├── css/                   # Bootstrap and theme styles
└── js/                    # Bootstrap and theme scripts
```

## 🗺️ Roadmap / Notes

- This is a theme starter, not a standalone WordPress application; WordPress and ACF are external requirements.
- No automated tests or local development configuration are included.
- The Contact Us template currently contains placeholder copy for its form area.

## 👤 Author

**Brian Dol**, Senior Full Stack Engineer · [Portfolio](https://portfolio.dol-brian23.workers.dev/) · [LinkedIn](https://linkedin.com/in/brian-dol-31a06115a/)
