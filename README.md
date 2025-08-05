# Adding People, Categories, and Publications

## Adding a Person

To add a person to the website:

1. **Create a Markdown file** in the `_people` directory. Use the format: `firstname_lastname.md`.
2. **Use the following template** in your Markdown file:

    ```yaml
    ---
    layout: about
    firstname: Firstname
    lastname: Lastname
    description: Your description here
    img: path/to/image.jpg # Ensure this path is correct
    redirect: https://link-to-profile
    linkedin_username: linkedin_handle
    github_username: github_handle
    email: your-email@example.com
    category: Your category here
    show: true # or false to hide
    ---
    ```

3. **Upload an Image**: Place the image in the appropriate category folder within `assets/img/people/`:
   - `assets/img/people/phd/` for PhD Students
   - `assets/img/people/mtech/` for M.Tech Students
   - `assets/img/people/alumni/` for Alumni
   - `assets/img/people/project-associates/` for Project Associates
**Necessarily make the image square**

4. **Category**: You can categorize people as "PhD Students", "MSc Students", "M.Tech Students", "Alumni", "Undergraduates", or "Lab Director". Add accordingly under `category`.

5. **Image Path**: Update the `img:` field to reflect the correct folder structure, e.g., `assets/img/people/phd/yourname.jpg`

## Categories

Categories can be defined for organizing both people and collections:

- **People Categories**: Defined directly in each `_people/firstname_lastname.md` file under the `category` tag.
- **Project/Collection Categories**: Adjust these in the `_config.yml` file under collections or directly within each project/article markdown files.

## Adding a Publication

To add a publication:

1. **Edit the BibTeX file** located at `_bibliography/papers.bib`.
2. **Add a BibTeX entry** using the following template:

    ```bibtex
    @article{author2023title,
      author       = {Author, A. and Another, B.},
      title        = {Title of the Work},
      journal      = {Journal Name},
      year         = {2023},
      volume       = {10},
      number       = {1},
      pages        = {1--10},
      url          = {https://link.to/publication},
      bibtex_show  = {true}
    }
    ```

3. **Additional Info**: Optional fields include `abstract`, `doi`, `pdf`, etc., which can be linked in the assets directory.

## Organization Structure

The assets are organized in the following folder structure:

- **People Images**: `assets/img/people/[category]/` - Images organized by role (phd, msc, mtech, alumni, undergraduates, lab_director)
- **Funding Logos**: `assets/img/funders/` - All funding organization logos and sponsor images
- **Publication Previews**: `assets/img/publication_preview/` - Preview images for publications
- **Lab Photos**: `assets/img/labphotos/` - Laboratory and facility photos
- **Project Images**: Various project-specific folders for related images


