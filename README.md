<h1 align="center">Hi 👋 We are <a href="https://github.com/ElianDochev" target="blank">
Eliyan Dochev</a> and <a href="https://github.com/VividVice" target="blank">Vasiliy Novikov!</a> </h1>
<h2 align="center">Get started with React and Gatsby</h3>

<h3 align="center" > <img src="https://media.giphy.com/media/iY8CRBdQXODJSCERIr/giphy.gif" width="30" height="30" style="margin-right: 10px;">Get in touch with us 🤝 </h3>

<div style="display: flex; flex-direction: row; justify-content: center; align-items: center;">
  <p align="center">
  <h1 align="center"> Eliyan Dochev </h1>
   <div align="center"  class="icons-social" style="margin-left: 10px;">
          <a style="margin-left: 10px;"  target="_blank" href="https://www.linkedin.com/in/elian-dochev-8a53a9250/">
  			<img  style="width: 40px; height: 40px" src="https://img.icons8.com/doodle/40/000000/linkedin--v2.png"></a>
          <a style="margin-left: 10px;" target="_blank" href="https://github.com/ElianDochev">
  		<img  style="width: 40px; height: 40px" src="https://img.icons8.com/doodle/40/000000/github--v1.png"></a>
  		<a style="margin-left: 5px;" target="_blank" href="mailto:eliyan.dochev@epitech.eu">
  					<img style="width: 40px; height: 40px" src="https://image.similarpng.com/very-thumbnail/2021/09/Outlook-icon-on-transparent-background-PNG.png" ></a>
        </div>
  </p>

  <p align="center">
  <h1 align="center"> Vasiliy Novikov </h1>

   <div align="center"  class="icons-social" style="margin-left: 10px;">
          <a style="margin-left: 10px;"  target="_blank" href="#!/">
  			<img  style="width: 40px; height: 40px" src="https://img.icons8.com/doodle/40/000000/linkedin--v2.png"></a>
          <a style="margin-left: 10px;" target="_blank" href="#!">
  		<img  style="width: 40px; height: 40px" src="https://img.icons8.com/doodle/40/000000/github--v1.png"></a>
  		<a style="margin-left: 5px;" target="_blank" href="mailto:#!">
  					<img style="width: 40px; height: 40px" src="https://image.similarpng.com/very-thumbnail/2021/09/Outlook-icon-on-transparent-background-PNG.png" ></a>
        </div>
  </p>
</div>

## Introduction

