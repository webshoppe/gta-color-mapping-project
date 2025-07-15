# 🛠️ Community Scripts

## 📝 A Note on the Original Scripts (Why this folder is here)

The creation of this dataset was a significant data archaeology project.  The source data came from dozens of different places accumulated over many years, including .html files from the Wayback Machine, Archive.today, forum posts, text files, github repos and spreadsheets in various formats.

Because of this, the internal scripts used were written on-the-fly and on an as-needed basis.  They were typically one-off tools designed to tackle a very specific, messy data source at a particular moment, as you can tell from the `requirements.txt`.  As the dataset and formatting became more standardized, these scripts were patched, changed, and ultimately became obsolete.

In short, they were not good examples of clean, reusable code and would not be very helpful to the community.

This presents a fantastic opportunity!  Now that the dataset is clean and predictable, we are officially inviting the community to build a new generation of high-quality, reusable scripts.  Your contributions here will help other users interact with this data in new and powerful ways.

---

## ⭐ Script Wishlist

We are particularly interested in scripts that can perform tasks like:

- **Color Matching:**  Convert between hex, RGB, and other color formats.
- **Swatch Generation:**  Automatically create, name and sort image swatches from the color data.
- **Image Processing:**  Tools for resizing or manipulating related images.
- **Data Import/Export:**  Helpers for loading the data into different databases or formats.
- **Cross-Referencing:**  Tools to easily find all colors for a specific vehicle or all vehicles that use a specific livery.
- **Crew Code Updater:**  Tool to quicky update all matching hex values across all rows and sheets.
- **Color Picker:**  Tools to pick a color from another source, determine the hex/rgb and generate an entry w/ swatch and optional preview image to the 'Crew' data.

## ✍️ How to Contribute a Script

1.  Please add your script to this directory.
2.  If it has any dependencies, create a `requirements.txt` file within a sub-folder for your script.
3.  Add a brief description of your script and how to use it to this README file under a new heading.
4.  Submit a Pull Request with your changes.

**For general guidelines on creating a fork, making a branch, and submitting a Pull Request, please see our main [CONTRIBUTING.md](../CONTRIBUTING.md) file.**

---

### 🤗 Contributed Scripts

*(This section will be populated as people contribute)*

---
