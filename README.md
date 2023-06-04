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
