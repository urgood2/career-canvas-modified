# CareerCanvas Hugo Theme

A modern, responsive Hugo theme for personal websites and portfolios, created by Felipe Cordero. This theme is designed to showcase your professional experience, skills, and projects in a clean and elegant way, with a focus on engineering and technical portfolios.

## Features

- Responsive design with modern UI
- Dark mode support
- Portfolio showcase with image galleries
- Blog support
- Skills section with interactive cards
- Experience timeline
- Contact form
- Social media integration
- Multilingual support (English/French)
- Resume/CV integration
- Tailwind CSS for styling
- Optimized for technical and engineering portfolios

## Installation

### As a Git Submodule

```bash
git submodule add https://github.com/felipecordero/careercanvas.git themes/careercanvas
```

### As a Git Clone

```bash
git clone https://github.com/felipecordero/careercanvas.git themes/careercanvas
```

## Configuration

Add the following to your `config.toml`:

```toml
theme = "careercanvas"

[params]
  name = "Your Name"
  tagline = "Your Tagline"
  location = "Your Location"
  email = "your.email@example.com"
  profile_image = "/images/your-profile.jpg"
  description = "Your description"
  author = "Your Name"

  # Social Media
  linkedin_url = "https://linkedin.com/in/yourprofile"
  github_url = "https://github.com/yourusername"

  # Resume/CV
  resume_url_en = "/files/your-resume-en.pdf"  # Path to English resume
  resume_url_fr = "/files/your-resume-fr.pdf"  # Path to French resume (optional)
  resume_label = "Download Full Resume"

  # Social Icons
  [[params.social]]
    icon = "linkedin-in"
    url = "https://linkedin.com/in/yourprofile"

  [[params.social]]
    icon = "github"
    url = "https://github.com/yourusername"
```

## Menu Configuration

```toml
[[menu.main]]
  name = "About"
  url = "/#about"
  weight = 2

[[menu.main]]
  name = "Skills"
  url = "/#skills"
  weight = 3

[[menu.main]]
  name = "Experience"
  url = "/#experience"
  weight = 4

[[menu.main]]
  name = "Contact"
  url = "/#contact"
  weight = 5
```

## Image Galleries

The theme includes a gallery shortcode for showcasing your work:

```markdown
{{< gallery dir="images/your-gallery" >}}
```

## Development

This theme uses Tailwind CSS for styling. To modify the styles:

1. Install dependencies:
```bash
npm install
```

2. Build CSS:
```bash
npm run build:css
```

3. Watch for changes:
```bash
npm run watch:css
```

## Author

Created by [Felipe Cordero](https://felipecordero.com) - Structural engineer and software developer combining 14+ years in AEC with AI/ML expertise.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This theme is released under the MIT License. See the [LICENSE](LICENSE) file for more information. 