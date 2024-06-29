### Comprehensive Report on the Implementation and Management of the CS2Italy2025 Conference Website

#### Introduction
The CS2Italy2025 website serves as the official platform for the first Conference on Computational Social Science in Italy. This comprehensive report provides an in-depth overview of the implementation process, detailing the selection and adaptation of the template, integration with Jekyll, hosting on GitHub Pages, and the mechanisms for updating content. The site is designed to be a central hub for event information, registration, and updates, ensuring a seamless experience for both organizers and participants.

#### 1. Template Selection
The website was developed using the Bootstrap version 5.3.2 template provided by Bootstrapmade. The chosen template, "The Event" (available [here](https://bootstrapmade.com/theevent-conference-event-bootstrap-template/)), was specifically designed for event websites, making it an ideal fit for the CS2Italy conference.

The selection process focused on identifying a template that offered both visual appeal and functional flexibility. "The Event" template was chosen due to its clean design, responsive layout, and ease of customization. Its features, such as a built-in event schedule, speaker profiles, and registration sections, were particularly well-suited for the needs of the CS2Italy conference.

#### 2. Template Adaptation
The website structure was planned starting from the template and adapted to meet the specific needs of the client. This adaptation process included:

- **Defining the Structure:** Creating necessary sections for the website, such as the main page, event information, topics, dates, and registration methods. Each section was tailored to provide clear and concise information, ensuring that visitors could easily find what they needed.
- **Choosing Colors and Images:** The site's color scheme was defined to align with the branding of the CS2Italy conference. The primary colors used are detailed below, with their respective RGB codes in hexadecimal. Additionally, images released under a reuse license were selected, and clickable information was added to enhance user interaction.

#### 3. Colors Used
The primary colors used on the site, along with their respective RGB codes in hexadecimal, are:

- **White:** #F8F8F8 (RGB: 248, 248, 248)
- **Dark Blue:** #0D1329 (RGB: 13, 19, 41)
- **Medium Blue:** #2D3548 (RGB: 45, 53, 72)
- **Grayish Blue:** #494E5E (RGB: 73, 78, 94)
- **Dark Gray:** #3C4254 (RGB: 60, 66, 84)

These colors were chosen to create a professional and cohesive look, ensuring good contrast and readability across all devices.

#### 4. Integration with Jekyll
The template was adapted to work with Jekyll, a static site generator. Jekyll was chosen for its simplicity and efficiency in managing static websites. This choice allowed for more efficient content management and straightforward publishing on GitHub Pages. Jekyll's modular structure facilitated the organization of content into distinct sections, making updates and maintenance straightforward.

#### 5. Publishing on GitHub Pages
The site was hosted on GitHub Pages, leveraging its seamless integration with Git repositories. The project repository is accessible [here](https://github.com/CS2Italy/conference), allowing all members of the CS2Italy organization on GitHub to access, make changes, and updates.

Using GitHub Pages provided several advantages, including automatic deployment of changes, version control, and collaboration features. It also ensured that the site could be quickly restored to a previous state if needed.

#### 6. Domain Configuration
A DNS domain was associated with the site published on GitHub Pages, making it accessible at https://cs2italy.org/. This custom domain configuration enhances the site's professionalism and makes it easy for attendees to find.

#### 7. Font Used
The font used for the site is "RedHatDisplay", which is licensed under the SIL Open Font License 1.1. This license allows for both personal and commercial use, modification, and redistribution, with certain conditions:

- **Permissions:**
  - The font can be used, studied, modified, and redistributed freely.
  - It can be bundled, embedded, and redistributed with software.

- **Restrictions:**
  - The font cannot be sold by itself.
  - Derivative works can be released under the same license.
  - The font name must not be used to promote the derivative work without permission.

#### 8. Privacy and Cookies
The site does not load resources from domains other than the main page's domain. Additionally, it does not use cookies and therefore does not track any personal information. This commitment to privacy is also stated in the cookie law banner, ensuring that visitors are aware of the site's privacy practices.

#### 9. Third-Party Files
All third-party files (JavaScript, CSS, fonts, etc.) are located in the `assets` directory of the project. This approach ensures that all resources are self-contained within the site, improving load times and security.

### Detailed Content Update Procedure
Content updates are managed through a combination of configuration files, Markdown files for text content, CSV files for tabular data, and images stored in a designated directory. Below are the specific details on which files to update for different sections of the website:

#### Basic Information
The `_config.yml` file contains essential site-wide settings, including:

- **title:** The title of the site.
- **description:** A detailed description of the event used for meta tags and SEO.
- **keywords:** SEO keywords.
- **year:** The year of the event.
- **datelocation:** The dates and location of the event.
- **organizers:** The organizers of the event.

To update these settings, edit the `_config.yml` file directly in the repository.

#### Text Content
Text content is organized in the `_texts` directory with Markdown files for each section:

- **01_about.md:** Contains the main website description.
- **02_topics.md:** Describes the conference topics.
- **03_dates.md:** Lists the conference dates.
- **04_registrationfees.md:** Describes registration fees.
- **05_sponsors.md:** Provides information about the sponsors.

To update text content, edit the corresponding Markdown file in the `_texts` directory.

#### Tabular Data
Tabular information is stored in the `_data` directory in CSV files:

- **organizers.csv:** Lists the event organizers.
- **scientific_committee.csv:** Lists members of the scientific committee.
- **program_day1.csv, program_day2.csv, program_day3.csv, program_day4.csv:** Contain the detailed schedule for each day of the conference.
- **sponsors.csv:** Lists the event sponsors.

To update tabular data, edit the corresponding CSV file in the `_data` directory.

#### Images
Images used on the site are stored in the `docs/assets/img/` directory. This directory contains specific subfolders:

- **docs/img/assets:** Contains sponsor logos.
- **docs/img/gallery:** Contains images used for the venue section.

To update images, add new images to the appropriate subfolder and update any references to these images in the site’s code if necessary.

### Updating Procedure
To update any content on the site, follow these general steps:

1. **Clone the Repository:** Clone the site's GitHub repository to your computer.
   ```sh
   git clone https://github.com/CS2Italy/conference.git
   ```

2. **Modify the Files:** Make the necessary changes to the Markdown, CSV, or image files.

3. **Commit and Push Changes:** Commit the changes to the repository and push them to GitHub.
   ```sh
   git add .
   git commit -m "Content update"
   git push origin main
   ```

4. **Verify Changes:** Verify that the changes have been applied correctly by visiting the website.

### Alternative: Updating Through GitHub Web Interface
Alternatively, updates can be made directly through the GitHub web interface:

1. **Access the Repository:** Access the site’s repository on GitHub at [https://github.com/CS2Italy/conference](https://github.com/CS2Italy/conference).

2. **Modify the Files:** Navigate to the file you want to update (e.g., `_config.yml`, a Markdown file in the `_texts` directory, or a CSV file in the `_data` directory) and click the pencil icon to edit the file.

3. **Save Changes:** Make the necessary changes and scroll down to commit the changes. You can add a commit message to describe the changes made.

4. **Verify Changes:** Verify that the changes have been applied correctly by visiting the website.

### Paper Review and Conference Registration
For the review of papers to be submitted and conference registration, third-party platforms will be used based on the client's preference. Links and references to these platforms will be simply integrated into the website. For the review process, we recommend using OpenReview ([https://openreview.net](https://openreview.net)). For ticket management, consider evaluating platforms such as Eventbrite ([https://www.eventbrite.com](https://www.eventbrite.com)), Ticket Tailor ([https://www.tickettailor.com](https://www.tickettailor.com)), or Pretix ([https://pretix.eu](https://pretix.eu)).

### Conclusion
The creation of the CS2Italy2025 website followed a methodical process of selection, adaptation, and implementation, using modern technologies and efficient content management platforms. The result is a functional and easy-to-update website that effectively supports the organization of the Computational Social Science conference in Italy.

This comprehensive approach ensures that the website not only meets the immediate needs of the conference but is also scalable and adaptable for future events. By leveraging GitHub Pages and Jekyll, the CS2Italy team can maintain a high level of control over content and updates, ensuring the site

 remains current and relevant.

If you need further details or assistance with specific technical aspects of the project, feel free to ask!
