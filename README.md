# Big Book of R

Welcome to the Big Book of R repository! This repository hosts a collection of nearly 400 R programming books, most of which are freely available. The project is open to contributions of both free and paid books.

## Getting Started

To work with this repository, you need to have some tools and libraries installed on your system:

### Prerequisites
- **Quarto:** We use Quarto to render the books. Make sure Quarto is installed on your machine.
- **R Programming Environment:** Ensure that R is installed.
- **R Libraries:** Install the following R libraries:
  ```R
  library(dplyr)
  library(tidyr)
  library(stringr)
  library(googlesheets4)
  library(readr)
- **Visual Studio Code (VS Code):** This project is best managed using VS Code. We recommend installing it for an optimal experience.

### Repository Structure
- `_quarto.yml`: The primary configuration file that manages the rendering of books and calls all `.qmd` files.
- `chapters/`: Directory where individual `.qmd` files are stored after fetching data from the Google Sheets.
- `scripts/`:
  - `fetch_books.R`: Script to fetch book data from Google Sheets and create `.qmd` files in the `chapters` directory.
  - `generate_ordered_list.sh`: Bash script to list `.qmd` files with their paths. The output is saved in `chapter_list.txt`.
  - `chapter_list.txt`: Text file containing the list of `.qmd` files generated by `generate_ordered_list.sh`.
- HTML files: these are part of the book rendering process.

### Setting Up Your Local Environment
1. Clone the repository to your local machine.
2. Install all the prerequisites mentioned above.
3. Ensure R and necessary libraries are installed. Use the following commands to install the required R packages if not already installed:
   ```R
   install.packages("dplyr")
   install.packages("tidyr")
   install.packages("stringr")
   install.packages("googlesheets4")
   install.packages("readr")
4. Begin by running `fetch_books.R` script to populate the `chapters` directory.
5. Use the `generate_ordered_list.sh` script to create the `chapter_list.txt` which will be used to update the `_quarto.yml` with the correct sequence of chapters.
6. Run `quarto check` to ensure your setup is correct.
7. Finally, execute `quarto preview` to render the book locally and check for errors.

## Contribution Guidelines
We welcome contributions! If you wish to add books or suggest improvements:
- Please open an issue through this link: [Issue Tracker](https://github.com/oscarbaruffa/BigBookofR/issues).
- Follow the contribution guidelines provided in the repository.

## Additional Information
The metadata about the books is stored in a Google Sheet, accessible [here](https://docs.google.com/spreadsheets/d/1vufdtrIzF5wbkWZUG_HGIBAXpT1C4joPx2qTh5aYzDg).

For any further assistance, please refer to the issue tracker and the README within the repository.
