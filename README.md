<img src="https://i.imgur.com/ZG4gSnb.jpeg" alt="demo"/>

# Photography ![OpenCollective](https://opencollective.com/photography/tiers/backer/badge.svg?label=backer&color=brightgreen)
A jekyll website for photographers

## Highlights
1. Easy setup and you get a website of your own for __free__. No web hosting charges too.
2. To add new pictures, you need to just upload them. __No code__ changes required.
3. And, my favorite, you get to see EXIF data like __aperture, shutter speed, iso__ etc. when you click on any image, automagically. Moreover, you can customize this as per your needs.

## Quick Start
If you know a tad about tech and love taking pictures then this open-source project may help you setup a website to showcase
all your creations without effort. And not just that, with this you need not pay a single dime to host your website as
it's hosted by GitHub for __free__.

**Just follow the below steps and your website would be live in no time:**

1. Fork this repo by hitting the `Fork` button at the top right corner.
2. Enable github pages from the repo settings.
3. Upload your pictures to `images/fulls` and `images/thumbs` directory. _You can do that on github.com itself or you can clone and push the images to your repo._
4. Add your own custom domain in `CNAME` file or just remove the file if you don't own a domain and use the default domain that github provides ([yourusername].github.io/photography).
5. Update `baseurl` field in `_config.yml` file with whatever domain you used in step 4.
6. And that's it, your website is set. To view, go to [photography.rampatra.com](http://photography.rampatra.com) (or whatever you have in the CNAME file) and if you don't have one, you can go to [[yourusername].github.io/photography](http://yourusername.github.io/photography)

And, of course, you don't want my name at the bottom to show up. You can change it in `_config.yml` file as well as a few other settings like your social links, google analytics, etc. Just do not forget to [build the website](#build-the-website) after you make the changes.

## Run the website locally to test
1. `$ cd photography` - go to the project directory
2. `$ bundle install` - install gems
3. Change the `baseurl` in `_config.yml`
4. `$ bundle exec jekyll serve` - start/run the website

### Build the website (updated by Luke)
1. `$ npm install` - install all npm dependencies
2. `python resize_images.py` - After putting the full-sized images in the /thumbs folder, type this to resize all images in /thumbs to thumbnails
3. `$ gulp` - minify css, js, resize images, etc.

### Naming convention for folders and images
Folders are named using the following format:
YYYY.MM.DD-PhotoLocation-Sport@HomeOrAway

For example: 2025.1.18-WashU-MBB@Home

Images do not have a specific naming convention. It seems like Jekyll doesn't like when
image files lead off with an underscore (_), so if your camera prefaces image files with an
underscore, make sure to remove it before pasting your images in fills and thumbs (or just
rename the file before you export it in Lightroom).

Valid filename: DSC-1234.jpg

Invalid filename: _DSC-1234.jpg

Note: You only need to build the website if you make changes such as replacing the images, modifying the css styles, etc.
 
## ProTips

### Contact Form
You can make the contact form work without the need of any server-side code. Just follow this [article on github](https://github.com/dwyl/html-form-send-email-via-google-script-without-server) which uses a simple google script to send emails or to upload to a google spreadsheet when someone submits the form.

## Credits
Thanks to [AJ](https://twitter.com/ajlkn) for the website template which I enhanced for [jekyll](http://jekyllrb.com/).

## Sponsors

Proudly sponsored by [Presentify](http://presentify.compzets.com?ref=GitHub), [ToDoBar](http://todobar.compzets.com?ref=GitHub), and [FaceScreen](https://facescreenapp.com/). Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://x.com/rampatra_)]

<table>
    <tr>
        <td>
            <a href="https://presentifyapp.com/" target="_blank"><img src="https://presentifyapp.com/assets/img/presentify/app-icon-512.png" width="150" height="150"></a>
        </td>
        <td>
            <a href="https://todobarapp.com/" target="_blank"><img src="https://todobarapp.com/assets/img/todobar/app-icon-512.png" width="150" height="150"></a>
        </td>
        <td>
            <a href="https://facescreenapp.com/" target="_blank"><img src="https://github.com/user-attachments/assets/b251b413-ccc4-48f1-a316-c2c2a71f959e" width="150" height="150"></a>
        </td>
    </tr>
</table>

---

_P.S. For any queries or concerns, you can reach out to me on [Twitter](https://twitter.com/ram__patra). I'll try my best to help 🙏._
