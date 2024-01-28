# Template for the MSc Thesis Website

This is a local version of the template for the Master Thesis Websites, which will be hosted in our group's website. The template is intended for the students that are finishing the thesis and want to showcase their results. You can find an example of the template being properly rendered in [here](https://andreumatoses.github.io/amr-website-new/msc_projects_finished/msc-project-template) *(Currently this is a draft of the soon to be new website of our group)*.

This local version is a bit limited in terms of styling, but it should be enough for you to be able to see more or less how it will look like at the end. There are tow options (choose one) to use this template:

1. Write it in `markdown`. This is the easiest option, but you will have to do some manual work to make sure the images are in the right place. You can see an example of this [here](msc_project_template_md_version.md). The main problem would be that the local rendering is limited to render it as a `.md` file, so you may not know how it will look like in the end.

2. Write it in `html`. This is a bit more complicated, but you will have more control over the styling. You can see an example of this [here](msc_project_template_html_version.html). Additionally you can render it locally without any extra work.

> **Tip:** Regarding the styling (CSS)
> The website uses [bootstrap 5](https://getbootstrap.com/) for the styling, so you can use any of the components from there. Check the documentation as they have many examples. ChatGPT can be quite helpful too. If you require any extra special styling, add it in the same html file.

## Get started:

You can clone the repository or just download the files.

1. Make sure you have all the images you want to use in the folder `assets/images/msc_projects/YY_my-title/`. Make sure you rename the folder `YY_my-title` to your year and title. For example, if you are in the year 2021 and your title is "My Awesome Project", then the folder should be `assets/images/msc_projects/21_my-awesome-project/`. Same for the files inside the respective folder.

2. Rename the file of choice `msc_project_template_xx_version` to `YY_my-title.md` or `YY_my-title.html` respectively. Delete the file you have not used.

> **Warning:** Regarding File Size
> For images, make them a small size (~1MB). Keep videos light too (.mp4 with low bitrate, not too long). If you have a big video, consider uploading to youtube and embedding it. You should also have your images in standard aspect ratios such as 1x1 or 4x3, especially of they will displayed next to each other. The cove image should be 1x1 (square).

## What to do before sending it to your supervisor

1. Fill the Front Matter with all the data appropriately. The front matter is what is defined between the `---` at the beginning of the file. 

    This is an example of the front matter:

    ```yaml
    ---
    title: "Sampling Based MPC for Motion Planning of Autonomous Vehicles"
    authors:
        - name: "John Doe"
        url: "https://andreumatoses.github.io/"
        superscript: "*1"
        - name: "Luzia Knödler"
        url: "https://andreumatoses.github.io/"
        superscript: "1"
        - name: "Ludwig van Beethoven"
        url: "https://andreumatoses.github.io/"
        superscript: "†"
    affiliations:
        - name: "Equal contribution"
        superscript: "*"
        - name: "TU Delft"
        superscript: "1"
        url: "https://tudelft.nl"
        - name: "Wien Opera House"
        superscript: "†"
    end_date: 2022-01-01 # end date if ended, approximated if not sure. Just for display purposes and ordering.
    # This is the short project description, displayed in the project's card"
    description: "This project explores ..."
    cover_image: /assets/images/msc_projects/msc_project_template/jackal.jpg # Image displayed in the project's card, make it aspect ratio 1x1 (square) for best results, and keep it a reasonable size (like 1-2MB). Can also be a gif. !!!! This image link does NOT need to be fixed.
    links: # If you have other website for the project, github repos, datasets, etc. put it here. You can also add an icon from https://icons.getbootstrap.com/
        - name: Paper
        icon: bi-file-earmark-pdf
        url: "/"
        - name: arXiv
        url: "/"
        - name: Code
        icon: bi-github
        url: "/"
        - name: Video
        icon: bi-youtube
        url: "/"
    ---
    ```
2. Make sure the website renders decently enough for small devices such as phones. You can do this by resizing the browser window to a small size and see if it looks good. If not, you may have to change some of the styling. If you don't know how to do this, just stick to the responsive columns for images that are present in the template.

3. **FIX ALL THE RELATIVE LINKS!** This is the most important part. You will have to change all the relative links to the images, videos or files. For example, if you have an image in `"/assets/images/msc_projects/21_my-awesome-project/my-image.png"`, then you will have to change the relative link to `"{% include fix_link.html link='/assets/images/msc_projects/21_my-awesome-project/my-image.png' %}"`. This is because the website uses jekyll, which requires some extra care with local links. If you don't do this, the images will not be rendered correctly.


4. FINALLY, If you used the .html version, delete all the header and other code wrapping the body. This is indicated by the comments:

    ```html
    <!-- THESE IS THE HEAD, WHERE ALL THE BASIC CSS , JS etc, IS LOADED-->
    <!-- ONLY HERE SO YOU CAN RENDER IT LOCALLY -->
    <!-- ONCE DONE, DELETE FROM HERE TO THE NEXT DELETE COMMENT !!!! -->
    ...
    <!-- DELETE UNTIL HERE.  -->
    <!-- YOU NEED TO ALSO DELETE THE CLOSING OF THE BODY, BOTTOM OF THE DOCUMENT-->
    ```

    and the closing of the body:

    ```html
    <!-- DELETE THIS TOO FROM HERE -->
    ...
    <!-- DELETE UNTIL HERE -->
    ```

## Recommendations

Keep it brief and avoid adding many mathematical equations or code snippets unless they are very relevant. This is mostly to show your results, demos, usecases, etc. You can always add a link to the paper or code if you want to show more details.

Some cool websites for inspiration:

- [Eureka: Human-Level Reward Design via Coding Large Language Models](https://eureka-research.github.io/)
- [Nerfies: Deformable Neural Radiance Fields](https://nerfies.github.io/)
- [RT-2: Vision-Language-Action Models ](https://robotics-transformer2.github.io/)
- [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware](https://tonyzhaozh.github.io/aloha/)

You cal also check the websites of  [students from previous years](https://andreumatoses.github.io/amr-website-new/msc_projects_finished/). There may still not be any as this is new (2024).