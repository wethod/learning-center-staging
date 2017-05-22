# learning-center-source
Here you can find all the files needed to build the site "WETHOD Learning Center". 
## Details
* The site is statically generated using [Hugo](https://gohugo.io/);
* The site is hosted on GitHub Pages;
* If you need a visual editor, you can use [Forestry.io](https://forestry.io);
* The served files are in another repo. We need to mantain different repositories for source code and served files because of Forestry.io.
## How to edit 
Using Forestry.io:
1. Login with the WETHOD account;
2. In the section "My Sites" choose "wethod-support";
3. Edit content;
4. Refresh the github.io page (clearing cache using `⌘ + MAIUSC + R`) to see the changes.

Manually:
1. Clone this repository;
2. Clone the repository which contains the served files;
3. Edit content;
4. Build with Hugo;
5. Push the changes to the source code;
6. Push the "public" folder to the repository which contains the served files;
7. Refresh the github.io page to see the changes.
