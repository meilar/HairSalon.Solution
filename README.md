<h1 align="center">EauClaireWare</h1>

Matthew Eilar | [LinkedIn](https://www.linkedin.com/in/eilar-503/) | [email](mailto:<meilar@gmail.com>) | [website](https://www.mattheweilar.com)

![Screenshot of webapp](/project_screenshot.jpg)
## About this project
*EauClaireWare* is a .Net 5 web application adhering to the MVC (Model-View-Controller) design pattern. This project was created as an [Epicodus](https://www.epicodus.com) weekly independent project. 

This application allows a salon owner to track a list of stylists, a list of clients, and to associate those clients with a stylist. 

## Accessing this application

### Pre-installation

Before downloading project files, you must have the following tools installed:

- You should know to open a command line on your operating system. [Here's a beginner's guide if you don't know what that means.](https://www.learnenough.com/command-line-tutorial)
- Git | [Instructions](https://github.com/git-guides/install-git)
- .NET | [Instructions](https://dotnet.microsoft.com/en-us/learn/dotnet/hello-world-tutorial/intro)
- MySQL Community Server & MySQL Workbench | [Instructions](https://www.learnhowtoprogram.com/c-and-net/getting-started-with-c/installing-and-configuring-mysql)


### Setting up your database

- Open MySQL Workbench and log into your server. 
- Select `Administration` from the `Navigator` panel.
- Select `Data Import/Restore`
- Select `Import from self-contained file`, then choose `matthew_eilar.sql` in the `HairSalon` folder.
- In `Default Schema to be Imported to`, select `New` and name the schema `matthew_eilar`. If you select a different name, the project will not load.
- Click `Start Import`
- Once the schema has been added, click on the circle with arrows icon to refresh your view, and confirm that the new schema appears in the list. If it does not appear, please try these instructions again.   

### Downloading the application

- Open your command line and clone this project with the following instruction: `$ git clone https://www.github.com/meilar/HairSalon.Solution`
- Open the project folder in a file browser. Navigate to the `HairSalon` folder.
- Create a new file named `appsettings.json`, and insert this block of code. Make sure to enter the userid and password you set up when installing MySQL Community Server in the brackets:
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=matthew_eilar;uid={YOUR USER ID HERE};pwd={YOUR PASSWORD HERE};"
  }
}
```

### Starting the application

- Navigate to the project folder in your Terminal with the following command: `$ cd HairSalon.Solution/HairSalon`
- Install project dependencies with the command `dotnet restore`
- Start the application with the following command: `$ dotnet run`
- Open the displayed URL in a web browser, typically `http://localhost:5000`. Please note that this project was designed and tested in Google Chrome, and all features may not be supported in all browsers.

## Technologies Used

This site incorporates the following frameworks and languages:

- C#
- HTML
- CSS
- Bootstrap 4
- .NET Core + Entity Core
- Git
- MySQL & MySQL Workbench

## Acknowledgements

Thank you to my partner, Alex, for support in all ways. Thank you to my parents for encouraging technology exploration, even when resources were scarce. Congratulations to the Kohlenberg Foundation for making it to another season of Survivor.

## License 

MIT License

© 2022 Matthew Eilar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