This repo is related to an [Epitech workshop](https://www.epitech.eu/) </br>
This workshop will allow you to build your first (or not) React app using [Gatsby](https://www.gatsbyjs.com/docs/),
[Material UI](https://mui.com/) and
[TypeScript](https://www.typescriptlang.org/).

## Let's start !

## Step 0 - Requirement & Configuration

### Fork the repository

For the needs of the workshop, you'll need to fork the GitHub repository on your profile.</br>
This will help us to mark you as present.
Please, fork it as a public repository, or we could not access to it, and you'll be marked as absent.

**Documentaion https://docs.github.com/en/get-started/quickstart/fork-a-repo**

Then, clone the repository on your local machine.

```bash
git clone git@github.com:ElianDochev/WorkshopReact_TS_MUI.git
```

### Install NodeJS

You will need to install [NodeJS](https://nodejs.org/en) on your machine.</br>

```bash
## On Fedora
sudo dnf install nodejs

## On Debian
sudo apt install nodejs
```

after that go to the root of the project and run the following command

```bash
npm install
```

to start the project run

```bash
npm start
```

## Step 1 - Get familiar with [Material UI](https://mui.com/)

### Step 1.0 - Your Themes

open the file `src/pages/index.tsx` and you will see the following code it is the theme that you should use for the workshop, feel free to change it if you want but you need 2 themes

```tsx
const themeOne = createTheme({
  palette: {
    primary: {
      main: "#FF4081",
      dark: "#c60055",
      light: "#ff79b0",
    },
    secondary: {
      main: "#00BFA5",
      dark: "#008e76",
      light: "#5df2d6",
    },
    background: {
      default: "#F5F5F5",
    },
    text: {
      primary: "#f34221",
      secondary: "#757575",
    },
  },
});

const themeTwo = createTheme({
  palette: {
    primary: {
      main: "#2962FF",
      dark: "#0039cb",
      light: "#768fff",
    },
    secondary: {
      main: "#FFD740",
      dark: "#c8a600",
      light: "#ffff6b",
    },
    background: {
      default: "#FFFFFF",
    },
    text: {
      primary: "#333333",
      secondary: "#757575",
    },
  },
});
```

### Step 1.1 - Create your first cpomponent and wrap it with a theme

Delete the code in the return statement and add a typography component with the following text
**Hello World**. wrap it with a theme asign it a theme color

Documentation [Text](https://mui.com/components/typography/), [Theme](https://mui.com/customization/theming/), [Palette](https://mui.com/customization/palette/)

Hint: it should look something like this

```tsx
<ThemePr?? theme={theme?}>
  <Typography variant="h1" color="?">Hello World</Typography>
</ThemePr??>
```

### Step 1.2 - Wrap your component with a wrapper

Now that you have your component, you will need to wrap it with a wrapper and center it.<br><br>
Use the Approprient component from Material UI to do so

Documentation [Box](https://mui.com/components/box/), [Center](https://mui.com/components/center/), [Grid](https://mui.com/components/grid/),
[Container](https://mui.com/components/container/)
<br><br>
Hint: it should look something like this

```tsx
<TheCompenentWrapper>
  <ThemePr?? theme={theme?}>
    <Typography variant="h1" color="?">Hello World</Typography>
  </ThemePr??>
</TheCompenentWrapper>
```

### Step 1.3 - Introduction to Grid

Now that you have your component wrapped, create copy of the Typography component and change the text to **Hello World 2**. <br><br>
Position it next to the first component using the [**Grid**](https://mui.com/components/grid/) component from Material UI.
Feel free to experiment with the different props of the Grid component.

Documentation [Grid](https://mui.com/components/grid/)
<br><br>
Hint: it should look something like this

```tsx
<TheCompenentWrapper>
  <ThemePr?? theme={theme?}>
    <Grid ? spacing={2}>
     <Grid ? xs={?}>
      <Typography variant="h1" color="?">Hello World</Typography>
     </Grid>
     <Grid ? xs={?}>
      <Typography variant="h1" color="?">Hello World 2</Typography>
     </Grid>
    </Grid>
  </ThemePr??>
</TheCompenentWrapper>
```

## Step 2 - Get familiar with [Gatsby](https://www.gatsbyjs.com/docs/)

### Step 2.0 - Understanding 404 page

The 404 page is a special page that is used when the user tries to access a page that does not exist.<br><br>
To see it in action go to the url `http://localhost:8000/404`.<br><br>
or to any other url that does not exist.<br><br>

### Step 2.1 - Create a new page

With Gatsby you can create pages dynamically, to do so you wiil need
to create a new file in the `src/pages` folder and name it `page2.tsx`.<br><br>
In this file you will need to create a new component that will display the text **Hello World From the other side**.<br><br>

You should be albe to acess it via the url `http://localhost:8000/page2`
Documentation [Gatsby](https://www.gatsbyjs.com/docs/)

### Step 2.2 - Create a link to the new page and vice versa

Now that you have your new page, you will need to create a link to it from the home page.<br><br>
Using the **Button** component from Material UI, create a link to the new page.<br><br>
Then, create a link from the new page to the home page.<br><br>

FYI: You can use the **Link** component from Material UI to create a link to a page. but only use a HTML link to go to an external page.
Documentation [Link](https://mui.com/components/links/), [Button](https://mui.com/components/buttons/)

Hint: it should look something like this

```tsx
<Link to="path of the page">
  <Button variant="?" color="?">
    Text
  </Button>
</Link>
```

### Step 2.3 - Static Gatbsy Image

Gatsby has a special component that allows you to display images. **StaticImage**, **Gatbsy Image**
<br><br>
It is very optimized and will allow you to display images in a very performant way.<br><br>
To use it you will need to import it from Gatsby and use it like this

FYI: ussually it requires some configuration but for the needs of the workshop it is already configured.

```tsx
import { StaticImage } from "gatsby-plugin-image";
```

Now embed the picture from `assets/MUI_React_ts.png` in the home page using the **StaticImage** component.
you can use whatever size you want but the image should be centered. Experiment with the different props of the component.

Hint : think about using the **Box** and **Grid** components from Material UI to center the image.

Documentation [Image Plugin](https://www.gatsbyjs.com/plugins/gatsby-plugin-image/?=gatsby%20image),
[Static Image](https://www.gatsbyjs.com/docs/reference/built-in-components/gatsby-plugin-image/#staticimage)

### Step 2.4 - GraphQL in Gatsby

In this workshop we will not delve too much into GraphQL, but it is important to know that Gatsby uses GraphQL to fetch data from the backend.
<br><br>
To see it in actions and experiment with it, go to the url `http://localhost:8000/___graphql`.<br><br>

There are several ways to use GraphQL in Gatsby, but the most common one is to use the **useStaticQuery** hook.

Using the Gatsby Filesystem Get the data from the file `src/data/data.json` and display its contents in the home page.
Use whatever component you want to display the data but prefferably use the **Typography** component from Material UI.

FIY: The configuration for the Gatsby Filesystem is already done for you.

Documentation [Gatsby Filesystem](https://www.gatsbyjs.com/docs/reference/graphql-data-layer/file-system-route-api/),
[useStaticQuery](https://www.gatsbyjs.com/docs/how-to/querying-data/use-static-query/)

### Step 2.5 - Create a component and use Gatbsy Image in it

Create a new component in the `src/components` folder and name it `Image.tsx`.<br><br>
In this component you will need to use the **Gatsby Image** component from Gatsby and display the image from `assets/MUI_React_ts.png`.<br><br>
Then, use this component in the home page and the page2 page.
pass the image information as a prop to the component.

Documentation [Gatsby Image](https://www.gatsbyjs.com/docs/reference/built-in-components/gatsby-plugin-image/)
<br><br>

Hint: This information is available in the GraphQL playground.

## Step 3 - Making your portfolio (FINAL STEP)

Using the knowledge you have gained so far, create a portfolio for yourself.

A portfolio is a website that contains information about you, your skills, your projects, your contact information, etc.

Here is the section a portfolio should have:

    Home/Introduction: This section introduces yourself, provides a brief overview of your skills and background, and sets the tone for the rest of the portfolio.

    Projects: Showcase your best projects in this section. Include project titles, descriptions, screenshots, and links to live demos or GitHub repositories. Highlight the technologies used and your role in each project.

    Skills: List the relevant skills you possess, such as programming languages, frameworks, tools, or methodologies. You can display them using tags or a visual representation like a skill meter.

    Experience: If you have professional experience, include a section that outlines your work history, job titles, and responsibilities. Briefly describe your accomplishments and the technologies you worked with.

    Education: Provide information about your educational background, such as degrees, certifications, or courses you've completed. Mention any academic achievements or relevant coursework.

    Testimonials: If you have received positive feedback or testimonials from clients, colleagues, or professors, include a section where you can showcase these recommendations. Testimonials add credibility and can help potential employers or clients gauge your skills and work ethic.

    Contact: Create a contact section with your email address, phone number, and links to your professional social media profiles (LinkedIn, GitHub, etc.). Add a contact form if you want to receive messages directly through your portfolio.

    Blog: If you maintain a blog, include a section where you can showcase your recent blog posts or provide a link to your blog page.

    Resume/CV: Optionally, you can include a downloadable PDF version of your resume or CV. This allows visitors to easily access and print your professional information.

    Design and Layout: Ensure that the design and layout of your portfolio are visually appealing and user-friendly. Use Material-UI components to create a consistent and responsive design. Pay attention to typography, colors, and overall aesthetics to make a good impression.
