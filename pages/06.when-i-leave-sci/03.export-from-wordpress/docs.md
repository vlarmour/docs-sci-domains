---
title: 'Export from WordPress'
taxonomy:
    category:
        - docs
visible: true
---

If you are using your WordPress, you can also get an export of your posts, pages, comments, custom fields, categories, and tags.

The WordPress export is great for grabbing the content of your WordPress site so that you can import it into another WordPress host, such as WordPress.com or WordPress.org.

> Note: Exports do not include plug-ins, or other site customizations.

## Exporting
From the **Dashboard** navigate to _Tools>Export_.

The Export page shows how to export all of your posts, pages, comments, custom fields, terms, navigation menus, and custom posts. However, you can also export just certain posts, pages, or media.

This export process generates an XML file of your blog’s content. WordPress calls this an  eXtended RSS or WXR file.

**Note**: This will ONLY export your **posts**, **pages**, **comments**, **categories**, and **tags**; uploads and images _may_ need to be manually transferred to the new blog. If possible, do not delete your blog until after media files have successfully been imported into the new blog.

## Importing
Once you have exported your posts, pages, etc., you can import them into your new WordPress site.
1. Login to your new WordPress.com or self-hosted WordPress site and go to the Dashboard.  From there navigate to **Tools>Import** and click on the link to “**Run Importer**“
2. Next you will see a screen that prompts you to upload the WXR (.xml) file you generated through the export process. Browse to your exported WordPress archive and then click the “**Upload file and import**” button.
3. Choose and upload your file.  You will then be prompted to assign an author to the posts that you are importing.  You can use this function to assign one author to all posts, or you can manually set the author for each post in the posts menu. Unless you have a space limit, you will also want to select the option to “download and import file attachments” before clicking the “**Submit**” button.
4. When your import is complete, you will see a confirmation screen.

Your exported content is now added to your site. If you had posts on your site prior to importing, those posts are still available.

Because the export did not include themes or plug-ins, you will need to reinstall those separately from the export/import process.